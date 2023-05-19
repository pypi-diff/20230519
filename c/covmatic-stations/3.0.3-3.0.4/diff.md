# Comparing `tmp/covmatic-stations-3.0.3.tar.gz` & `tmp/covmatic-stations-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/covmatic-stations-3.0.3.tar", last modified: Wed Apr 26 12:47:22 2023, max compression
+gzip compressed data, was "dist/covmatic-stations-3.0.4.tar", last modified: Fri May 19 12:52:18 2023, max compression
```

## Comparing `covmatic-stations-3.0.3.tar` & `covmatic-stations-3.0.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/
--rw-r--r--   0 root         (0) root         (0)     1050 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1286 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8834 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8170 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations/
--rw-r--r--   0 root         (0) root         (0)     1356 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations/a/
--rw-r--r--   0 root         (0) root         (0)     5224 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/COPAN 15 Tube Rack 14000 µL.json
--rw-r--r--   0 root         (0) root         (0)     1058 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23355 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/a.py
--rw-r--r--   0 root         (0) root         (0)     7712 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/aBioerPreparation.py
--rw-r--r--   0 root         (0) root         (0)     7386 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/copan_24.py
--rw-r--r--   0 root         (0) root         (0)     4627 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/copan_48.py
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/copan_48_correction.json
--rw-r--r--   0 root         (0) root         (0)     5634 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/copan_48_saliva.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/
--rw-r--r--   0 root         (0) root         (0)      886 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationA.json
--rw-r--r--   0 root         (0) root         (0)      181 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationAP1000.json
--rw-r--r--   0 root         (0) root         (0)      204 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationAP1000Reload.json
--rw-r--r--   0 root         (0) root         (0)      145 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationAP300.json
--rw-r--r--   0 root         (0) root         (0)      247 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationAReloadMixin.json
--rw-r--r--   0 root         (0) root         (0)     1571 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationATechnogenetics.json
--rw-r--r--   0 root         (0) root         (0)      198 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationATechnogenetics24.json
--rw-r--r--   0 root         (0) root         (0)      198 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationATechnogenetics48.json
--rw-r--r--   0 root         (0) root         (0)     9547 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/p1000.py
--rw-r--r--   0 root         (0) root         (0)     1382 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/p1000reload.py
--rw-r--r--   0 root         (0) root         (0)     1281 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/p300.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/reload.py
--rw-r--r--   0 root         (0) root         (0)    16556 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/technogenetics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations/b/
--rw-r--r--   0 root         (0) root         (0)     1058 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32204 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/b.py
--rw-r--r--   0 root         (0) root         (0)      830 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/magnet_heights.json
--rw-r--r--   0 root         (0) root         (0)     1649 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/magnets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations/b/msg/
--rw-r--r--   0 root         (0) root         (0)      935 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/msg/StationB.json
--rw-r--r--   0 root         (0) root         (0)     2806 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/msg/StationBTechnogenetics.json
--rw-r--r--   0 root         (0) root         (0)      538 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/msg/StationBTechnogeneticsElutionRemoval.json
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/msg/StationBTechnogeneticsWashBRemoval.json
--rw-r--r--   0 root         (0) root         (0)    24730 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/nest_12_reservoir_15ml_modified.json
--rw-r--r--   0 root         (0) root         (0)    17522 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/technogenetics.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/technogenetics_short.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/bioer/
--rw-r--r--   0 root         (0) root         (0)    22106 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/bioer/Bioer_full_dw.py
--rw-r--r--   0 root         (0) root         (0)    10649 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/bioer/Bioer_preparation.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/bioer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/bioer/msg/
--rw-r--r--   0 root         (0) root         (0)      472 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/bioer/msg/BioerProtocol.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/c/
--rw-r--r--   0 root         (0) root         (0)     1058 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12774 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/bioer_mastermix_prep.py
--rw-r--r--   0 root         (0) root         (0)    16605 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/c.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/c/msg/
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/msg/StationC.json
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/msg/StationCBioerMastermixPrep.json
--rw-r--r--   0 root         (0) root         (0)      580 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/msg/StationCTechnogenetics.json
--rw-r--r--   0 root         (0) root         (0)     5005 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/technogenetics.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/geometry.py
--rw-r--r--   0 root         (0) root         (0)      560 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/hardware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/labware/
--rw-r--r--   0 root         (0) root         (0)    30016 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/labware/bioer_96_wellplate_2000ul.json
--rw-r--r--   0 root         (0) root         (0)     1370 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/labware/biofil_1_reservoir_500000ul.json
--rw-r--r--   0 root         (0) root         (0)     1983 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/labware/biofil_3_reservoir_200000ul.json
--rw-r--r--   0 root         (0) root         (0)     4003 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/lights.py
--rw-r--r--   0 root         (0) root         (0)     5008 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/movement_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/msg/
--rw-r--r--   0 root         (0) root         (0)     1644 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/msg/Station.json
--rw-r--r--   0 root         (0) root         (0)     5589 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/multi_tube_source.py
--rw-r--r--   0 root         (0) root         (0)     5276 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/request.py
--rw-r--r--   0 root         (0) root         (0)     3329 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/sound_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/sounds/
--rw-r--r--   0 root         (0) root         (0)    43884 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/sounds/alarm.mp3
--rw-r--r--   0 root         (0) root         (0)    20897 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/sounds/beep.mp3
--rw-r--r--   0 root         (0) root         (0)    23816 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/sounds/beep2.mp3
--rw-r--r--   0 root         (0) root         (0)    50089 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/sounds/finish.mp3
--rw-r--r--   0 root         (0) root         (0)    25253 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/station.py
--rw-r--r--   0 root         (0) root         (0)    13334 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8834 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2689 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2702 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8834 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8170 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations/
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations/a/
+-rw-r--r--   0 root         (0) root         (0)     5224 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/COPAN 15 Tube Rack 14000 µL.json
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23355 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/a.py
+-rw-r--r--   0 root         (0) root         (0)     7712 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/aBioerPreparation.py
+-rw-r--r--   0 root         (0) root         (0)     7386 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/copan_24.py
+-rw-r--r--   0 root         (0) root         (0)     4627 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/copan_48.py
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/copan_48_correction.json
+-rw-r--r--   0 root         (0) root         (0)     5634 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/copan_48_saliva.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations/a/msg/
+-rw-r--r--   0 root         (0) root         (0)      886 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/msg/StationA.json
+-rw-r--r--   0 root         (0) root         (0)      181 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/msg/StationAP1000.json
+-rw-r--r--   0 root         (0) root         (0)      204 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/msg/StationAP1000Reload.json
+-rw-r--r--   0 root         (0) root         (0)      145 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/msg/StationAP300.json
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/msg/StationAReloadMixin.json
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/msg/StationATechnogenetics.json
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/msg/StationATechnogenetics24.json
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/msg/StationATechnogenetics48.json
+-rw-r--r--   0 root         (0) root         (0)     9547 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/p1000.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/p1000reload.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/p300.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/reload.py
+-rw-r--r--   0 root         (0) root         (0)    16556 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/a/technogenetics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations/b/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/b/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32204 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/b/b.py
+-rw-r--r--   0 root         (0) root         (0)      830 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/b/magnet_heights.json
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/b/magnets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations/b/msg/
+-rw-r--r--   0 root         (0) root         (0)      935 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/b/msg/StationB.json
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/b/msg/StationBTechnogenetics.json
+-rw-r--r--   0 root         (0) root         (0)      538 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/b/msg/StationBTechnogeneticsElutionRemoval.json
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/b/msg/StationBTechnogeneticsWashBRemoval.json
+-rw-r--r--   0 root         (0) root         (0)    24730 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/b/nest_12_reservoir_15ml_modified.json
+-rw-r--r--   0 root         (0) root         (0)    17522 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/b/technogenetics.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/b/technogenetics_short.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations/bioer/
+-rw-r--r--   0 root         (0) root         (0)    22106 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/bioer/Bioer_full_dw.py
+-rw-r--r--   0 root         (0) root         (0)    10649 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/bioer/Bioer_preparation.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/bioer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations/bioer/msg/
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/bioer/msg/BioerProtocol.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations/c/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/c/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12774 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/c/bioer_mastermix_prep.py
+-rw-r--r--   0 root         (0) root         (0)    16605 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/c/c.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations/c/msg/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/c/msg/StationC.json
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/c/msg/StationCBioerMastermixPrep.json
+-rw-r--r--   0 root         (0) root         (0)      580 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/c/msg/StationCTechnogenetics.json
+-rw-r--r--   0 root         (0) root         (0)     5005 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/c/technogenetics.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/geometry.py
+-rw-r--r--   0 root         (0) root         (0)      560 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/hardware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations/labware/
+-rw-r--r--   0 root         (0) root         (0)    30016 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/labware/bioer_96_wellplate_2000ul.json
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/labware/biofil_1_reservoir_500000ul.json
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/labware/biofil_3_reservoir_200000ul.json
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/lights.py
+-rw-r--r--   0 root         (0) root         (0)     5008 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/movement_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations/msg/
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/msg/Station.json
+-rw-r--r--   0 root         (0) root         (0)     5589 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/multi_tube_source.py
+-rw-r--r--   0 root         (0) root         (0)     5276 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/request.py
+-rw-r--r--   0 root         (0) root         (0)     3329 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/sound_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations/sounds/
+-rw-r--r--   0 root         (0) root         (0)    43884 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/sounds/alarm.mp3
+-rw-r--r--   0 root         (0) root         (0)    20897 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/sounds/beep.mp3
+-rw-r--r--   0 root         (0) root         (0)    23816 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/sounds/beep2.mp3
+-rw-r--r--   0 root         (0) root         (0)    50089 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/sounds/finish.mp3
+-rw-r--r--   0 root         (0) root         (0)    25277 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/station.py
+-rw-r--r--   0 root         (0) root         (0)    13408 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/covmatic_stations/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8834 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/covmatic_stations.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 12:52:18.000000 covmatic-stations-3.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2702 2023-05-19 12:51:59.000000 covmatic-stations-3.0.4/setup.py
```

### Comparing `covmatic-stations-3.0.3/LICENSE` & `covmatic-stations-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/MANIFEST.in` & `covmatic-stations-3.0.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/PKG-INFO` & `covmatic-stations-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covmatic-stations
-Version: 3.0.3
+Version: 3.0.4
 Summary: Package for the COVMATIC Opentrons stations
 Home-page: https://github.com/covmatic/stations
 Author: Marco Tiraboschi
 Author-email: marco.tiraboschi@unimi.it
 Maintainer: Marco Tiraboschi, Agostino Facotti, Giada Facoetti
 Maintainer-email: marco.tiraboschi@unimi.it, agostino.facotti@gmail.com, giada.facoetti@hotmail.it
 License: UNKNOWN
```

### Comparing `covmatic-stations-3.0.3/README.md` & `covmatic-stations-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/__init__.py` & `covmatic-stations-3.0.4/covmatic_stations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-__version__ = "3.0.3"
+__version__ = "3.0.4"
 
 logging.basicConfig(
     level=logging.INFO,
     format='%(asctime)s %(name)-12s %(levelname)-8s: %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S',
 )
 logging.getLogger("asyncio").setLevel(logging.WARNING)
```

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/COPAN 15 Tube Rack 14000 µL.json` & `covmatic-stations-3.0.4/covmatic_stations/a/COPAN 15 Tube Rack 14000 µL.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/__init__.py` & `covmatic-stations-3.0.4/covmatic_stations/a/__init__.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/a.py` & `covmatic-stations-3.0.4/covmatic_stations/a/a.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/aBioerPreparation.py` & `covmatic-stations-3.0.4/covmatic_stations/a/aBioerPreparation.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/copan_24.py` & `covmatic-stations-3.0.4/covmatic_stations/a/copan_24.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/copan_48.py` & `covmatic-stations-3.0.4/covmatic_stations/a/copan_48.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/copan_48_saliva.py` & `covmatic-stations-3.0.4/covmatic_stations/a/copan_48_saliva.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/msg/StationA.json` & `covmatic-stations-3.0.4/covmatic_stations/a/msg/StationA.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/msg/StationATechnogenetics.json` & `covmatic-stations-3.0.4/covmatic_stations/a/msg/StationATechnogenetics.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/p1000.py` & `covmatic-stations-3.0.4/covmatic_stations/a/p1000.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/p1000reload.py` & `covmatic-stations-3.0.4/covmatic_stations/a/p1000reload.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/p300.py` & `covmatic-stations-3.0.4/covmatic_stations/a/p300.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/reload.py` & `covmatic-stations-3.0.4/covmatic_stations/a/reload.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/a/technogenetics.py` & `covmatic-stations-3.0.4/covmatic_stations/a/technogenetics.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/b/__init__.py` & `covmatic-stations-3.0.4/covmatic_stations/b/__init__.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/b/b.py` & `covmatic-stations-3.0.4/covmatic_stations/b/b.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/b/magnet_heights.json` & `covmatic-stations-3.0.4/covmatic_stations/b/magnet_heights.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/b/magnets.py` & `covmatic-stations-3.0.4/covmatic_stations/b/magnets.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/b/msg/StationB.json` & `covmatic-stations-3.0.4/covmatic_stations/b/msg/StationB.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/b/msg/StationBTechnogenetics.json` & `covmatic-stations-3.0.4/covmatic_stations/b/msg/StationBTechnogenetics.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/b/msg/StationBTechnogeneticsElutionRemoval.json` & `covmatic-stations-3.0.4/covmatic_stations/b/msg/StationBTechnogeneticsElutionRemoval.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/b/nest_12_reservoir_15ml_modified.json` & `covmatic-stations-3.0.4/covmatic_stations/b/nest_12_reservoir_15ml_modified.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/b/technogenetics.py` & `covmatic-stations-3.0.4/covmatic_stations/b/technogenetics.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/b/technogenetics_short.py` & `covmatic-stations-3.0.4/covmatic_stations/b/technogenetics_short.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/bioer/Bioer_full_dw.py` & `covmatic-stations-3.0.4/covmatic_stations/bioer/Bioer_full_dw.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/bioer/Bioer_preparation.py` & `covmatic-stations-3.0.4/covmatic_stations/bioer/Bioer_preparation.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/bioer/__init__.py` & `covmatic-stations-3.0.4/covmatic_stations/bioer/__init__.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/c/__init__.py` & `covmatic-stations-3.0.4/covmatic_stations/c/__init__.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/c/bioer_mastermix_prep.py` & `covmatic-stations-3.0.4/covmatic_stations/c/bioer_mastermix_prep.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/c/c.py` & `covmatic-stations-3.0.4/covmatic_stations/c/c.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/c/msg/StationC.json` & `covmatic-stations-3.0.4/covmatic_stations/c/msg/StationC.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/c/msg/StationCBioerMastermixPrep.json` & `covmatic-stations-3.0.4/covmatic_stations/c/msg/StationCBioerMastermixPrep.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/c/msg/StationCTechnogenetics.json` & `covmatic-stations-3.0.4/covmatic_stations/c/msg/StationCTechnogenetics.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/c/technogenetics.py` & `covmatic-stations-3.0.4/covmatic_stations/c/technogenetics.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/geometry.py` & `covmatic-stations-3.0.4/covmatic_stations/geometry.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/hardware.py` & `covmatic-stations-3.0.4/covmatic_stations/hardware.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/labware/bioer_96_wellplate_2000ul.json` & `covmatic-stations-3.0.4/covmatic_stations/labware/bioer_96_wellplate_2000ul.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/labware/biofil_1_reservoir_500000ul.json` & `covmatic-stations-3.0.4/covmatic_stations/labware/biofil_1_reservoir_500000ul.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/labware/biofil_3_reservoir_200000ul.json` & `covmatic-stations-3.0.4/covmatic_stations/labware/biofil_3_reservoir_200000ul.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/lights.py` & `covmatic-stations-3.0.4/covmatic_stations/lights.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/movement_manager.py` & `covmatic-stations-3.0.4/covmatic_stations/movement_manager.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/msg/Station.json` & `covmatic-stations-3.0.4/covmatic_stations/msg/Station.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/multi_tube_source.py` & `covmatic-stations-3.0.4/covmatic_stations/multi_tube_source.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/request.py` & `covmatic-stations-3.0.4/covmatic_stations/request.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/sound_manager.py` & `covmatic-stations-3.0.4/covmatic_stations/sound_manager.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/sounds/alarm.mp3` & `covmatic-stations-3.0.4/covmatic_stations/sounds/alarm.mp3`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/sounds/beep.mp3` & `covmatic-stations-3.0.4/covmatic_stations/sounds/beep.mp3`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/sounds/beep2.mp3` & `covmatic-stations-3.0.4/covmatic_stations/sounds/beep2.mp3`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/sounds/finish.mp3` & `covmatic-stations-3.0.4/covmatic_stations/sounds/finish.mp3`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/covmatic_stations/station.py` & `covmatic-stations-3.0.4/covmatic_stations/station.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from . import __version__, __file__ as module_path
 
 from .movement_manager import MovementManager
 from .request import StationRESTServerThread, DEFAULT_REST_KWARGS
 from .sound_manager import SoundManager
 from .utils import ProtocolContextLoggingHandler, LocalWebServerLogger, DelayManager
 from .lights import Button, BlinkingLightHTTP, BlinkingLight
-from opentrons.protocol_api import ProtocolContext
+from opentrons.protocol_api import ProtocolContext, Well
 from opentrons.types import Point
 import opentrons.commands.types
 from abc import ABCMeta, abstractmethod
 from functools import wraps, partialmethod
 from itertools import chain, dropwhile
 from opentrons.types import Location
-from typing import Optional, Callable, Tuple
+from typing import Optional, Callable, Tuple, List
 import json
 import math
 import os
 import logging
 import time
 import signal
 
@@ -324,15 +324,15 @@
         """Count the number of used tips"""
         self._tip_log['count'] = {t: sum(map(lambda x: not x.has_tip, self._tip_log['tips'][t])) for t in self._tipracks().keys()}
 
     def _reset_tips(self):
         for key, tiprack in self._tip_log['tips'].items():
             self._reset_tips_in_tiprack(tiprack)
 
-    def _reset_tips_in_tiprack(self, tiprack):
+    def _reset_tips_in_tiprack(self, tiprack: List[Well]):
         for t in tiprack:
             t.has_tip = True
 
     def setup_tip_log(self):
         data_tip_status = {}
         if self._tip_track:
             self.logger.info(self.msg_format("tip info log", self._tip_log_filepath))
```

### Comparing `covmatic-stations-3.0.3/covmatic_stations/utils.py` & `covmatic-stations-3.0.4/covmatic_stations/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,18 @@
         else:
             remaining_height = self._volume / (self._well.length * self._well.width)
 
         remaining_height -= self._headroom_height
         final_height = max(remaining_height, self._min_height)
         return final_height
 
+    @property
+    def volume(self) -> float:
+        return self._volume
+
     def extract_vol_and_get_height(self, aspirate_vol: float) -> float:
         """Return the maximum height to aspirate safely a volume from a well
         :param aspirate_vol: The volume to aspirate
         :returns: the maximum height to aspirate safely the volume in the well"""
         self._volume = self._volume - aspirate_vol if self._volume > aspirate_vol else 0
 
         return self.height
```

### Comparing `covmatic-stations-3.0.3/covmatic_stations.egg-info/PKG-INFO` & `covmatic-stations-3.0.4/covmatic_stations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covmatic-stations
-Version: 3.0.3
+Version: 3.0.4
 Summary: Package for the COVMATIC Opentrons stations
 Home-page: https://github.com/covmatic/stations
 Author: Marco Tiraboschi
 Author-email: marco.tiraboschi@unimi.it
 Maintainer: Marco Tiraboschi, Agostino Facotti, Giada Facoetti
 Maintainer-email: marco.tiraboschi@unimi.it, agostino.facotti@gmail.com, giada.facoetti@hotmail.it
 License: UNKNOWN
```

### Comparing `covmatic-stations-3.0.3/covmatic_stations.egg-info/SOURCES.txt` & `covmatic-stations-3.0.4/covmatic_stations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.3/setup.py` & `covmatic-stations-3.0.4/setup.py`

 * *Files identical despite different names*

