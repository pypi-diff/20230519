# Comparing `tmp/libNeuroML-0.5.1.tar.gz` & `tmp/libNeuroML-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libNeuroML-0.5.1.tar", last modified: Wed May 10 10:15:48 2023, max compression
+gzip compressed data, was "libNeuroML-0.5.2.tar", last modified: Fri May 19 08:28:17 2023, max compression
```

## Comparing `libNeuroML-0.5.1.tar` & `libNeuroML-0.5.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.215885 libNeuroML-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-10 10:15:48.215885 libNeuroML-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.207885 libNeuroML-0.5.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.207885 libNeuroML-0.5.1/libNeuroML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-10 10:15:48.000000 libNeuroML-0.5.1/libNeuroML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-10 10:15:48.000000 libNeuroML-0.5.1/libNeuroML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 10:15:48.000000 libNeuroML-0.5.1/libNeuroML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 10:15:48.000000 libNeuroML-0.5.1/libNeuroML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 10:15:48.000000 libNeuroML-0.5.1/libNeuroML.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.207885 libNeuroML-0.5.1/neuroml/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/arraymorph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/arraymorph_load_time_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.207885 libNeuroML-0.5.1/neuroml/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/hdf5/DefaultNetworkHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    15728 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/hdf5/NetworkBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/hdf5/NetworkContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29523 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/hdf5/NeuroMLHdf5Parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/hdf5/NeuroMLXMLParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/neuro_lex_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.211885 libNeuroML-0.5.1/neuroml/nml/
--rw-r--r--   0 runner    (1001) docker     (123)   137302 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   137302 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.1.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   169821 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.2.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   178637 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.3.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    73810 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta1.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    79479 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta2.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    84413 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta3.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   129617 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta4.xsd
--rw-r--r--   0 runner    (1001) docker     (123)   137302 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta5.xsd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/annotate_nml.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/gds_imports-template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/generateds_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/generatedscollector.py
--rw-r--r--   0 runner    (1001) docker     (123)    23753 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/generatedssupersuper.py
--rw-r--r--   0 runner    (1001) docker     (123)   107919 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)  2412988 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/nml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.215885 libNeuroML-0.5.1/neuroml/test/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/README
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/misc_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_arraymorph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_hdf5_optimized.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_hdf5_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)    25543 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_nml.py
--rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_writers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/writers.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-10 10:15:48.215885 libNeuroML-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:17.474784 libNeuroML-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-19 08:28:17.474784 libNeuroML-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:17.462783 libNeuroML-0.5.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:17.462783 libNeuroML-0.5.2/libNeuroML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-19 08:28:17.000000 libNeuroML-0.5.2/libNeuroML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-19 08:28:17.000000 libNeuroML-0.5.2/libNeuroML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 08:28:17.000000 libNeuroML-0.5.2/libNeuroML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 08:28:17.000000 libNeuroML-0.5.2/libNeuroML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 08:28:17.000000 libNeuroML-0.5.2/libNeuroML.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:17.462783 libNeuroML-0.5.2/neuroml/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/arraymorph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/arraymorph_load_time_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:17.466783 libNeuroML-0.5.2/neuroml/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/hdf5/DefaultNetworkHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15728 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/hdf5/NetworkBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/hdf5/NetworkContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29523 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/hdf5/NeuroMLHdf5Parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/hdf5/NeuroMLXMLParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/neuro_lex_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:17.470783 libNeuroML-0.5.2/neuroml/nml/
+-rw-r--r--   0 runner    (1001) docker     (123)   137302 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/NeuroML_v2.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   137302 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/NeuroML_v2.1.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   169821 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/NeuroML_v2.2.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   178637 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/NeuroML_v2.3.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    73810 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/NeuroML_v2beta1.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    79479 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/NeuroML_v2beta2.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    84413 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/NeuroML_v2beta3.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   129617 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/NeuroML_v2beta4.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   137302 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/NeuroML_v2beta5.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/annotate_nml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/gds_imports-template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/generateds_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/generatedscollector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23837 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/generatedssupersuper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107919 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2412988 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/nml/nml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:17.474784 libNeuroML-0.5.2/neuroml/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/README
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/misc_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/test_arraymorph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/test_hdf5_optimized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/test_hdf5_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/test_morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25543 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/test_nml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/test_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/test/test_xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/neuroml/writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-19 08:28:17.474784 libNeuroML-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-19 08:28:00.000000 libNeuroML-0.5.2/setup.py
```

### Comparing `libNeuroML-0.5.1/LICENSE` & `libNeuroML-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/PKG-INFO` & `libNeuroML-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libNeuroML
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Python library for working with NeuroML descriptions of neuronal models
 Home-page: http://libneuroml.readthedocs.org/en/latest/
 Author: libNeuroML authors and contributors
 Author-email: vellamike@gmail.com, p.gleeson@gmail.com
 License: BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `libNeuroML-0.5.1/README.md` & `libNeuroML-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/doc/Makefile` & `libNeuroML-0.5.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/doc/conf.py` & `libNeuroML-0.5.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/libNeuroML.egg-info/PKG-INFO` & `libNeuroML-0.5.2/libNeuroML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libNeuroML
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Python library for working with NeuroML descriptions of neuronal models
 Home-page: http://libneuroml.readthedocs.org/en/latest/
 Author: libNeuroML authors and contributors
 Author-email: vellamike@gmail.com, p.gleeson@gmail.com
 License: BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `libNeuroML-0.5.1/libNeuroML.egg-info/SOURCES.txt` & `libNeuroML-0.5.2/libNeuroML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/arraymorph.py` & `libNeuroML-0.5.2/neuroml/arraymorph.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/arraymorph_load_time_benchmark.py` & `libNeuroML-0.5.2/neuroml/arraymorph_load_time_benchmark.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/hdf5/DefaultNetworkHandler.py` & `libNeuroML-0.5.2/neuroml/hdf5/DefaultNetworkHandler.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/hdf5/NetworkBuilder.py` & `libNeuroML-0.5.2/neuroml/hdf5/NetworkBuilder.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/hdf5/NetworkContainer.py` & `libNeuroML-0.5.2/neuroml/hdf5/NetworkContainer.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/hdf5/NeuroMLHdf5Parser.py` & `libNeuroML-0.5.2/neuroml/hdf5/NeuroMLHdf5Parser.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/hdf5/NeuroMLXMLParser.py` & `libNeuroML-0.5.2/neuroml/hdf5/NeuroMLXMLParser.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/hdf5/__init__.py` & `libNeuroML-0.5.2/neuroml/hdf5/__init__.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/loaders.py` & `libNeuroML-0.5.2/neuroml/loaders.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/neuro_lex_ids.py` & `libNeuroML-0.5.2/neuroml/neuro_lex_ids.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.0.xsd` & `libNeuroML-0.5.2/neuroml/nml/NeuroML_v2.0.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.1.xsd` & `libNeuroML-0.5.2/neuroml/nml/NeuroML_v2.1.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.2.xsd` & `libNeuroML-0.5.2/neuroml/nml/NeuroML_v2.2.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.3.xsd` & `libNeuroML-0.5.2/neuroml/nml/NeuroML_v2.3.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta1.xsd` & `libNeuroML-0.5.2/neuroml/nml/NeuroML_v2beta1.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta2.xsd` & `libNeuroML-0.5.2/neuroml/nml/NeuroML_v2beta2.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta3.xsd` & `libNeuroML-0.5.2/neuroml/nml/NeuroML_v2beta3.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta4.xsd` & `libNeuroML-0.5.2/neuroml/nml/NeuroML_v2beta4.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta5.xsd` & `libNeuroML-0.5.2/neuroml/nml/NeuroML_v2beta5.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/annotate_nml.py` & `libNeuroML-0.5.2/neuroml/nml/annotate_nml.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/generateds_config.py` & `libNeuroML-0.5.2/neuroml/nml/generateds_config.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/generatedscollector.py` & `libNeuroML-0.5.2/neuroml/nml/generatedscollector.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/generatedssupersuper.py` & `libNeuroML-0.5.2/neuroml/nml/generatedssupersuper.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,16 +299,17 @@
         try:
             info_str = "{}\n\n".format(
                 self.__class__.__doc__.split(":param")[0].strip()
             )
         except AttributeError:
             info_str = ""
 
-        info_str += "Please see the NeuroML standard schema documentation at https://docs.neuroml.org/Userdocs/NeuroMLv2.html for more information.\n\n"
-        info_str += "Valid members for {} are:\n".format(self.__class__.__name__)
+        class_name = self.__class__.__name__
+        info_str += f"NeuroMLv2 schema documentation: https://docs.neuroml.org/Userdocs/Schemas/Index.html?highlight={class_name[0].lower()}{class_name[1:]}#{class_name.lower()} for more information.\n\n"
+        info_str += "Valid members for {} are:\n".format(class_name)
         all_members = self._get_members()
         for member in all_members:
             info_str += "* {} (class: {}, {})\n".format(
                 member.get_name(),
                 member.get_data_type(),
                 "Optional" if member.get_optional() else "Required",
             )
```

### Comparing `libNeuroML-0.5.1/neuroml/nml/helper_methods.py` & `libNeuroML-0.5.2/neuroml/nml/helper_methods.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/nml/nml.py` & `libNeuroML-0.5.2/neuroml/nml/nml.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/test/misc_tests.py` & `libNeuroML-0.5.2/neuroml/test/misc_tests.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/test/test_arraymorph.py` & `libNeuroML-0.5.2/neuroml/test/test_arraymorph.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/test/test_cell.py` & `libNeuroML-0.5.2/neuroml/test/test_cell.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/test/test_hdf5_optimized.py` & `libNeuroML-0.5.2/neuroml/test/test_hdf5_optimized.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/test/test_hdf5_parser.py` & `libNeuroML-0.5.2/neuroml/test/test_hdf5_parser.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/test/test_integration.py` & `libNeuroML-0.5.2/neuroml/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/test/test_loaders.py` & `libNeuroML-0.5.2/neuroml/test/test_loaders.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/test/test_morphology.py` & `libNeuroML-0.5.2/neuroml/test/test_morphology.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/test/test_nml.py` & `libNeuroML-0.5.2/neuroml/test/test_nml.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/test/test_segment.py` & `libNeuroML-0.5.2/neuroml/test/test_segment.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/test/test_utils.py` & `libNeuroML-0.5.2/neuroml/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/test/test_writers.py` & `libNeuroML-0.5.2/neuroml/test/test_writers.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/test/test_xml_parser.py` & `libNeuroML-0.5.2/neuroml/test/test_xml_parser.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/utils.py` & `libNeuroML-0.5.2/neuroml/utils.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/neuroml/writers.py` & `libNeuroML-0.5.2/neuroml/writers.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.5.1/setup.py` & `libNeuroML-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,19 @@
     packages=["neuroml", "neuroml.test", "neuroml.nml", "neuroml.hdf5"],
     package_data={"neuroml.test": ["*.nml"], "neuroml.nml": ["*.xsd"]},
     author="libNeuroML authors and contributors",
     author_email="vellamike@gmail.com, p.gleeson@gmail.com",
     description="A Python library for working with NeuroML descriptions of neuronal models",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["lxml", "six", "networkx"],
+    install_requires=["lxml", "six", "networkx", "numpy"],
     tests_require=["pytest"],
     extras_require={
         "full": [
             "cython",
-            "numpy",
             "numexpr",
             "tables>=3.3.0",
         ]
     },
     license="BSD",
     url="http://libneuroml.readthedocs.org/en/latest/",
     classifiers=[
```

