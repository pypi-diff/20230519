# Comparing `tmp/syngen-0.1.2.tar.gz` & `tmp/syngen-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.1.2.tar", last modified: Fri May 19 07:30:18 2023, max compression
+gzip compressed data, was "syngen-0.1.3.tar", last modified: Fri May 19 10:36:34 2023, max compression
```

## Comparing `syngen-0.1.2.tar` & `syngen-0.1.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.022168 syngen-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-19 07:28:40.000000 syngen-0.1.2/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-19 07:28:40.000000 syngen-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-19 07:28:40.000000 syngen-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-19 07:30:18.022168 syngen-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14309 2023-05-19 07:28:40.000000 syngen-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-19 07:28:40.000000 syngen-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-19 07:30:18.022168 syngen-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.006168 syngen-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.010168 syngen-0.1.2/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.010168 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15251 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6554 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.018168 syngen-0.1.2/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.022168 syngen-0.1.2/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    33025 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.022168 syngen-0.1.2/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.022168 syngen-0.1.2/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.022168 syngen-0.1.2/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-19 07:28:40.000000 syngen-0.1.2/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 07:30:18.014168 syngen-0.1.2/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-19 07:30:17.000000 syngen-0.1.2/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-19 07:30:18.000000 syngen-0.1.2/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-19 07:30:17.000000 syngen-0.1.2/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-19 07:30:17.000000 syngen-0.1.2/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-19 07:30:17.000000 syngen-0.1.2/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-19 07:30:17.000000 syngen-0.1.2/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.409033 syngen-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-19 10:35:10.000000 syngen-0.1.3/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-19 10:35:10.000000 syngen-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-19 10:35:10.000000 syngen-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-19 10:36:34.409033 syngen-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14309 2023-05-19 10:35:10.000000 syngen-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-19 10:35:10.000000 syngen-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-19 10:36:34.409033 syngen-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.397033 syngen-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.401033 syngen-0.1.3/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.401033 syngen-0.1.3/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.401033 syngen-0.1.3/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.401033 syngen-0.1.3/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.401033 syngen-0.1.3/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7879 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.405033 syngen-0.1.3/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.405033 syngen-0.1.3/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.397033 syngen-0.1.3/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.405033 syngen-0.1.3/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.405033 syngen-0.1.3/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.405033 syngen-0.1.3/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.405033 syngen-0.1.3/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.405033 syngen-0.1.3/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.405033 syngen-0.1.3/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15251 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.405033 syngen-0.1.3/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6554 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.409033 syngen-0.1.3/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.409033 syngen-0.1.3/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33024 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.409033 syngen-0.1.3/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.409033 syngen-0.1.3/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.409033 syngen-0.1.3/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-19 10:35:10.000000 syngen-0.1.3/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 10:36:34.401033 syngen-0.1.3/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-19 10:36:34.000000 syngen-0.1.3/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-19 10:36:34.000000 syngen-0.1.3/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-19 10:36:34.000000 syngen-0.1.3/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-19 10:36:34.000000 syngen-0.1.3/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-19 10:36:34.000000 syngen-0.1.3/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-19 10:36:34.000000 syngen-0.1.3/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.1.2/LICENSE` & `syngen-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/PKG-INFO` & `syngen-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.1.2
+Version: 0.1.3
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
-Metadata-Version: 2.1 Name: syngen Version: 0.1.2 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.1.3 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.1.2/README.md` & `syngen-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/setup.cfg` & `syngen-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/infer.py` & `syngen-0.1.3/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/config/configurations.py` & `syngen-0.1.3/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/convertor/convertor.py` & `syngen-0.1.3/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.1.3/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files 10% similar despite different names*

```diff
@@ -188,14 +188,28 @@
     """
     Class for loading and saving data in YAML format
     """
     def load_data(self, metadata_path: str) -> dict:
         with open(metadata_path, "r", encoding="utf-8") as metadata_file:
             metadata = yaml.load(metadata_file, Loader=Loader)
             validate_schema(configuration_schema, metadata)
+            parameters = ["train_settings", "infer_settings"]
+            metadata = self.replace_none_values_of_metadata_settings(parameters, metadata)
+        return metadata
+
+    @staticmethod
+    def replace_none_values_of_metadata_settings(parameters, metadata: dict):
+        """
+        Replace None values for parameters
+        in the metadata
+        """
+        for table in metadata.keys():
+            for parameter in parameters:
+                if metadata.get(table).get(parameter) is None:
+                    metadata[table][parameter] = {}
         return metadata
 
     def save_data(self, path: str, df: pd.DataFrame, **kwargs):
         raise NotImplementedError("Saving YAML files is not supported")
 
 
 class BinaryLoader(BaseDataLoader):
```

### Comparing `syngen-0.1.2/src/syngen/ml/metrics/__init__.py` & `syngen-0.1.3/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.1.3/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.1.3/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.1.3/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.1.3/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.1.3/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.1.3/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/metrics/utils.py` & `syngen-0.1.3/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/reporters/reporters.py` & `syngen-0.1.3/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/strategies/strategies.py` & `syngen-0.1.3/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.1.3/src/syngen/ml/train_chain/train_chain.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/utils/utils.py` & `syngen-0.1.3/src/syngen/ml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.1.3/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/vae/models/dataset.py` & `syngen-0.1.3/src/syngen/ml/vae/models/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,14 @@
             data_subset = data_subset.dropna().apply(self._is_valid_uuid)
             self.uuid_columns_types = dict(data_subset[data_subset.isin([1, 2, 3, 4, 5, "ulid"])])
             self.uuid_columns = set(self.uuid_columns_types.keys())
             if self.uuid_columns:
                 logger.info(
                     f"The columns - {self.uuid_columns} contain UUIDs")
 
-
     def _general_data_pipeline(self, df: pd.DataFrame, schema: Dict, check_object_on_float: bool = True):
         """
         Divide columns in dataframe into groups - binary, categorical, integer, float, string, date
         in case metadata of the table is absent
 
         :param df: dataframe
         :param schema: metadata of the table
```

### Comparing `syngen-0.1.2/src/syngen/ml/vae/models/features.py` & `syngen-0.1.3/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/vae/models/model.py` & `syngen-0.1.3/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.1.3/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.1.3/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,31 +2,37 @@
 
 from schema import Schema, Optional, And, Or, SchemaError
 from loguru import logger
 
 
 configuration_schema = Schema({
     str: {
-        Optional("train_settings"): {
-            Optional("epochs"): And(int, lambda n: n >= 1),
-            Optional("drop_null"): bool,
-            Optional("row_limit"): And(int, lambda n: n >= 1),
-            Optional("batch_size"): And(int, lambda n: n >= 1),
-            Optional("print_report"): bool,
-            Optional("column_types"): {
-                Optional("categorical"): [str]
-            }
-        },
-        Optional("infer_settings"): {
-            Optional("size"): And(int, lambda n: n >= 1),
-            Optional("run_parallel"): bool,
-            Optional("batch_size"): And(int, lambda n: n >= 1),
-            Optional("random_seed"): And(int, lambda n: n >= 0),
-            Optional("print_report"): bool
-        },
+        Optional("train_settings"): Or(
+            {
+                Optional("epochs"): And(int, lambda n: n >= 1),
+                Optional("drop_null"): bool,
+                Optional("row_limit"): And(int, lambda n: n >= 1),
+                Optional("batch_size"): And(int, lambda n: n >= 1),
+                Optional("print_report"): bool,
+                Optional("column_types"): {
+                    Optional("categorical"): [str]
+                }
+            },
+            None
+        ),
+        Optional("infer_settings"): Or(
+            {
+                Optional("size"): And(int, lambda n: n >= 1),
+                Optional("run_parallel"): bool,
+                Optional("batch_size"): And(int, lambda n: n >= 1),
+                Optional("random_seed"): And(int, lambda n: n >= 0),
+                Optional("print_report"): bool
+            },
+            None
+        ),
         "source": str,
         Optional("keys"): {
             str: {
                 "type": Or("FK", "PK", "UQ"),
                 "columns": [str],
                 Optional("references"): {
                     "table": str,
```

### Comparing `syngen-0.1.2/src/syngen/ml/worker/worker.py` & `syngen-0.1.3/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen/train.py` & `syngen-0.1.3/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.2/src/syngen.egg-info/PKG-INFO` & `syngen-0.1.3/src/syngen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.1.2
+Version: 0.1.3
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
-Metadata-Version: 2.1 Name: syngen Version: 0.1.2 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.1.3 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.1.2/src/syngen.egg-info/SOURCES.txt` & `syngen-0.1.3/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

