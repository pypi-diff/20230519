# Comparing `tmp/cbcflow-0.2.2.tar.gz` & `tmp/cbcflow-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcflow-0.2.2.tar", last modified: Wed May 10 10:17:23 2023, max compression
+gzip compressed data, was "cbcflow-0.2.3.tar", last modified: Fri May 19 19:22:43 2023, max compression
```

## Comparing `cbcflow-0.2.2.tar` & `cbcflow-0.2.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.972633 cbcflow-0.2.2/
--rw-r--r--   0 greg      (1000) greg      (1000)       37 2023-04-21 10:34:59.000000 cbcflow-0.2.2/.gitattributes
--rw-r--r--   0 greg      (1000) greg      (1000)      217 2023-04-21 10:34:59.000000 cbcflow-0.2.2/.gitignore
--rw-r--r--   0 greg      (1000) greg      (1000)     1533 2023-04-21 10:34:59.000000 cbcflow-0.2.2/.gitlab-ci.yml
--rw-r--r--   0 greg      (1000) greg      (1000)      873 2023-04-21 10:34:59.000000 cbcflow-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 greg      (1000) greg      (1000)     1078 2023-05-10 10:16:22.000000 cbcflow-0.2.2/CHANGELOG.md
--rw-r--r--   0 greg      (1000) greg      (1000)     1084 2023-04-21 10:34:59.000000 cbcflow-0.2.2/LICENSE.md
--rw-r--r--   0 greg      (1000) greg      (1000)      123 2023-04-21 10:34:59.000000 cbcflow-0.2.2/MANIFEST.in
--rw-r--r--   0 greg      (1000) greg      (1000)     3027 2023-05-10 10:17:23.972633 cbcflow-0.2.2/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     2390 2023-04-21 14:02:43.000000 cbcflow-0.2.2/README.md
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/docs/
--rw-r--r--   0 greg      (1000) greg      (1000)      613 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/Makefile
--rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/requirements.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/docs/source/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/docs/source/_templates/
--rw-r--r--   0 greg      (1000) greg      (1000)      662 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1408 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1158 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/actionitems.rst
--rw-r--r--   0 greg      (1000) greg      (1000)      690 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/adding-to-the-schema.rst
--rw-r--r--   0 greg      (1000) greg      (1000)       39 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/asimov.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4404 2023-05-10 08:29:20.000000 cbcflow-0.2.2/docs/source/cbcflow-git-merging.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     2616 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/conf.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1770 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/configuration.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1444 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/development-setup.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/docs/source/example_mini_schema/
--rw-r--r--   0 greg      (1000) greg      (1000)     2924 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/example_mini_schema/example.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     6391 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/example_mini_schema/schema_doc.css
--rw-r--r--   0 greg      (1000) greg      (1000)    27212 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/example_mini_schema/schema_doc.html
--rw-r--r--   0 greg      (1000) greg      (1000)      984 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/example_mini_schema/schema_doc.min.js
--rw-r--r--   0 greg      (1000) greg      (1000)      458 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/gwosc.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1255 2023-05-10 08:29:20.000000 cbcflow-0.2.2/docs/source/index.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     2799 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/docs/source/libraries_images/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/docs/source/libraries_images/.ipynb_checkpoints/
--rw-r--r--   0 greg      (1000) greg      (1000)    72683 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
--rw-r--r--   0 greg      (1000) greg      (1000)     8993 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_1.png
--rw-r--r--   0 greg      (1000) greg      (1000)    15966 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_2.png
--rw-r--r--   0 greg      (1000) greg      (1000)    38016 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_3.png
--rw-r--r--   0 greg      (1000) greg      (1000)    51488 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_4.png
--rw-r--r--   0 greg      (1000) greg      (1000)    41435 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_5.png
--rw-r--r--   0 greg      (1000) greg      (1000)    54941 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_6.png
--rw-r--r--   0 greg      (1000) greg      (1000)    67345 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_7.png
--rw-r--r--   0 greg      (1000) greg      (1000)    72180 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_8.png
--rw-r--r--   0 greg      (1000) greg      (1000)    10255 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/library-index-labelling.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1352 2023-05-10 10:03:05.000000 cbcflow-0.2.2/docs/source/library-indices.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     3620 2023-05-10 08:29:20.000000 cbcflow-0.2.2/docs/source/library-setup-from-scratch.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1287 2023-05-10 08:29:20.000000 cbcflow-0.2.2/docs/source/local-library-copy-setup.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1782 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/monitor-usage.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4809 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/reading-the-schema.rst
--rw-r--r--   0 greg      (1000) greg      (1000)      106 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/schema-visualization.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    15476 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/updating-metadata-from-the-command-line.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    12152 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/updating-metadata-with-the-python-api.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4916 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/what-is-metadata.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/examples/
--rw-r--r--   0 greg      (1000) greg      (1000)     7368 2023-04-21 10:34:59.000000 cbcflow-0.2.2/examples/initial_example.md
--rw-r--r--   0 greg      (1000) greg      (1000)      856 2023-04-21 14:02:43.000000 cbcflow-0.2.2/pyproject.toml
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/schema/
--rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-21 10:34:59.000000 cbcflow-0.2.2/schema/cbc-meta-data-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)    88906 2023-04-24 13:44:33.000000 cbcflow-0.2.2/schema/cbc-meta-data-v2.schema
--rwxr-xr-x   0 greg      (1000) greg      (1000)     1766 2023-05-10 10:03:05.000000 cbcflow-0.2.2/schema/index-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     1635 2023-05-10 10:17:23.972633 cbcflow-0.2.2/setup.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)      567 2023-04-21 10:34:59.000000 cbcflow-0.2.2/setup.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.952633 cbcflow-0.2.2/src/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/src/cbcflow/
--rw-r--r--   0 greg      (1000) greg      (1000)     1462 2023-04-24 14:06:13.000000 cbcflow-0.2.2/src/cbcflow/__init__.py
--rw-r--r--   0 greg      (1000) greg      (1000)      160 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow/_version.py
--rw-r--r--   0 greg      (1000) greg      (1000)    14041 2023-05-10 08:29:20.000000 cbcflow-0.2.2/src/cbcflow/asimov.py
--rwxr-xr-x   0 greg      (1000) greg      (1000)     9343 2023-05-10 10:03:05.000000 cbcflow-0.2.2/src/cbcflow/cbcflow.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1330 2023-04-24 14:06:13.000000 cbcflow-0.2.2/src/cbcflow/configuration.py
--rw-r--r--   0 greg      (1000) greg      (1000)    37155 2023-05-10 10:15:43.000000 cbcflow-0.2.2/src/cbcflow/database.py
--rw-r--r--   0 greg      (1000) greg      (1000)    14125 2023-05-10 10:03:05.000000 cbcflow-0.2.2/src/cbcflow/gracedb.py
--rw-r--r--   0 greg      (1000) greg      (1000)    14413 2023-05-10 10:03:05.000000 cbcflow-0.2.2/src/cbcflow/metadata.py
--rw-r--r--   0 greg      (1000) greg      (1000)     6270 2023-05-10 08:29:20.000000 cbcflow-0.2.2/src/cbcflow/monitor.py
--rw-r--r--   0 greg      (1000) greg      (1000)     5096 2023-05-10 10:03:05.000000 cbcflow-0.2.2/src/cbcflow/online_pe.py
--rw-r--r--   0 greg      (1000) greg      (1000)     8049 2023-05-10 08:29:20.000000 cbcflow-0.2.2/src/cbcflow/parser.py
--rw-r--r--   0 greg      (1000) greg      (1000)    35849 2023-05-10 10:03:05.000000 cbcflow-0.2.2/src/cbcflow/process.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/src/cbcflow/schema/
--rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow/schema/cbc-meta-data-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)    88906 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow/schema/cbc-meta-data-v2.schema
--rwxr-xr-x   0 greg      (1000) greg      (1000)     1766 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow/schema/index-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     2779 2023-04-24 14:06:13.000000 cbcflow-0.2.2/src/cbcflow/schema.py
--rw-r--r--   0 greg      (1000) greg      (1000)     7294 2023-05-10 08:29:20.000000 cbcflow-0.2.2/src/cbcflow/utils.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/src/cbcflow.egg-info/
--rw-r--r--   0 greg      (1000) greg      (1000)     3027 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow.egg-info/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     3290 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow.egg-info/SOURCES.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow.egg-info/dependency_links.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      599 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow.egg-info/entry_points.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      130 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow.egg-info/requires.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        8 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow.egg-info/top_level.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/tests/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.972633 cbcflow-0.2.2/tests/files_for_testing/
--rw-r--r--   0 greg      (1000) greg      (1000)    26759 2023-04-21 10:34:59.000000 cbcflow-0.2.2/tests/files_for_testing/cbc-meta-data-example.json
--rw-r--r--   0 greg      (1000) greg      (1000)     5972 2023-05-10 08:29:20.000000 cbcflow-0.2.2/tests/files_for_testing/merge_test.json
--rw-r--r--   0 greg      (1000) greg      (1000)       56 2023-04-21 10:34:59.000000 cbcflow-0.2.2/tests/files_for_testing/test-file-for-linking-1.txt
--rw-r--r--   0 greg      (1000) greg      (1000)       86 2023-04-21 10:34:59.000000 cbcflow-0.2.2/tests/files_for_testing/test-file-for-linking-2.txt
--rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-05-10 08:29:20.000000 cbcflow-0.2.2/tests/files_for_testing/test-file-for-linking-3.txt
--rw-r--r--   0 greg      (1000) greg      (1000)     3091 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/files_for_testing/update_json_1.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1221 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/files_for_testing/update_json_2.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1626 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/files_for_testing/update_yaml_1.yaml
--rw-r--r--   0 greg      (1000) greg      (1000)      571 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/files_for_testing/update_yaml_2.yaml
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.972633 cbcflow-0.2.2/tests/library_for_testing/
--rw-r--r--   0 greg      (1000) greg      (1000)     5338 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230227hp-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     4289 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230331e-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     4275 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230401h-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     2416 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230402dv-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     3353 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230403ae-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     5238 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230404hb-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     3256 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230404jc-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)      193 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/library.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)       90 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/testing-library-index.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1838 2023-05-10 10:03:05.000000 cbcflow-0.2.2/tests/test_database.py
--rw-r--r--   0 greg      (1000) greg      (1000)    38496 2023-05-10 08:29:20.000000 cbcflow-0.2.2/tests/test_merging.py
--rw-r--r--   0 greg      (1000) greg      (1000)    23545 2023-05-10 08:29:20.000000 cbcflow-0.2.2/tests/test_metadata.py
--rw-r--r--   0 greg      (1000) greg      (1000)      755 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/test_schema.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.095388 cbcflow-0.2.3/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       37 2022-09-02 21:51:00.000000 cbcflow-0.2.3/.gitattributes
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      217 2023-04-17 16:08:35.000000 cbcflow-0.2.3/.gitignore
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1533 2023-04-17 16:08:35.000000 cbcflow-0.2.3/.gitlab-ci.yml
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      873 2023-03-15 15:11:03.000000 cbcflow-0.2.3/.pre-commit-config.yaml
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1078 2023-05-10 19:01:56.000000 cbcflow-0.2.3/CHANGELOG.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1084 2023-04-17 16:08:35.000000 cbcflow-0.2.3/LICENSE.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      123 2023-04-17 16:08:35.000000 cbcflow-0.2.3/MANIFEST.in
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3027 2023-05-19 19:22:43.095388 cbcflow-0.2.3/PKG-INFO
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2390 2023-04-21 18:28:00.000000 cbcflow-0.2.3/README.md
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.703384 cbcflow-0.2.3/docs/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      613 2023-04-07 19:31:48.000000 cbcflow-0.2.3/docs/Makefile
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2022-09-02 21:51:00.000000 cbcflow-0.2.3/docs/requirements.txt
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.793385 cbcflow-0.2.3/docs/source/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.797385 cbcflow-0.2.3/docs/source/_templates/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      662 2023-04-07 19:31:48.000000 cbcflow-0.2.3/docs/source/_templates/custom-class-template.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1408 2023-04-07 19:31:48.000000 cbcflow-0.2.3/docs/source/_templates/custom-module-template.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1158 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/actionitems.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      690 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/adding-to-the-schema.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       39 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/asimov.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4404 2023-05-05 16:21:05.000000 cbcflow-0.2.3/docs/source/cbcflow-git-merging.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2616 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/conf.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1770 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/configuration.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1444 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/development-setup.rst
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.806385 cbcflow-0.2.3/docs/source/example_mini_schema/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2924 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/example_mini_schema/example.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6391 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/example_mini_schema/schema_doc.css
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    27212 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/example_mini_schema/schema_doc.html
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      984 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/example_mini_schema/schema_doc.min.js
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      458 2023-04-07 19:31:48.000000 cbcflow-0.2.3/docs/source/gwosc.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1255 2023-05-05 16:21:05.000000 cbcflow-0.2.3/docs/source/index.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2799 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries.rst
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.897386 cbcflow-0.2.3/docs/source/libraries_images/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.977387 cbcflow-0.2.3/docs/source/libraries_images/.ipynb_checkpoints/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72683 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     8993 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_1.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15966 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_2.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38016 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_3.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    51488 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_4.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    41435 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_5.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    54941 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_6.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    67345 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_7.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72180 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/libraries_images/part_8.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    10255 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/library-index-labelling.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1352 2023-05-10 19:01:56.000000 cbcflow-0.2.3/docs/source/library-indices.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3620 2023-05-09 00:07:03.000000 cbcflow-0.2.3/docs/source/library-setup-from-scratch.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1287 2023-05-05 16:21:05.000000 cbcflow-0.2.3/docs/source/local-library-copy-setup.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1782 2023-04-07 19:31:48.000000 cbcflow-0.2.3/docs/source/monitor-usage.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4809 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/reading-the-schema.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      106 2023-04-07 19:31:49.000000 cbcflow-0.2.3/docs/source/schema-visualization.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15476 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/updating-metadata-from-the-command-line.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    12152 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/updating-metadata-with-the-python-api.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4916 2023-04-17 16:08:35.000000 cbcflow-0.2.3/docs/source/what-is-metadata.rst
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.999387 cbcflow-0.2.3/examples/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     7368 2022-09-29 19:29:06.000000 cbcflow-0.2.3/examples/initial_example.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      856 2023-04-21 18:28:00.000000 cbcflow-0.2.3/pyproject.toml
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.005387 cbcflow-0.2.3/schema/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2023-03-16 15:08:33.000000 cbcflow-0.2.3/schema/cbc-meta-data-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2023-04-25 20:47:59.000000 cbcflow-0.2.3/schema/cbc-meta-data-v2.schema
+-rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2023-05-10 19:01:56.000000 cbcflow-0.2.3/schema/index-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1635 2023-05-19 19:22:43.097388 cbcflow-0.2.3/setup.cfg
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      567 2023-04-08 00:03:25.000000 cbcflow-0.2.3/setup.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:42.654384 cbcflow-0.2.3/src/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.029388 cbcflow-0.2.3/src/cbcflow/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1462 2023-04-25 20:47:59.000000 cbcflow-0.2.3/src/cbcflow/__init__.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      160 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow/_version.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    14160 2023-05-19 18:18:46.000000 cbcflow-0.2.3/src/cbcflow/asimov.py
+-rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     9343 2023-05-10 19:01:56.000000 cbcflow-0.2.3/src/cbcflow/cbcflow.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1330 2023-04-25 20:47:59.000000 cbcflow-0.2.3/src/cbcflow/configuration.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    39799 2023-05-19 19:17:47.000000 cbcflow-0.2.3/src/cbcflow/database.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    14407 2023-05-19 19:17:47.000000 cbcflow-0.2.3/src/cbcflow/gracedb.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    14413 2023-05-10 19:01:56.000000 cbcflow-0.2.3/src/cbcflow/metadata.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6270 2023-05-10 19:01:56.000000 cbcflow-0.2.3/src/cbcflow/monitor.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5096 2023-05-10 19:01:56.000000 cbcflow-0.2.3/src/cbcflow/online_pe.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     9016 2023-05-16 15:26:32.000000 cbcflow-0.2.3/src/cbcflow/parser.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    35849 2023-05-10 19:01:56.000000 cbcflow-0.2.3/src/cbcflow/process.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.041388 cbcflow-0.2.3/src/cbcflow/schema/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow/schema/cbc-meta-data-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow/schema/cbc-meta-data-v2.schema
+-rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow/schema/index-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2779 2023-04-25 20:47:59.000000 cbcflow-0.2.3/src/cbcflow/schema.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     7294 2023-05-10 19:01:56.000000 cbcflow-0.2.3/src/cbcflow/utils.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.036388 cbcflow-0.2.3/src/cbcflow.egg-info/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3027 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow.egg-info/PKG-INFO
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3290 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        1 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      599 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow.egg-info/entry_points.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      130 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow.egg-info/requires.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        8 2023-05-19 19:22:42.000000 cbcflow-0.2.3/src/cbcflow.egg-info/top_level.txt
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.048388 cbcflow-0.2.3/tests/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.077388 cbcflow-0.2.3/tests/files_for_testing/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    26759 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/cbc-meta-data-example.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5972 2023-05-05 16:21:05.000000 cbcflow-0.2.3/tests/files_for_testing/merge_test.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       56 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/test-file-for-linking-1.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       86 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/test-file-for-linking-2.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2023-05-05 16:21:05.000000 cbcflow-0.2.3/tests/files_for_testing/test-file-for-linking-3.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3091 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/update_json_1.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1221 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/update_json_2.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1626 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/update_yaml_1.yaml
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      571 2023-04-07 19:31:49.000000 cbcflow-0.2.3/tests/files_for_testing/update_yaml_2.yaml
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-05-19 19:22:43.094388 cbcflow-0.2.3/tests/library_for_testing/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5338 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230227hp-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4289 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230331e-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4275 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230401h-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2416 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230402dv-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3353 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230403ae-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5238 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230404hb-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3256 2023-04-08 00:03:25.000000 cbcflow-0.2.3/tests/library_for_testing/S230404jc-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      193 2023-04-07 19:31:48.000000 cbcflow-0.2.3/tests/library_for_testing/library.cfg
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       90 2023-04-07 19:31:48.000000 cbcflow-0.2.3/tests/library_for_testing/testing-library-index.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1838 2023-05-10 19:01:56.000000 cbcflow-0.2.3/tests/test_database.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38496 2023-05-05 16:21:05.000000 cbcflow-0.2.3/tests/test_merging.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    23545 2023-05-09 00:07:03.000000 cbcflow-0.2.3/tests/test_metadata.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      755 2023-03-27 22:27:03.000000 cbcflow-0.2.3/tests/test_schema.py
```

### Comparing `cbcflow-0.2.2/.gitlab-ci.yml` & `cbcflow-0.2.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/.pre-commit-config.yaml` & `cbcflow-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/CHANGELOG.md` & `cbcflow-0.2.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/LICENSE.md` & `cbcflow-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/PKG-INFO` & `cbcflow-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/cbcflow
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/cbcflow
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/cbcflow/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.2.2/README.md` & `cbcflow-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/Makefile` & `cbcflow-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/_templates/custom-class-template.rst` & `cbcflow-0.2.3/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/_templates/custom-module-template.rst` & `cbcflow-0.2.3/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/actionitems.rst` & `cbcflow-0.2.3/docs/source/actionitems.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/adding-to-the-schema.rst` & `cbcflow-0.2.3/docs/source/adding-to-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/cbcflow-git-merging.rst` & `cbcflow-0.2.3/docs/source/cbcflow-git-merging.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/conf.py` & `cbcflow-0.2.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/configuration.rst` & `cbcflow-0.2.3/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/development-setup.rst` & `cbcflow-0.2.3/docs/source/development-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/example_mini_schema/example.schema` & `cbcflow-0.2.3/docs/source/example_mini_schema/example.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/example_mini_schema/schema_doc.css` & `cbcflow-0.2.3/docs/source/example_mini_schema/schema_doc.css`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/example_mini_schema/schema_doc.html` & `cbcflow-0.2.3/docs/source/example_mini_schema/schema_doc.html`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/example_mini_schema/schema_doc.min.js` & `cbcflow-0.2.3/docs/source/example_mini_schema/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/index.rst` & `cbcflow-0.2.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/libraries.rst` & `cbcflow-0.2.3/docs/source/libraries.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png` & `cbcflow-0.2.3/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/libraries_images/part_1.png` & `cbcflow-0.2.3/docs/source/libraries_images/part_1.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/libraries_images/part_2.png` & `cbcflow-0.2.3/docs/source/libraries_images/part_2.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/libraries_images/part_3.png` & `cbcflow-0.2.3/docs/source/libraries_images/part_3.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/libraries_images/part_4.png` & `cbcflow-0.2.3/docs/source/libraries_images/part_4.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/libraries_images/part_5.png` & `cbcflow-0.2.3/docs/source/libraries_images/part_5.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/libraries_images/part_6.png` & `cbcflow-0.2.3/docs/source/libraries_images/part_6.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/libraries_images/part_7.png` & `cbcflow-0.2.3/docs/source/libraries_images/part_7.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/libraries_images/part_8.png` & `cbcflow-0.2.3/docs/source/libraries_images/part_8.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/library-index-labelling.rst` & `cbcflow-0.2.3/docs/source/library-index-labelling.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/library-indices.rst` & `cbcflow-0.2.3/docs/source/library-indices.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/library-setup-from-scratch.rst` & `cbcflow-0.2.3/docs/source/library-setup-from-scratch.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/local-library-copy-setup.rst` & `cbcflow-0.2.3/docs/source/local-library-copy-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/monitor-usage.rst` & `cbcflow-0.2.3/docs/source/monitor-usage.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/reading-the-schema.rst` & `cbcflow-0.2.3/docs/source/reading-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/updating-metadata-from-the-command-line.rst` & `cbcflow-0.2.3/docs/source/updating-metadata-from-the-command-line.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/updating-metadata-with-the-python-api.rst` & `cbcflow-0.2.3/docs/source/updating-metadata-with-the-python-api.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/docs/source/what-is-metadata.rst` & `cbcflow-0.2.3/docs/source/what-is-metadata.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/examples/initial_example.md` & `cbcflow-0.2.3/examples/initial_example.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/pyproject.toml` & `cbcflow-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/schema/cbc-meta-data-v1.schema` & `cbcflow-0.2.3/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/schema/cbc-meta-data-v2.schema` & `cbcflow-0.2.3/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/schema/index-v1.schema` & `cbcflow-0.2.3/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/setup.cfg` & `cbcflow-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/setup.py` & `cbcflow-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow/__init__.py` & `cbcflow-0.2.3/src/cbcflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow/asimov.py` & `cbcflow-0.2.3/src/cbcflow/asimov.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,16 @@
                             analysis.pipeline.production.name,
                             analysis.pipeline.category,
                         )[0]
                         analysis_output["ConfigFile"] = {}
                         analysis_output["ConfigFile"]["Path"] = ini
                     except IndexError:
                         logger.warning("Could not find ini file for this analysis")
-                    analysis_output["Notes"] = [analysis.comment]
+                    if analysis.comment is not None:
+                        analysis_output["Notes"] = [analysis.comment]
                     if analysis.review.status:
                         if analysis.review.status.lower() == "approved":
                             analysis_output["ReviewStatus"] = "pass"
                         elif analysis.review.status.lower() == "rejected":
                             analysis_output["ReviewStatus"] = "fail"
                         elif analysis.review.status.lower() == "deprecated":
                             analysis_output["Deprecated"] = True
@@ -151,15 +152,15 @@
                                     "Could not get results from RIFT run - to many or too few outputs"
                                 )
 
                     if analysis.status == "uploaded":
                         # Next, try to get PESummary information
                         pesummary_pages_dir = os.path.join(
                             config.get("general", "webroot"),
-                            analysis.subject.name,
+                            analysis.event.name,
                             analysis.name,
                             "pesummary",
                         )
                         sample_h5s = glob.glob(f"{pesummary_pages_dir}/samples/*.h5")
                         if len(sample_h5s) == 1:
                             # If there is only one samples h5, we're good!
                             # This *should* be true, and it should normally be called "posterior_samples.h5"
@@ -226,24 +227,25 @@
         max_f = quality["maximum frequency"] = {}
         min_f = quality["minimum frequency"] = {}
 
         # Data settings
         data = {}
         channels = data["channels"] = {}
         frame_types = data["frame types"] = {}
-        data["segment length"] = detchar["RecommendedDuration"]
         # NOTE there are also detector specific quantities "RecommendedStart/EndTime"
         # but it is not clear how these should be reconciled with
 
         ifo_list = []
 
         for ifo in ifos:
             # Grab IFO specific quantities
             ifo_name = ifo["UID"]
             ifo_list.append(ifo_name)
+            if "RecommendedDuration" in detchar.keys():
+                data["segment length"] = detchar["RecommendedDuration"]
             if "RecommendedMaximumFrequency" in ifo.keys():
                 max_f[ifo_name] = ifo["RecommendedMaximumFrequency"]
             if "RecommendedMinimumFrequency" in ifo.keys():
                 min_f[ifo_name] = ifo["RecommendedMinimumFrequency"]
             if "RecommendedChannel" in ifo.keys():
                 channels[ifo_name] = ifo["RecommendedChannel"]
             if "FrameType" in ifo.keys():
```

### Comparing `cbcflow-0.2.2/src/cbcflow/cbcflow.py` & `cbcflow-0.2.3/src/cbcflow/cbcflow.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow/configuration.py` & `cbcflow-0.2.3/src/cbcflow/configuration.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow/database.py` & `cbcflow-0.2.3/src/cbcflow/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Class objects for databases, and for providing supplemental database behavior"""
 import configparser
 import copy
 import glob
 import json
 import os
+import ast
 from functools import cached_property
 import sys
 from pprint import pformat
-from typing import Union, Dict, Type, TypeVar
+from typing import Union, Dict, Type, TypeVar, Tuple
 from datetime import datetime
 
 import dateutil.parser as dp
 from jsondiff import diff
 import jsonschema
 import git
 import tqdm
@@ -213,40 +214,59 @@
             The branch_name to write commits to, per `cbcflow.database.LocalLibraryDatabase.git_add_and_commit`"""
         return None
 
 
 class GraceDbDatabase(LibraryParent):
     """The LibraryParent class to use when the parent is GraceDB"""
 
-    def __init__(self, service_url: str, library: "LocalLibraryDatabase") -> None:
+    def __init__(
+        self,
+        service_url: str,
+        library: "LocalLibraryDatabase",
+        cred: Union[Tuple[str, str], str, None] = None,
+    ) -> None:
         """Setup the GraceDbDatabase that this library pairs to
 
         Parameters
         ==========
         service_url : str
             The http address for the gracedb instance that this library pairs to
         library : `LocalLibraryDatabase`
             The library for which this serves as a parent.
         """
         super(GraceDbDatabase, self).__init__(source_path=service_url, library=library)
+        self.cred = cred
+
+    @property
+    def cred(self) -> Union[Tuple[str, str], str, None]:
+        """Information on the credentials to pass to GraceDb, per
+        https://ligo-gracedb.readthedocs.io/en/latest/api.html#ligo.gracedb.rest.GraceDb
+        """
+        return self._cred
+
+    @cred.setter
+    def cred(self, input_cred: Union[Tuple[str, str], str, None]) -> None:
+        self._cred = input_cred
 
     def pull(self, sname: str) -> dict:
         """Pull information on the superevent with this sname from GraceDB
 
         Parameters
         ==========
         sname : str
             The sname for the superevent in question
 
         Returns
         =======
         dict
             The GraceDB data for the superevent
         """
-        return fetch_gracedb_information(sname, service_url=self.source_path)
+        return fetch_gracedb_information(
+            sname, service_url=self.source_path, cred=self.cred
+        )
 
     def query_superevents(self, query: str) -> list:
         """Queries superevents in GraceDb, according to a given query
 
         Parameters
         ==========
         query : str
@@ -257,15 +277,15 @@
         =======
         list
             The superevents which satisfy the query
         """
         from ligo.gracedb.rest import GraceDb
 
         queried_superevents = []
-        with GraceDb(service_url=self.source_path) as gdb:
+        with GraceDb(service_url=self.source_path, cred=self.cred) as gdb:
             superevent_iterator = gdb.superevents(query)
             for superevent in superevent_iterator:
                 queried_superevents.append(superevent["superevent_id"])
         return queried_superevents
 
     def pull_library_updates(self, branch_name: Union[str, None] = None) -> None:
         """Pulls updates from GraceDb and writes them to library, creates default data as required
@@ -374,14 +394,27 @@
             if superevent_id not in self.superevents_to_propagate:
                 self.superevents_to_propagate.append(superevent_id)
                 logger.info(
                     f"Also querying superevent {superevent_id} which was in the library\
                 \n but which did not meet query parameters"
                 )
 
+        # For special events which are called out by name, act accordingly
+        specially_included_snames = ast.literal_eval(
+            self.library.library_config["Events"]["snames-to-include"]
+        )
+        specially_excuded_snames = ast.literal_eval(
+            self.library.library_config["Events"]["snames-to-exclude"]
+        )
+
+        self.superevents_to_propagate += specially_included_snames
+        self.superevents_to_propagate = list(
+            set(self.superevents_to_propagate) - set(specially_excuded_snames)
+        )
+
         self.pull_library_updates(branch_name=branch_name)
 
 
 class LocalLibraryDatabase(object):
     """An object reflecting the contents of a local library, and offering methods to interact with it"""
 
     def __init__(
@@ -430,16 +463,34 @@
         """
         if source_path is None:
             source_path = self.library_config["Monitor"]["parent"]
             logger.info(
                 f"Initializing parent from configuration, with source path {source_path}"
             )
         if "https://gracedb" in source_path:
+            if self.library_config["Monitor"]["cred"] is not None:
+                import re
+
+                if self.library_config["Monitor"]["cred"].lower() == "none":
+                    # If it's just the string None
+                    logger.info("Using default credentials")
+                    cred = None
+                elif re.match(r"\(.,.\)", self.library_config["Monitor"]["cred"]):
+                    import ast
+
+                    logger.info("Using cred/key pair given")
+                    cred = ast.literal_eval(self.library_config["Monitor"]["cred"])
+                else:
+                    logger.info("Using path to credential proxy file")
+                    cred = self.library_config["Monitor"]["cred"]
+            else:
+                logger.info("Using default credentials")
+                cred = None
             self._library_parent = GraceDbDatabase(
-                service_url=source_path, library=self
+                service_url=source_path, library=self, cred=cred
             )
         elif os.path.exists(source_path):
             # This will be the branch for pulling from a git repo in the local filesystem
             pass
         elif "https" in source_path:
             # This will be the branch for pulling from a non-local git repo on e.g. gitlab
             pass
@@ -565,15 +616,15 @@
             "far-threshold": 1.2675e-7,
             "pastro-threshold": 0.5,
             "created-since": "2022-01-01",
             "created-before": "now",
             "snames-to-include": [],
             "snames-to-exclude": [],
         }
-        library_defaults["Monitor"] = {"parent": "gracedb"}
+        library_defaults["Monitor"] = {"parent": "gracedb", "cred": None}
         if os.path.exists(config_file):
             config.read(config_file)
             for section_key in config.sections():
                 if section_key not in library_defaults.keys():
                     library_defaults[section_key] = dict()
                 section = config[section_key]
                 for key in section.keys():
@@ -693,20 +744,38 @@
         their_file : str
             The file from head (changes being applied)
         most_recent_common_ancestor_file : str
             The file from the MRCA (last commit shared by head and base)
         """
         # `cbcflow.process.process_merge_json handles the logic for us`
         # We just need to load in files here
-        with open(our_file, "r") as file:
-            head_json = json.load(file)
-        with open(their_file, "r") as file:
-            base_json = json.load(file)
-        with open(most_recent_common_ancestor_file, "r") as file:
-            mrca_json = json.load(file)
+        try:
+            with open(our_file, "r") as file:
+                head_json = json.load(file)
+        except json.decoder.JSONDecodeError as e:
+            logger.info(
+                f"Could not read head with error {e}, proceeding as if it's empty"
+            )
+            head_json = {}
+        try:
+            with open(their_file, "r") as file:
+                base_json = json.load(file)
+        except json.decoder.JSONDecodeError as e:
+            logger.info(
+                f"Could not read base with error {e}, proceeding as if it's empty"
+            )
+            base_json = {}
+        try:
+            with open(most_recent_common_ancestor_file, "r") as file:
+                mrca_json = json.load(file)
+        except json.decoder.JSONDecodeError as e:
+            logger.info(
+                f"Could not read head with error {e}, proceeding as if it's empty"
+            )
+            mrca_json = {}
 
         # Now get the merged json and the return status
         merge_json, return_status = process_merge_json(
             base_json=base_json,
             head_json=head_json,
             mrca_json=mrca_json,
             schema=self.metadata_schema,
```

### Comparing `cbcflow-0.2.2/src/cbcflow/gracedb.py` & `cbcflow-0.2.3/src/cbcflow/gracedb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 """Methods for interacting with gracedb"""
 from datetime import datetime
-from typing import Union
+from typing import Union, Tuple
 
 from .utils import setup_logger
 
 logger = setup_logger()
 
 
-def fetch_gracedb_information(sname: str, service_url: Union[str, None] = None) -> dict:
+def fetch_gracedb_information(
+    sname: str,
+    service_url: Union[str, None] = None,
+    cred: Union[Tuple[str, str], str, None] = None,
+) -> dict:
     """Get the standard GraceDB metadata contents for this superevent
 
     Parameters
     ==========
     sname : str
         The sname of the superevent to fetch.
     service_url : Union[str, None], optional
         The url for the GraceDB instance to access.
         If None is passed then this will use the configuration default.
+    cred : Union[Tuple[str, str], str, None]
+        Per https://ligo-gracedb.readthedocs.io/en/latest/api.html#ligo.gracedb.rest.GraceDb, information on credentials
+        to use in authentication.
 
     Returns
     =======
     dict
         An update dictionary to apply to the metadata, containing the GraceDB info.
     """
     from ligo.gracedb.rest import GraceDb
@@ -30,15 +37,15 @@
         from .configuration import config_defaults
 
         service_url = config_defaults["gracedb_service_url"]
         logger.info("Using configuration default GraceDB service_url")
 
     data = dict(GraceDB=dict(Events=[]), Cosmology=dict())
 
-    with GraceDb(service_url=service_url) as gdb:
+    with GraceDb(service_url=service_url, cred=cred) as gdb:
         try:
             # Get the json of metadata for the superevent
             superevent = gdb.superevent(sname).json()
         except HTTPError:
             msg = f"Superevent {sname} not found on {service_url}. "
             msg += "Either it does not exist, or you may need to run ligo-proxy-init."
             raise ValueError(msg)
@@ -184,15 +191,15 @@
                             f"Failed to load data for event {event['graceid']}"
                         )
                     else:
                         logger.warning(
                             f"Failed to load an event for superevent {sname},\
                                     and could not return the event's id"
                         )
-            elif pipeline.lower().strip() == "cwb" and event["group"].lower() == "cbc":
+            elif pipeline.lower().strip() == "cwb" and event["search"].lower() == "bbh":
                 # Catch the pipeline cwb in the group cbc
                 try:
                     event_data = dict()
                     # Get the
                     gname = event["graceid"]
                     # Get the preferred event across pipelines
                     if gname == superevent["preferred_event"]:
```

### Comparing `cbcflow-0.2.2/src/cbcflow/metadata.py` & `cbcflow-0.2.3/src/cbcflow/metadata.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow/monitor.py` & `cbcflow-0.2.3/src/cbcflow/monitor.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow/online_pe.py` & `cbcflow-0.2.3/src/cbcflow/online_pe.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow/parser.py` & `cbcflow-0.2.3/src/cbcflow/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Parsing tools, and tools for generating default data"""
 import argparse
-from typing import Tuple
+from typing import Tuple, Union
 import re
 
 import argcomplete
 
 from .configuration import config_defaults
 from .utils import setup_logger
 
@@ -14,14 +14,38 @@
 
 group_shorthands = dict(
     parameter_estimation="parameter_estimation",
     publications="publications",
 )
 
 
+def str2bool(v: Union[str, bool]) -> bool:
+    """Helper type for argparse so we can do set True, etc,
+    from https://stackoverflow.com/questions/15008758/parsing-boolean-values-with-argparse
+
+    Parameters
+    ==========
+    v : str | bool
+        The value to comprehend. If a string will attempt to interpret.
+
+    Returns
+    =======
+    bool
+        The True/False interpretation of the value
+    """
+    if isinstance(v, bool):
+        return v
+    if v.lower() in ("yes", "true", "t", "y", "1"):
+        return True
+    elif v.lower() in ("no", "false", "f", "n", "0"):
+        return False
+    else:
+        raise argparse.ArgumentTypeError("Boolean value expected.")
+
+
 def process_property(
     key: str,
     value: dict,
     arg: str,
     parser: argparse.ArgumentParser,
     default_data: dict,
     schema: dict,
@@ -94,14 +118,21 @@
             action="store",
             help=f"Set the {arg}",
             type=float,
         )
         default = value.get("default", None)
         if default is not None:
             default_data[key] = default
+    elif value["type"] == "boolean":
+        parser.add_argument(
+            "--" + arg + "-set", action="store", help=f"Set the {arg}", type=str2bool
+        )
+        default = value.get("default", None)
+        if default is not None:
+            default_data[key] = default
     elif value["type"] == "array":
         if value["items"].get("type") == "string":
             parser.add_argument(
                 "--" + arg + "-add",
                 action="append",
                 help=f"Append to the {arg}",
             )
```

### Comparing `cbcflow-0.2.2/src/cbcflow/process.py` & `cbcflow-0.2.3/src/cbcflow/process.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow/schema/cbc-meta-data-v1.schema` & `cbcflow-0.2.3/src/cbcflow/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow/schema/cbc-meta-data-v2.schema` & `cbcflow-0.2.3/src/cbcflow/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow/schema/index-v1.schema` & `cbcflow-0.2.3/src/cbcflow/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow/schema.py` & `cbcflow-0.2.3/src/cbcflow/schema.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow/utils.py` & `cbcflow-0.2.3/src/cbcflow/utils.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow.egg-info/PKG-INFO` & `cbcflow-0.2.3/src/cbcflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/cbcflow
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/cbcflow
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/cbcflow/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.2.2/src/cbcflow.egg-info/SOURCES.txt` & `cbcflow-0.2.3/src/cbcflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/src/cbcflow.egg-info/entry_points.txt` & `cbcflow-0.2.3/src/cbcflow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/files_for_testing/cbc-meta-data-example.json` & `cbcflow-0.2.3/tests/files_for_testing/cbc-meta-data-example.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/files_for_testing/merge_test.json` & `cbcflow-0.2.3/tests/files_for_testing/merge_test.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/files_for_testing/update_json_1.json` & `cbcflow-0.2.3/tests/files_for_testing/update_json_1.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/files_for_testing/update_json_2.json` & `cbcflow-0.2.3/tests/files_for_testing/update_json_2.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/files_for_testing/update_yaml_1.yaml` & `cbcflow-0.2.3/tests/files_for_testing/update_yaml_1.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/files_for_testing/update_yaml_2.yaml` & `cbcflow-0.2.3/tests/files_for_testing/update_yaml_2.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/library_for_testing/S230227hp-cbc-metadata.json` & `cbcflow-0.2.3/tests/library_for_testing/S230227hp-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/library_for_testing/S230331e-cbc-metadata.json` & `cbcflow-0.2.3/tests/library_for_testing/S230331e-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/library_for_testing/S230401h-cbc-metadata.json` & `cbcflow-0.2.3/tests/library_for_testing/S230401h-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/library_for_testing/S230402dv-cbc-metadata.json` & `cbcflow-0.2.3/tests/library_for_testing/S230402dv-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/library_for_testing/S230403ae-cbc-metadata.json` & `cbcflow-0.2.3/tests/library_for_testing/S230403ae-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/library_for_testing/S230404hb-cbc-metadata.json` & `cbcflow-0.2.3/tests/library_for_testing/S230404hb-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/library_for_testing/S230404jc-cbc-metadata.json` & `cbcflow-0.2.3/tests/library_for_testing/S230404jc-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/test_database.py` & `cbcflow-0.2.3/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/test_merging.py` & `cbcflow-0.2.3/tests/test_merging.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/test_metadata.py` & `cbcflow-0.2.3/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.2/tests/test_schema.py` & `cbcflow-0.2.3/tests/test_schema.py`

 * *Files identical despite different names*

