# Comparing `tmp/hans-0.1.2.tar.gz` & `tmp/hans-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hans-0.1.2.tar", last modified: Tue Dec 20 14:33:04 2022, max compression
+gzip compressed data, was "hans-0.1.3.tar", last modified: Fri May 19 07:49:22 2023, max compression
```

## Comparing `hans-0.1.2.tar` & `hans-0.1.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:33:04.529513 hans-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:33:04.513513 hans-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:33:04.517513 hans-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2022-12-20 14:32:44.000000 hans-0.1.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-20 14:32:44.000000 hans-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-20 14:32:44.000000 hans-0.1.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-20 14:32:44.000000 hans-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2022-12-20 14:33:04.529513 hans-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2022-12-20 14:32:44.000000 hans-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:33:04.521513 hans-0.1.2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2022-12-20 14:32:44.000000 hans-0.1.2/cli/animate1D.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2022-12-20 14:32:44.000000 hans-0.1.2/cli/animate2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2022-12-20 14:32:44.000000 hans-0.1.2/cli/generate_roughness.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3648 2022-12-20 14:32:44.000000 hans-0.1.2/cli/plot1D_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2022-12-20 14:32:44.000000 hans-0.1.2/cli/plot1D_height.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2784 2022-12-20 14:32:44.000000 hans-0.1.2/cli/plot1D_last.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2022-12-20 14:32:44.000000 hans-0.1.2/cli/plot2D_height.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2022-12-20 14:32:44.000000 hans-0.1.2/cli/plot2D_last.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3144 2022-12-20 14:32:44.000000 hans-0.1.2/cli/plot_scalar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1725 2022-12-20 14:32:44.000000 hans-0.1.2/cli/read_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:33:04.521513 hans-0.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2022-12-20 14:32:44.000000 hans-0.1.2/examples/channel1D_DH.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      511 2022-12-20 14:32:44.000000 hans-0.1.2/examples/channel1D_DH.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      515 2022-12-20 14:32:44.000000 hans-0.1.2/examples/channel1D_incomp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      518 2022-12-20 14:32:44.000000 hans-0.1.2/examples/channel_slip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2022-12-20 14:32:44.000000 hans-0.1.2/examples/journal1D_DH.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      478 2022-12-20 14:32:44.000000 hans-0.1.2/examples/journal1D_DH.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2022-12-20 14:32:44.000000 hans-0.1.2/examples/journal1D_incomp.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      479 2022-12-20 14:32:44.000000 hans-0.1.2/examples/journal1D_incomp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2022-12-20 14:32:44.000000 hans-0.1.2/examples/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2022-12-20 14:32:44.000000 hans-0.1.2/examples/pslider1D_cav.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      546 2022-12-20 14:32:44.000000 hans-0.1.2/examples/pslider1D_cav.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2022-12-20 14:32:44.000000 hans-0.1.2/examples/slider1D_ideal-gas.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      456 2022-12-20 14:32:44.000000 hans-0.1.2/examples/slider1D_ideal-gas.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:33:04.525513 hans-0.1.2/hans/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2022-12-20 14:32:44.000000 hans-0.1.2/hans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2022-12-20 14:32:44.000000 hans-0.1.2/hans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2022-12-20 14:32:44.000000 hans-0.1.2/hans/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    20118 2022-12-20 14:32:44.000000 hans-0.1.2/hans/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    21850 2022-12-20 14:32:44.000000 hans-0.1.2/hans/input.py
--rw-r--r--   0 runner    (1001) docker     (123)    23272 2022-12-20 14:32:44.000000 hans-0.1.2/hans/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2022-12-20 14:32:44.000000 hans-0.1.2/hans/material.py
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2022-12-20 14:32:44.000000 hans-0.1.2/hans/plottools.py
--rw-r--r--   0 runner    (1001) docker     (123)    20463 2022-12-20 14:32:44.000000 hans-0.1.2/hans/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    24230 2022-12-20 14:32:44.000000 hans-0.1.2/hans/stress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2022-12-20 14:32:44.000000 hans-0.1.2/hans/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:33:04.525513 hans-0.1.2/hans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2022-12-20 14:33:04.000000 hans-0.1.2/hans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2022-12-20 14:33:04.000000 hans-0.1.2/hans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 14:33:04.000000 hans-0.1.2/hans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2022-12-20 14:33:04.000000 hans-0.1.2/hans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-20 14:33:04.000000 hans-0.1.2/hans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-20 14:33:04.000000 hans-0.1.2/hans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 14:33:04.000000 hans-0.1.2/hans.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:33:04.529513 hans-0.1.2/maintenance/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2022-12-20 14:32:44.000000 hans-0.1.2/maintenance/copyright.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      737 2022-12-20 14:32:44.000000 hans-0.1.2/maintenance/create_tag.sh
--rw-r--r--   0 runner    (1001) docker     (123)      384 2022-12-20 14:32:44.000000 hans-0.1.2/maintenance/replace_header.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2022-12-20 14:32:44.000000 hans-0.1.2/maintenance/update_license_headers.sh
--rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-20 14:32:44.000000 hans-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-20 14:32:44.000000 hans-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2022-12-20 14:33:04.529513 hans-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:33:04.529513 hans-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 14:32:44.000000 hans-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2022-12-20 14:32:44.000000 hans-0.1.2/tests/channel-slip1D_x_incompressible.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2022-12-20 14:32:44.000000 hans-0.1.2/tests/channel-slip1D_y_incompressible.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2022-12-20 14:32:44.000000 hans-0.1.2/tests/inclined-slider1D_ideal-gas_U50_s5.6e-4.dat
--rw-r--r--   0 runner    (1001) docker     (123)      462 2022-12-20 14:32:44.000000 hans-0.1.2/tests/inclined-slider1D_x_ideal-gas.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      464 2022-12-20 14:32:44.000000 hans-0.1.2/tests/inclined-slider1D_y_ideal-gas.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2022-12-20 14:32:44.000000 hans-0.1.2/tests/journal-bearing1D_eps0.7_incompressible.dat
--rw-r--r--   0 runner    (1001) docker     (123)      488 2022-12-20 14:32:44.000000 hans-0.1.2/tests/journal-bearing1D_x_incompressible.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2022-12-20 14:32:44.000000 hans-0.1.2/tests/journal-bearing1D_y_incompressible.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2022-12-20 14:32:44.000000 hans-0.1.2/tests/test_channel-slip_1D_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2022-12-20 14:32:44.000000 hans-0.1.2/tests/test_channel-slip_1D_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2022-12-20 14:32:44.000000 hans-0.1.2/tests/test_inclined-slider_1D_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2022-12-20 14:32:44.000000 hans-0.1.2/tests/test_inclined-slider_1D_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2022-12-20 14:32:44.000000 hans-0.1.2/tests/test_journal-bearing_1D_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2022-12-20 14:32:44.000000 hans-0.1.2/tests/test_journal-bearing_1D_y.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:22.911721 hans-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:22.899721 hans-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:22.899721 hans-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-19 07:49:01.000000 hans-0.1.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 07:49:01.000000 hans-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-19 07:49:01.000000 hans-0.1.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-19 07:49:01.000000 hans-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-19 07:49:22.911721 hans-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-19 07:49:01.000000 hans-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:22.903721 hans-0.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-19 07:49:01.000000 hans-0.1.3/examples/channel1D_DH.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-19 07:49:01.000000 hans-0.1.3/examples/channel1D_DH.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-19 07:49:01.000000 hans-0.1.3/examples/channel1D_incomp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-19 07:49:01.000000 hans-0.1.3/examples/channel_slip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-19 07:49:01.000000 hans-0.1.3/examples/journal1D_DH.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-19 07:49:01.000000 hans-0.1.3/examples/journal1D_DH.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-19 07:49:01.000000 hans-0.1.3/examples/journal1D_incomp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-19 07:49:01.000000 hans-0.1.3/examples/journal1D_incomp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-19 07:49:01.000000 hans-0.1.3/examples/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-19 07:49:01.000000 hans-0.1.3/examples/pslider1D_cav.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-19 07:49:01.000000 hans-0.1.3/examples/pslider1D_cav.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-19 07:49:01.000000 hans-0.1.3/examples/slider1D_ideal-gas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-19 07:49:01.000000 hans-0.1.3/examples/slider1D_ideal-gas.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:22.903721 hans-0.1.3/hans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-19 07:49:01.000000 hans-0.1.3/hans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-19 07:49:01.000000 hans-0.1.3/hans/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:22.907721 hans-0.1.3/hans/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-19 07:49:01.000000 hans-0.1.3/hans/cli/animate1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-19 07:49:01.000000 hans-0.1.3/hans/cli/animate2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-19 07:49:01.000000 hans-0.1.3/hans/cli/generate_roughness.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3648 2023-05-19 07:49:01.000000 hans-0.1.3/hans/cli/plot1D_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-19 07:49:01.000000 hans-0.1.3/hans/cli/plot1D_height.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2784 2023-05-19 07:49:01.000000 hans-0.1.3/hans/cli/plot1D_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-19 07:49:01.000000 hans-0.1.3/hans/cli/plot2D_height.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-19 07:49:01.000000 hans-0.1.3/hans/cli/plot2D_last.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3144 2023-05-19 07:49:01.000000 hans-0.1.3/hans/cli/plot_scalar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1725 2023-05-19 07:49:01.000000 hans-0.1.3/hans/cli/read_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-05-19 07:49:01.000000 hans-0.1.3/hans/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20118 2023-05-19 07:49:01.000000 hans-0.1.3/hans/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21850 2023-05-19 07:49:01.000000 hans-0.1.3/hans/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23272 2023-05-19 07:49:01.000000 hans-0.1.3/hans/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-05-19 07:49:01.000000 hans-0.1.3/hans/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-05-19 07:49:01.000000 hans-0.1.3/hans/plottools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20463 2023-05-19 07:49:01.000000 hans-0.1.3/hans/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24230 2023-05-19 07:49:01.000000 hans-0.1.3/hans/stress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-19 07:49:01.000000 hans-0.1.3/hans/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:22.903721 hans-0.1.3/hans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-19 07:49:22.000000 hans-0.1.3/hans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-19 07:49:22.000000 hans-0.1.3/hans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 07:49:22.000000 hans-0.1.3/hans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-19 07:49:22.000000 hans-0.1.3/hans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-19 07:49:22.000000 hans-0.1.3/hans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 07:49:22.000000 hans-0.1.3/hans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 07:49:22.000000 hans-0.1.3/hans.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:22.907721 hans-0.1.3/maintenance/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-19 07:49:01.000000 hans-0.1.3/maintenance/copyright.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      737 2023-05-19 07:49:01.000000 hans-0.1.3/maintenance/create_tag.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-19 07:49:01.000000 hans-0.1.3/maintenance/replace_header.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-19 07:49:01.000000 hans-0.1.3/maintenance/update_license_headers.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-19 07:49:01.000000 hans-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-19 07:49:01.000000 hans-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-19 07:49:22.911721 hans-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:22.911721 hans-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 07:49:01.000000 hans-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-19 07:49:01.000000 hans-0.1.3/tests/channel-slip1D_x_incompressible.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-19 07:49:01.000000 hans-0.1.3/tests/channel-slip1D_y_incompressible.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-05-19 07:49:01.000000 hans-0.1.3/tests/inclined-slider1D_ideal-gas_U50_s5.6e-4.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 07:49:01.000000 hans-0.1.3/tests/inclined-slider1D_x_ideal-gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-19 07:49:01.000000 hans-0.1.3/tests/inclined-slider1D_y_ideal-gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-19 07:49:01.000000 hans-0.1.3/tests/journal-bearing1D_eps0.7_incompressible.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-19 07:49:01.000000 hans-0.1.3/tests/journal-bearing1D_x_incompressible.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-19 07:49:01.000000 hans-0.1.3/tests/journal-bearing1D_y_incompressible.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-19 07:49:01.000000 hans-0.1.3/tests/test_channel-slip_1D_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-19 07:49:01.000000 hans-0.1.3/tests/test_channel-slip_1D_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-19 07:49:01.000000 hans-0.1.3/tests/test_inclined-slider_1D_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-19 07:49:01.000000 hans-0.1.3/tests/test_inclined-slider_1D_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-19 07:49:01.000000 hans-0.1.3/tests/test_journal-bearing_1D_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-19 07:49:01.000000 hans-0.1.3/tests/test_journal-bearing_1D_y.py
```

### Comparing `hans-0.1.2/.github/workflows/ci.yaml` & `hans-0.1.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/LICENSE.md` & `hans-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/PKG-INFO` & `hans-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hans
-Version: 0.1.2
+Version: 0.1.3
 Summary: Height-Averaged Navier-Stokes (HANS) solver for 2D lubrication problems
 Home-page: http://github.com/hannes-holey/hans
 Author: Hannes Holey
 Author-email: hannes.holey@kit.edu
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hans-0.1.2/README.md` & `hans-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/cli/animate1D.py` & `hans-0.1.3/hans/cli/animate1D.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/cli/animate2D.py` & `hans-0.1.3/hans/cli/animate2D.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/cli/generate_roughness.py` & `hans-0.1.3/hans/cli/generate_roughness.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/cli/plot1D_evolution.py` & `hans-0.1.3/hans/cli/plot1D_evolution.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/cli/plot1D_height.py` & `hans-0.1.3/hans/cli/plot1D_height.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/cli/plot1D_last.py` & `hans-0.1.3/hans/cli/plot1D_last.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/cli/plot2D_height.py` & `hans-0.1.3/hans/cli/plot2D_height.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/cli/plot2D_last.py` & `hans-0.1.3/hans/cli/plot2D_last.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/cli/plot_scalar.py` & `hans-0.1.3/hans/cli/plot_scalar.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/cli/read_config.py` & `hans-0.1.3/hans/cli/read_config.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/examples/channel1D_DH.ipynb` & `hans-0.1.3/examples/channel1D_DH.ipynb`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/examples/channel1D_incomp.yaml` & `hans-0.1.3/examples/channel1D_incomp.yaml`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/examples/channel_slip.yaml` & `hans-0.1.3/examples/channel_slip.yaml`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/examples/journal1D_DH.ipynb` & `hans-0.1.3/examples/journal1D_DH.ipynb`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/examples/journal1D_incomp.ipynb` & `hans-0.1.3/examples/journal1D_incomp.ipynb`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/examples/matplotlibrc` & `hans-0.1.3/examples/matplotlibrc`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/examples/pslider1D_cav.ipynb` & `hans-0.1.3/examples/pslider1D_cav.ipynb`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/examples/pslider1D_cav.yaml` & `hans-0.1.3/examples/pslider1D_cav.yaml`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/examples/slider1D_ideal-gas.ipynb` & `hans-0.1.3/examples/slider1D_ideal-gas.ipynb`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/hans/__init__.py` & `hans-0.1.3/hans/__init__.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/hans/__main__.py` & `hans-0.1.3/hans/__main__.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/hans/field.py` & `hans-0.1.3/hans/field.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/hans/geometry.py` & `hans-0.1.3/hans/geometry.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/hans/input.py` & `hans-0.1.3/hans/input.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/hans/integrate.py` & `hans-0.1.3/hans/integrate.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/hans/material.py` & `hans-0.1.3/hans/material.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/hans/plottools.py` & `hans-0.1.3/hans/plottools.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/hans/problem.py` & `hans-0.1.3/hans/problem.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/hans/stress.py` & `hans-0.1.3/hans/stress.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/hans/tools.py` & `hans-0.1.3/hans/tools.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/hans.egg-info/PKG-INFO` & `hans-0.1.3/hans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hans
-Version: 0.1.2
+Version: 0.1.3
 Summary: Height-Averaged Navier-Stokes (HANS) solver for 2D lubrication problems
 Home-page: http://github.com/hannes-holey/hans
 Author: Hannes Holey
 Author-email: hannes.holey@kit.edu
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hans-0.1.2/hans.egg-info/SOURCES.txt` & `hans-0.1.3/hans.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,24 +2,14 @@
 AUTHORS
 LICENSE.md
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 .github/workflows/ci.yaml
-cli/animate1D.py
-cli/animate2D.py
-cli/generate_roughness.py
-cli/plot1D_evolution.py
-cli/plot1D_height.py
-cli/plot1D_last.py
-cli/plot2D_height.py
-cli/plot2D_last.py
-cli/plot_scalar.py
-cli/read_config.py
 examples/channel1D_DH.ipynb
 examples/channel1D_DH.yaml
 examples/channel1D_incomp.yaml
 examples/channel_slip.yaml
 examples/journal1D_DH.ipynb
 examples/journal1D_DH.yaml
 examples/journal1D_incomp.ipynb
@@ -43,14 +33,24 @@
 hans.egg-info/PKG-INFO
 hans.egg-info/SOURCES.txt
 hans.egg-info/dependency_links.txt
 hans.egg-info/entry_points.txt
 hans.egg-info/requires.txt
 hans.egg-info/top_level.txt
 hans.egg-info/zip-safe
+hans/cli/animate1D.py
+hans/cli/animate2D.py
+hans/cli/generate_roughness.py
+hans/cli/plot1D_evolution.py
+hans/cli/plot1D_height.py
+hans/cli/plot1D_last.py
+hans/cli/plot2D_height.py
+hans/cli/plot2D_last.py
+hans/cli/plot_scalar.py
+hans/cli/read_config.py
 maintenance/copyright.py
 maintenance/create_tag.sh
 maintenance/replace_header.py
 maintenance/update_license_headers.sh
 tests/__init__.py
 tests/channel-slip1D_x_incompressible.yaml
 tests/channel-slip1D_y_incompressible.yaml
```

### Comparing `hans-0.1.2/maintenance/copyright.py` & `hans-0.1.3/maintenance/copyright.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/maintenance/create_tag.sh` & `hans-0.1.3/maintenance/create_tag.sh`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/setup.cfg` & `hans-0.1.3/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 	pytest>=4
 	scipy>=1.3
 python_requires = >=3.6
 tests_require = pytest
 
 [options.entry_points]
 console_scripts = 
-	animate1D = cli:animate1D.main
-	animate2D = cli:animate2D.main
-	generate_roughness = cli:generate_roughness.main
-	plot1D_evolution = cli:plot1D_evolution.main
-	plot1D_height = cli:plot1D_height.main
-	plot1D_last = cli:plot1D_last.main
-	plot2D_height = cli:plot2D_height.main
-	plot2D_last = cli:plot2D_last.main
-	plot_scalar = cli:plot_scalar.main
-	read_config = cli:read_config.main
+	animate1D = hans.cli:animate1D.main
+	animate2D = hans.cli:animate2D.main
+	generate_roughness = hans.cli:generate_roughness.main
+	plot1D_evolution = hans.cli:plot1D_evolution.main
+	plot1D_height = hans.cli:plot1D_height.main
+	plot1D_last = hans.cli:plot1D_last.main
+	plot2D_height = hans.cli:plot2D_height.main
+	plot2D_last = hans.cli:plot2D_last.main
+	plot_scalar = hans.cli:plot_scalar.main
+	read_config = hans.cli:read_config.main
 
 [flake8]
 max_line_length = 140
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `hans-0.1.2/tests/channel-slip1D_x_incompressible.yaml` & `hans-0.1.3/tests/channel-slip1D_x_incompressible.yaml`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/tests/channel-slip1D_y_incompressible.yaml` & `hans-0.1.3/tests/channel-slip1D_y_incompressible.yaml`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/tests/inclined-slider1D_ideal-gas_U50_s5.6e-4.dat` & `hans-0.1.3/tests/inclined-slider1D_ideal-gas_U50_s5.6e-4.dat`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/tests/journal-bearing1D_eps0.7_incompressible.dat` & `hans-0.1.3/tests/journal-bearing1D_eps0.7_incompressible.dat`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/tests/test_channel-slip_1D_x.py` & `hans-0.1.3/tests/test_channel-slip_1D_x.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/tests/test_channel-slip_1D_y.py` & `hans-0.1.3/tests/test_channel-slip_1D_y.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/tests/test_inclined-slider_1D_x.py` & `hans-0.1.3/tests/test_inclined-slider_1D_x.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/tests/test_inclined-slider_1D_y.py` & `hans-0.1.3/tests/test_inclined-slider_1D_y.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/tests/test_journal-bearing_1D_x.py` & `hans-0.1.3/tests/test_journal-bearing_1D_x.py`

 * *Files identical despite different names*

### Comparing `hans-0.1.2/tests/test_journal-bearing_1D_y.py` & `hans-0.1.3/tests/test_journal-bearing_1D_y.py`

 * *Files identical despite different names*

