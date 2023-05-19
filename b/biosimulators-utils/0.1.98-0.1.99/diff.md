# Comparing `tmp/biosimulators_utils-0.1.98.tar.gz` & `tmp/biosimulators_utils-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biosimulators_utils-0.1.98.tar", last modified: Wed Jul 28 23:37:27 2021, max compression
+gzip compressed data, was "biosimulators_utils-0.1.99.tar", last modified: Thu Jul 29 20:14:41 2021, max compression
```

## Comparing `biosimulators_utils-0.1.98.tar` & `biosimulators_utils-0.1.99.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.390174 biosimulators_utils-0.1.98/
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      403 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5165 2021-07-28 23:37:27.390174 biosimulators_utils-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4173 2021-07-28 23:37:22.000000 biosimulators_utils-0.1.98/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.374174 biosimulators_utils-0.1.98/biosimulators_utils/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17883 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.374174 biosimulators_utils-0.1.98/biosimulators_utils/archive/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/archive/data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/archive/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/archive/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.374174 biosimulators_utils-0.1.98/biosimulators_utils/biosimulations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/biosimulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6999 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/biosimulations/data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/biosimulations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.378174 biosimulators_utils-0.1.98/biosimulators_utils/combine/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/combine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12427 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/combine/data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/combine/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    13953 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/combine/exec.py
--rw-r--r--   0 runner    (1001) docker     (121)    15175 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/combine/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     5512 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/combine/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11747 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/combine/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5924 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3089 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.378174 biosimulators_utils-0.1.98/biosimulators_utils/gh_action/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/gh_action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11804 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/gh_action/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      857 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/gh_action/data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4059 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/image.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.378174 biosimulators_utils-0.1.98/biosimulators_utils/kisao/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/kisao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      988 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/kisao/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.378174 biosimulators_utils-0.1.98/biosimulators_utils/log/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21313 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/log/data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    16030 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/log/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/log/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.378174 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.378174 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/bngl/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/bngl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7014 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/bngl/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2332 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/bngl/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.382174 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/cellml/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/cellml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33542 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/cellml/cellml1.0.rng
--rw-r--r--   0 runner    (1001) docker     (121)    99353 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/cellml/mathml2.rng
--rw-r--r--   0 runner    (1001) docker     (121)     9280 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/cellml/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7466 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/cellml/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.382174 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/lems/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/lems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2886 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/lems/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.382174 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/neuroml/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/neuroml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/neuroml/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.382174 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/sbml/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/sbml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18870 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/sbml/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/sbml/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.382174 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/smoldyn/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/smoldyn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4722 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/smoldyn/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3179 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/model_lang/smoldyn/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.382174 biosimulators_utils-0.1.98/biosimulators_utils/omex_meta/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/omex_meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11234 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/omex_meta/data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    31711 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/omex_meta/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     3899 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/omex_meta/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5417 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/omex_meta/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.382174 biosimulators_utils-0.1.98/biosimulators_utils/report/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2514 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/report/data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    15004 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/report/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/report/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.386174 biosimulators_utils-0.1.98/biosimulators_utils/sedml/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/sedml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    61607 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/sedml/data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/sedml/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    37086 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/sedml/exec.py
--rw-r--r--   0 runner    (1001) docker     (121)    76845 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/sedml/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     4969 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/sedml/math.py
--rw-r--r--   0 runner    (1001) docker     (121)     5772 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/sedml/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    45733 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/sedml/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    69243 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/sedml/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/sedml/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.386174 biosimulators_utils-0.1.98/biosimulators_utils/simulator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6293 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator/data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator/environ.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7445 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator/exec.py
--rw-r--r--   0 runner    (1001) docker     (121)     4474 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     9837 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator/specs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.386174 biosimulators_utils-0.1.98/biosimulators_utils/simulator_registry/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3194 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator_registry/data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3038 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator_registry/process_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator_registry/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     2652 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/simulator_registry/submit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.390174 biosimulators_utils-0.1.98/biosimulators_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11633 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/utils/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.390174 biosimulators_utils-0.1.98/biosimulators_utils/viz/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/viz/data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     7193 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/viz/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     1757 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/viz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.390174 biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.390174 biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/escher/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/escher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16364 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/escher/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    20151 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/escher/template.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.390174 biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/ginml/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/ginml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18577 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/ginml/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    17091 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/ginml/template.json
--rw-r--r--   0 runner    (1001) docker     (121)      914 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/viz/warnings.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.390174 biosimulators_utils-0.1.98/biosimulators_utils/xml/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6654 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/biosimulators_utils/xml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 23:37:27.374174 biosimulators_utils-0.1.98/biosimulators_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5165 2021-07-28 23:37:27.000000 biosimulators_utils-0.1.98/biosimulators_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4509 2021-07-28 23:37:27.000000 biosimulators_utils-0.1.98/biosimulators_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-28 23:37:27.000000 biosimulators_utils-0.1.98/biosimulators_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-07-28 23:37:27.000000 biosimulators_utils-0.1.98/biosimulators_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      636 2021-07-28 23:37:27.000000 biosimulators_utils-0.1.98/biosimulators_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-07-28 23:37:27.000000 biosimulators_utils-0.1.98/biosimulators_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      206 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/requirements.optional.txt
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-07-28 23:37:27.390174 biosimulators_utils-0.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2021-07-28 23:36:06.000000 biosimulators_utils-0.1.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.956853 biosimulators_utils-0.1.99/
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5387 2021-07-29 20:14:41.956853 biosimulators_utils-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4372 2021-07-29 20:14:37.000000 biosimulators_utils-0.1.99/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.940853 biosimulators_utils-0.1.99/biosimulators_utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17883 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.944853 biosimulators_utils-0.1.99/biosimulators_utils/archive/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2379 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/archive/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1693 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/archive/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1329 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/archive/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.944853 biosimulators_utils-0.1.99/biosimulators_utils/biosimulations/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/biosimulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6999 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/biosimulations/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1341 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/biosimulations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.944853 biosimulators_utils-0.1.99/biosimulators_utils/combine/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/combine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12427 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/combine/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/combine/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13953 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/combine/exec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15175 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/combine/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5512 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/combine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11747 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/combine/validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5924 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3089 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.944853 biosimulators_utils-0.1.99/biosimulators_utils/gh_action/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/gh_action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11804 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/gh_action/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      857 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/gh_action/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4059 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/image.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.944853 biosimulators_utils-0.1.99/biosimulators_utils/kisao/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/kisao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/kisao/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.948853 biosimulators_utils-0.1.99/biosimulators_utils/log/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21313 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/log/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16030 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/log/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/log/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.948853 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.948853 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/bngl/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/bngl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7014 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/bngl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2332 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/bngl/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.948853 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/cellml/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/cellml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33542 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/cellml/cellml1.0.rng
+-rw-r--r--   0 runner    (1001) docker     (121)    99353 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/cellml/mathml2.rng
+-rw-r--r--   0 runner    (1001) docker     (121)     9280 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/cellml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7466 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/cellml/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.948853 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/lems/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/lems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2886 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/lems/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.948853 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/neuroml/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/neuroml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1253 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/neuroml/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.948853 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/sbml/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/sbml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18870 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/sbml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1655 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/sbml/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.948853 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/smoldyn/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/smoldyn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4722 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/smoldyn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3179 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/model_lang/smoldyn/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.948853 biosimulators_utils-0.1.99/biosimulators_utils/omex_meta/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/omex_meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11234 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/omex_meta/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31711 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/omex_meta/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3899 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/omex_meta/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5417 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/omex_meta/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.948853 biosimulators_utils-0.1.99/biosimulators_utils/report/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2514 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/report/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15004 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/report/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1382 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/report/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.952853 biosimulators_utils-0.1.99/biosimulators_utils/sedml/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/sedml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    61607 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/sedml/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/sedml/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37086 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/sedml/exec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    76845 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/sedml/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4969 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/sedml/math.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5772 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/sedml/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45733 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/sedml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    69243 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/sedml/validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1949 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/sedml/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.952853 biosimulators_utils-0.1.99/biosimulators_utils/simulator/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6293 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator/environ.py
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7445 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator/exec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4474 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9837 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator/specs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1356 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.952853 biosimulators_utils-0.1.99/biosimulators_utils/simulator_registry/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3194 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator_registry/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3038 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator_registry/process_submission.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1192 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator_registry/query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2652 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/simulator_registry/submit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.952853 biosimulators_utils-0.1.99/biosimulators_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11633 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/utils/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1713 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.952853 biosimulators_utils-0.1.99/biosimulators_utils/viz/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/viz/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7193 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/viz/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1757 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/viz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.952853 biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.952853 biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/escher/
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/escher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16364 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/escher/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20151 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/escher/template.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.956853 biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/ginml/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/ginml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18577 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/ginml/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17091 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/ginml/template.json
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      413 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/viz/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.956853 biosimulators_utils-0.1.99/biosimulators_utils/xml/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6654 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/biosimulators_utils/xml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-29 20:14:41.944853 biosimulators_utils-0.1.99/biosimulators_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5387 2021-07-29 20:14:41.000000 biosimulators_utils-0.1.99/biosimulators_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4509 2021-07-29 20:14:41.000000 biosimulators_utils-0.1.99/biosimulators_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-29 20:14:41.000000 biosimulators_utils-0.1.99/biosimulators_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-07-29 20:14:41.000000 biosimulators_utils-0.1.99/biosimulators_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2021-07-29 20:14:41.000000 biosimulators_utils-0.1.99/biosimulators_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-07-29 20:14:41.000000 biosimulators_utils-0.1.99/biosimulators_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/requirements.optional.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-07-29 20:14:41.956853 biosimulators_utils-0.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2255 2021-07-29 20:13:32.000000 biosimulators_utils-0.1.99/setup.py
```

### Comparing `biosimulators_utils-0.1.98/LICENSE` & `biosimulators_utils-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/PKG-INFO` & `biosimulators_utils-0.1.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosimulators_utils
-Version: 0.1.98
+Version: 0.1.99
 Summary: Command-line program and library for reading, writing, validating and executing modeling projects (COMBINE/OMEX archives with SED-ML files).
 Home-page: https://github.com/biosimulators/Biosimulators_utils
 Author: Center for Reproducible Biomedical Modeling
 Author-email: info@biosimulators.org
 License: MIT
 Download-URL: https://github.com/biosimulators/Biosimulators_utils
 Keywords: systems biology modeling simulation
@@ -15,14 +15,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Provides-Extra: bngl
 Provides-Extra: cellml
 Provides-Extra: lems
 Provides-Extra: neuroml
 Provides-Extra: sbml
 Provides-Extra: smoldyn
+Provides-Extra: escher
 Provides-Extra: containers
 Provides-Extra: logging
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
@@ -109,14 +110,22 @@
 To use BioSimulators utils to validate SBML models, install
 BioSimulators utils with the ``smoldyn`` option:
 
 ::
 
    pip install biosimulators-utils[smoldyn]
 
+To use BioSimulators utils to convert Escher metabolic maps to Vega flux
+data visualizations, install BioSimulators utils with the ``escher``
+option:
+
+::
+
+   pip install biosimulators-utils[escher]
+
 To use BioSimulators utils to execute containerized simulation tools,
 install BioSimulators utils with the ``containers`` option:
 
 ::
 
    pip install biosimulators-utils[containers]
```

### Comparing `biosimulators_utils-0.1.98/README.rst` & `biosimulators_utils-0.1.99/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -81,14 +81,22 @@
 To use BioSimulators utils to validate SBML models, install
 BioSimulators utils with the ``smoldyn`` option:
 
 ::
 
    pip install biosimulators-utils[smoldyn]
 
+To use BioSimulators utils to convert Escher metabolic maps to Vega flux
+data visualizations, install BioSimulators utils with the ``escher``
+option:
+
+::
+
+   pip install biosimulators-utils[escher]
+
 To use BioSimulators utils to execute containerized simulation tools,
 install BioSimulators utils with the ``containers`` option:
 
 ::
 
    pip install biosimulators-utils[containers]
```

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/__main__.py` & `biosimulators_utils-0.1.99/biosimulators_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/archive/data_model.py` & `biosimulators_utils-0.1.99/biosimulators_utils/archive/data_model.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/archive/io.py` & `biosimulators_utils-0.1.99/biosimulators_utils/archive/io.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/archive/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/archive/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/biosimulations/data_model.py` & `biosimulators_utils-0.1.99/biosimulators_utils/biosimulations/data_model.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/biosimulations/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/biosimulations/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/combine/data_model.py` & `biosimulators_utils-0.1.99/biosimulators_utils/combine/data_model.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/combine/exceptions.py` & `biosimulators_utils-0.1.99/biosimulators_utils/combine/exceptions.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/combine/exec.py` & `biosimulators_utils-0.1.99/biosimulators_utils/combine/exec.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/combine/io.py` & `biosimulators_utils-0.1.99/biosimulators_utils/combine/io.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/combine/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/combine/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/combine/validation.py` & `biosimulators_utils-0.1.99/biosimulators_utils/combine/validation.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/config.py` & `biosimulators_utils-0.1.99/biosimulators_utils/config.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/data_model.py` & `biosimulators_utils-0.1.99/biosimulators_utils/data_model.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/gh_action/core.py` & `biosimulators_utils-0.1.99/biosimulators_utils/gh_action/core.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/gh_action/data_model.py` & `biosimulators_utils-0.1.99/biosimulators_utils/gh_action/data_model.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/image.py` & `biosimulators_utils-0.1.99/biosimulators_utils/image.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/kisao/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/kisao/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/log/data_model.py` & `biosimulators_utils-0.1.99/biosimulators_utils/log/data_model.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/log/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/log/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/model_lang/bngl/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/model_lang/bngl/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/model_lang/bngl/validation.py` & `biosimulators_utils-0.1.99/biosimulators_utils/model_lang/bngl/validation.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/model_lang/cellml/cellml1.0.rng` & `biosimulators_utils-0.1.99/biosimulators_utils/model_lang/cellml/cellml1.0.rng`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/model_lang/cellml/mathml2.rng` & `biosimulators_utils-0.1.99/biosimulators_utils/model_lang/cellml/mathml2.rng`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/model_lang/cellml/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/model_lang/cellml/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/model_lang/cellml/validation.py` & `biosimulators_utils-0.1.99/biosimulators_utils/model_lang/cellml/validation.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/model_lang/lems/validation.py` & `biosimulators_utils-0.1.99/biosimulators_utils/model_lang/lems/validation.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/model_lang/neuroml/validation.py` & `biosimulators_utils-0.1.99/biosimulators_utils/model_lang/neuroml/validation.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/model_lang/sbml/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/model_lang/sbml/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/model_lang/sbml/validation.py` & `biosimulators_utils-0.1.99/biosimulators_utils/model_lang/sbml/validation.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/model_lang/smoldyn/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/model_lang/smoldyn/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/model_lang/smoldyn/validation.py` & `biosimulators_utils-0.1.99/biosimulators_utils/model_lang/smoldyn/validation.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/omex_meta/data_model.py` & `biosimulators_utils-0.1.99/biosimulators_utils/omex_meta/data_model.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/omex_meta/io.py` & `biosimulators_utils-0.1.99/biosimulators_utils/omex_meta/io.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/omex_meta/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/omex_meta/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/omex_meta/validation.py` & `biosimulators_utils-0.1.99/biosimulators_utils/omex_meta/validation.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/report/data_model.py` & `biosimulators_utils-0.1.99/biosimulators_utils/report/data_model.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/report/io.py` & `biosimulators_utils-0.1.99/biosimulators_utils/report/io.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/report/warnings.py` & `biosimulators_utils-0.1.99/biosimulators_utils/report/warnings.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/sedml/data_model.py` & `biosimulators_utils-0.1.99/biosimulators_utils/sedml/data_model.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/sedml/exceptions.py` & `biosimulators_utils-0.1.99/biosimulators_utils/sedml/exceptions.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/sedml/exec.py` & `biosimulators_utils-0.1.99/biosimulators_utils/sedml/exec.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/sedml/io.py` & `biosimulators_utils-0.1.99/biosimulators_utils/sedml/io.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/sedml/math.py` & `biosimulators_utils-0.1.99/biosimulators_utils/sedml/math.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/sedml/model_utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/sedml/model_utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/sedml/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/sedml/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/sedml/validation.py` & `biosimulators_utils-0.1.99/biosimulators_utils/sedml/validation.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/sedml/warnings.py` & `biosimulators_utils-0.1.99/biosimulators_utils/sedml/warnings.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/simulator/cli.py` & `biosimulators_utils-0.1.99/biosimulators_utils/simulator/cli.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/simulator/data_model.py` & `biosimulators_utils-0.1.99/biosimulators_utils/simulator/data_model.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/simulator/environ.py` & `biosimulators_utils-0.1.99/biosimulators_utils/simulator/environ.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/simulator/exec.py` & `biosimulators_utils-0.1.99/biosimulators_utils/simulator/exec.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/simulator/io.py` & `biosimulators_utils-0.1.99/biosimulators_utils/simulator/io.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/simulator/specs.py` & `biosimulators_utils-0.1.99/biosimulators_utils/simulator/specs.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/simulator/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/simulator/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/simulator_registry/data_model.py` & `biosimulators_utils-0.1.99/biosimulators_utils/simulator_registry/data_model.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/simulator_registry/process_submission.py` & `biosimulators_utils-0.1.99/biosimulators_utils/simulator_registry/process_submission.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/simulator_registry/query.py` & `biosimulators_utils-0.1.99/biosimulators_utils/simulator_registry/query.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/simulator_registry/submit.py` & `biosimulators_utils-0.1.99/biosimulators_utils/simulator_registry/submit.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/utils/core.py` & `biosimulators_utils-0.1.99/biosimulators_utils/utils/core.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/utils/logging.py` & `biosimulators_utils-0.1.99/biosimulators_utils/utils/logging.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/viz/io.py` & `biosimulators_utils-0.1.99/biosimulators_utils/viz/io.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/viz/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/viz/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/escher/core.py` & `biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/escher/core.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/escher/template.json` & `biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/escher/template.json`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/ginml/core.py` & `biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/ginml/core.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/ginml/template.json` & `biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/ginml/template.json`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/viz/vega/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/viz/vega/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/warnings.py` & `biosimulators_utils-0.1.99/biosimulators_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils/xml/utils.py` & `biosimulators_utils-0.1.99/biosimulators_utils/xml/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils.egg-info/PKG-INFO` & `biosimulators_utils-0.1.99/biosimulators_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosimulators-utils
-Version: 0.1.98
+Version: 0.1.99
 Summary: Command-line program and library for reading, writing, validating and executing modeling projects (COMBINE/OMEX archives with SED-ML files).
 Home-page: https://github.com/biosimulators/Biosimulators_utils
 Author: Center for Reproducible Biomedical Modeling
 Author-email: info@biosimulators.org
 License: MIT
 Download-URL: https://github.com/biosimulators/Biosimulators_utils
 Keywords: systems biology modeling simulation
@@ -15,14 +15,15 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Provides-Extra: bngl
 Provides-Extra: cellml
 Provides-Extra: lems
 Provides-Extra: neuroml
 Provides-Extra: sbml
 Provides-Extra: smoldyn
+Provides-Extra: escher
 Provides-Extra: containers
 Provides-Extra: logging
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
@@ -109,14 +110,22 @@
 To use BioSimulators utils to validate SBML models, install
 BioSimulators utils with the ``smoldyn`` option:
 
 ::
 
    pip install biosimulators-utils[smoldyn]
 
+To use BioSimulators utils to convert Escher metabolic maps to Vega flux
+data visualizations, install BioSimulators utils with the ``escher``
+option:
+
+::
+
+   pip install biosimulators-utils[escher]
+
 To use BioSimulators utils to execute containerized simulation tools,
 install BioSimulators utils with the ``containers`` option:
 
 ::
 
    pip install biosimulators-utils[containers]
```

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils.egg-info/SOURCES.txt` & `biosimulators_utils-0.1.99/biosimulators_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biosimulators_utils-0.1.98/biosimulators_utils.egg-info/requires.txt` & `biosimulators_utils-0.1.99/biosimulators_utils.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 appdirs
-bezier
 cement
 evalidate
 h5py
 kisao>=2.20
 lxml
 matplotlib
 mpmath
@@ -22,14 +21,15 @@
 requests
 simplejson
 termcolor
 validators
 yamldown
 
 [all]
+bezier
 bionetgen<=0.3.1,>=0.3.1
 capturer
 docker>=4.4
 jsonschema
 libcellml
 libneuroml
 pint
@@ -45,14 +45,17 @@
 libcellml
 
 [containers]
 docker>=4.4
 
 [docs]
 
+[escher]
+bezier
+
 [lems]
 pint
 pylems
 pyneuroml
 
 [logging]
 capturer
```

### Comparing `biosimulators_utils-0.1.98/setup.py` & `biosimulators_utils-0.1.99/setup.py`

 * *Files identical despite different names*

