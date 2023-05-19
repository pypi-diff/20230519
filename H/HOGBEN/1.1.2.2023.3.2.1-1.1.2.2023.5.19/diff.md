# Comparing `tmp/HOGBEN-1.1.2.2023.3.2.1.tar.gz` & `tmp/HOGBEN-1.1.2.2023.5.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HOGBEN-1.1.2.2023.3.2.1.tar", last modified: Thu Mar  2 10:31:25 2023, max compression
+gzip compressed data, was "HOGBEN-1.1.2.2023.5.19.tar", last modified: Fri May 19 13:25:17 2023, max compression
```

## Comparing `HOGBEN-1.1.2.2023.3.2.1.tar` & `HOGBEN-1.1.2.2023.5.19.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:25.879374 HOGBEN-1.1.2.2023.3.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:25.879374 HOGBEN-1.1.2.2023.3.2.1/HOGBEN.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-03-02 10:31:25.000000 HOGBEN-1.1.2.2023.3.2.1/HOGBEN.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-02 10:31:25.000000 HOGBEN-1.1.2.2023.3.2.1/HOGBEN.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-02 10:31:11.000000 HOGBEN-1.1.2.2023.3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-02 10:31:11.000000 HOGBEN-1.1.2.2023.3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-03-02 10:31:25.879374 HOGBEN-1.1.2.2023.3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-03-02 10:31:11.000000 HOGBEN-1.1.2.2023.3.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:25.871374 HOGBEN-1.1.2.2023.3.2.1/figures/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-03-02 10:31:11.000000 HOGBEN-1.1.2.2023.3.2.1/figures/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:25.871374 HOGBEN-1.1.2.2023.3.2.1/hogben/
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/contrasts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:25.871374 HOGBEN-1.1.2.2023.3.2.1/hogben/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:25.875374 HOGBEN-1.1.2.2023.3.2.1/hogben/data/DMPC_bilayer/
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/DMPC_bilayer/Si-D2O.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/DMPC_bilayer/Si-DMPC-D2O.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/DMPC_bilayer/Si-DMPC-H2O.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:25.875374 HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPC_RaLPS_bilayer/
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-D2O.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-H2O.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-SMW.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:25.875374 HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPG_monolayer/
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPG_monolayer/dDPPG-NRW.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPG_monolayer/hDPPG-D2O.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPG_monolayer/hDPPG-NRW.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:25.875374 HOGBEN-1.1.2.2023.3.2.1/hogben/data/YIG_sample/
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/YIG_sample/YIG_down.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/YIG_sample/YIG_up.dat
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:25.875374 HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/
--rw-r--r--   0 runner    (1001) docker     (123)    63893 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/INTER_non_polarised.dat
--rw-r--r--   0 runner    (1001) docker     (123)    51658 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/OFFSPEC_Polarised.dat
--rw-r--r--   0 runner    (1001) docker     (123)    53135 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/OFFSPEC_non_polarised.dat
--rw-r--r--   0 runner    (1001) docker     (123)    49407 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/OFFSPEC_non_polarised_old.dat
--rw-r--r--   0 runner    (1001) docker     (123)    49407 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/OFFSPEC_polarised_old.dat
--rw-r--r--   0 runner    (1001) docker     (123)    56140 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/POLREF_non_polarised.dat
--rw-r--r--   0 runner    (1001) docker     (123)    69362 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/POLREF_polarised.dat
--rw-r--r--   0 runner    (1001) docker     (123)    24527 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/SURF_non_polarised.dat
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/make_beam_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/kinetics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/magnetism.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:25.875374 HOGBEN-1.1.2.2023.3.2.1/hogben/models/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/models/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/models/bilayers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/models/magnetic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/models/monolayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/models/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/models/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/optimise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:25.879374 HOGBEN-1.1.2.2023.3.2.1/hogben/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/underlayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/hogben/visualise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:31:25.879374 HOGBEN-1.1.2.2023.3.2.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-02 10:31:25.879374 HOGBEN-1.1.2.2023.3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-02 10:31:12.000000 HOGBEN-1.1.2.2023.3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.076039 HOGBEN-1.1.2.2023.5.19/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.076039 HOGBEN-1.1.2.2023.5.19/HOGBEN.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-19 13:25:17.000000 HOGBEN-1.1.2.2023.5.19/HOGBEN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-19 13:25:17.000000 HOGBEN-1.1.2.2023.5.19/HOGBEN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-19 13:24:58.000000 HOGBEN-1.1.2.2023.5.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 13:24:58.000000 HOGBEN-1.1.2.2023.5.19/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-19 13:25:17.076039 HOGBEN-1.1.2.2023.5.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-19 13:24:58.000000 HOGBEN-1.1.2.2023.5.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.068039 HOGBEN-1.1.2.2023.5.19/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-19 13:24:58.000000 HOGBEN-1.1.2.2023.5.19/figures/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.068039 HOGBEN-1.1.2.2023.5.19/hogben/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/contrasts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.068039 HOGBEN-1.1.2.2023.5.19/hogben/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.072039 HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/Si-D2O.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/Si-DMPC-D2O.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/Si-DMPC-H2O.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.072039 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-D2O.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-H2O.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-SMW.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.072039 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/dDPPG-NRW.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/hDPPG-D2O.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/hDPPG-NRW.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.072039 HOGBEN-1.1.2.2023.5.19/hogben/data/YIG_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/YIG_sample/YIG_down.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/YIG_sample/YIG_up.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.072039 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/
+-rw-r--r--   0 runner    (1001) docker     (123)    63893 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/INTER_non_polarised.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    51658 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_Polarised.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    53135 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_non_polarised.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    49407 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_non_polarised_old.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    49407 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_polarised_old.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    56140 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/POLREF_non_polarised.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    69362 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/POLREF_polarised.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    24527 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/SURF_non_polarised.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/make_beam_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/magnetism.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.072039 HOGBEN-1.1.2.2023.5.19/hogben/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/bilayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/magnetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/monolayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/models/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/optimise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.076039 HOGBEN-1.1.2.2023.5.19/hogben/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/underlayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/hogben/visualise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:25:17.076039 HOGBEN-1.1.2.2023.5.19/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-19 13:25:17.076039 HOGBEN-1.1.2.2023.5.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-19 13:24:59.000000 HOGBEN-1.1.2.2023.5.19/setup.py
```

### Comparing `HOGBEN-1.1.2.2023.3.2.1/HOGBEN.egg-info/PKG-INFO` & `HOGBEN-1.1.2.2023.5.19/HOGBEN.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HOGBEN
-Version: 1.1.2.2023.3.2.1
+Version: 1.1.2.2023.5.19
 Summary: Holistic Optimization for Generating Better Experimental Neutrons - a package for optimzing neutron experiments using the Fisher information
 Home-page: https://github.com/jfkcooper/HOGBEN
 Author: Joshaniel Cooper
 Author-email: Jos.Cooper@stfc.ac.uk
 Project-URL: Bug Tracker, https://github.com/jfkcooper/HOGBEN/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `HOGBEN-1.1.2.2023.3.2.1/HOGBEN.egg-info/SOURCES.txt` & `HOGBEN-1.1.2.2023.5.19/HOGBEN.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/LICENSE` & `HOGBEN-1.1.2.2023.5.19/LICENSE`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/PKG-INFO` & `HOGBEN-1.1.2.2023.5.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HOGBEN
-Version: 1.1.2.2023.3.2.1
+Version: 1.1.2.2023.5.19
 Summary: Holistic Optimization for Generating Better Experimental Neutrons - a package for optimzing neutron experiments using the Fisher information
 Home-page: https://github.com/jfkcooper/HOGBEN
 Author: Joshaniel Cooper
 Author-email: Jos.Cooper@stfc.ac.uk
 Project-URL: Bug Tracker, https://github.com/jfkcooper/HOGBEN/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `HOGBEN-1.1.2.2023.3.2.1/README.md` & `HOGBEN-1.1.2.2023.5.19/README.md`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/figures/README.md` & `HOGBEN-1.1.2.2023.5.19/figures/README.md`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/README.md` & `HOGBEN-1.1.2.2023.5.19/hogben/README.md`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/angles.py` & `HOGBEN-1.1.2.2023.5.19/hogben/angles.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/contrasts.py` & `HOGBEN-1.1.2.2023.5.19/hogben/contrasts.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/DMPC_bilayer/Si-D2O.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/Si-D2O.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/DMPC_bilayer/Si-DMPC-D2O.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/Si-DMPC-D2O.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/DMPC_bilayer/Si-DMPC-H2O.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/DMPC_bilayer/Si-DMPC-H2O.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-D2O.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-D2O.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-H2O.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-H2O.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-SMW.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/DPPC_RaLPS_bilayer/dDPPC-RaLPS-SMW.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPG_monolayer/dDPPG-NRW.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/dDPPG-NRW.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPG_monolayer/hDPPG-D2O.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/hDPPG-D2O.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/DPPG_monolayer/hDPPG-NRW.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/DPPG_monolayer/hDPPG-NRW.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/YIG_sample/YIG_down.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/YIG_sample/YIG_down.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/YIG_sample/YIG_up.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/YIG_sample/YIG_up.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/INTER_non_polarised.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/INTER_non_polarised.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/OFFSPEC_Polarised.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_Polarised.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/OFFSPEC_non_polarised.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_non_polarised.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/OFFSPEC_non_polarised_old.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_non_polarised_old.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/OFFSPEC_polarised_old.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/OFFSPEC_polarised_old.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/POLREF_non_polarised.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/POLREF_non_polarised.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/POLREF_polarised.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/POLREF_polarised.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/SURF_non_polarised.dat` & `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/SURF_non_polarised.dat`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/data/directbeams/make_beam_spectra.py` & `HOGBEN-1.1.2.2023.5.19/hogben/data/directbeams/make_beam_spectra.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/kinetics.py` & `HOGBEN-1.1.2.2023.5.19/hogben/kinetics.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/magnetism.py` & `HOGBEN-1.1.2.2023.5.19/hogben/magnetism.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/models/README.md` & `HOGBEN-1.1.2.2023.5.19/hogben/models/README.md`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/models/base.py` & `HOGBEN-1.1.2.2023.5.19/hogben/models/base.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/models/bilayers.py` & `HOGBEN-1.1.2.2023.5.19/hogben/models/bilayers.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/models/magnetic.py` & `HOGBEN-1.1.2.2023.5.19/hogben/models/magnetic.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/models/monolayers.py` & `HOGBEN-1.1.2.2023.5.19/hogben/models/monolayers.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/models/parsing.py` & `HOGBEN-1.1.2.2023.5.19/hogben/models/parsing.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/models/samples.py` & `HOGBEN-1.1.2.2023.5.19/hogben/models/samples.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/optimise.py` & `HOGBEN-1.1.2.2023.5.19/hogben/optimise.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/simulate.py` & `HOGBEN-1.1.2.2023.5.19/hogben/simulate.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/tests/test_simulation.py` & `HOGBEN-1.1.2.2023.5.19/hogben/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/underlayers.py` & `HOGBEN-1.1.2.2023.5.19/hogben/underlayers.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/utils.py` & `HOGBEN-1.1.2.2023.5.19/hogben/utils.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/hogben/visualise.py` & `HOGBEN-1.1.2.2023.5.19/hogben/visualise.py`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/notebooks/README.md` & `HOGBEN-1.1.2.2023.5.19/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `HOGBEN-1.1.2.2023.3.2.1/setup.cfg` & `HOGBEN-1.1.2.2023.5.19/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = HOGBEN
-version = 1.1.2.2023.03.02.01
+version = attr: hogben.__version__
 author = Joshaniel Cooper
 author_email = Jos.Cooper@stfc.ac.uk
 description = Holistic Optimization for Generating Better Experimental Neutrons - a package for optimzing neutron experiments using the Fisher information
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jfkcooper/HOGBEN
 project_urls = 
@@ -26,15 +26,15 @@
 	importlib_resources
 	matplotlib
 	numpy
 	periodictable
 	Pillow
 	refl1d
 	refnx
-	scipy
 	tqdm
+	scipy
 include_package_data = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

