# Comparing `tmp/instamatic-1.8.0.tar.gz` & `tmp/instamatic-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instamatic-1.8.0.tar", last modified: Thu Mar 16 20:38:47 2023, max compression
+gzip compressed data, was "instamatic-1.9.0.tar", last modified: Fri May 19 06:34:15 2023, max compression
```

## Comparing `instamatic-1.8.0.tar` & `instamatic-1.9.0.tar`

### file list

```diff
@@ -1,250 +1,252 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.831971 instamatic-1.8.0/
--rw-rw-rw-   0        0        0     1790 2023-03-13 19:34:48.000000 instamatic-1.8.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1548 2022-11-07 08:27:17.000000 instamatic-1.8.0/LICENCE
--rw-rw-rw-   0        0        0      895 2023-03-13 19:09:51.000000 instamatic-1.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7400 2023-03-16 20:38:47.832970 instamatic-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      837 2021-08-09 14:43:18.000000 instamatic-1.8.0/THANKS.md
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.469569 instamatic-1.8.0/docs/
--rw-rw-rw-   0        0        0     4423 2023-03-13 19:38:15.000000 instamatic-1.8.0/docs/conf.py
--rw-rw-rw-   0        0        0    14104 2021-07-13 11:13:19.000000 instamatic-1.8.0/docs/config.md
--rw-rw-rw-   0        0        0     1816 2021-07-13 11:13:19.000000 instamatic-1.8.0/docs/formats.md
--rw-rw-rw-   0        0        0     8498 2021-07-13 11:13:20.000000 instamatic-1.8.0/docs/gui.md
--rw-rw-rw-   0        0        0     2817 2021-07-13 11:13:20.000000 instamatic-1.8.0/docs/make_programs_md.py
--rw-rw-rw-   0        0        0    21110 2021-08-03 11:25:30.000000 instamatic-1.8.0/docs/programs.md
--rw-rw-rw-   0        0        0     4846 2021-07-13 11:13:20.000000 instamatic-1.8.0/docs/setup.md
--rw-rw-rw-   0        0        0     8978 2021-07-13 11:13:20.000000 instamatic-1.8.0/docs/tem_api.md
--rw-rw-rw-   0        0        0     4767 2021-07-13 11:13:20.000000 instamatic-1.8.0/docs/tvips.md
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.494570 instamatic-1.8.0/instamatic/
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.544578 instamatic-1.8.0/instamatic/TEMController/
--rw-rw-rw-   0        0        0    24733 2021-08-03 12:59:57.000000 instamatic-1.8.0/instamatic/TEMController/TEMController.py
--rw-rw-rw-   0        0        0      116 2021-08-03 13:11:53.000000 instamatic-1.8.0/instamatic/TEMController/__init__.py
--rw-rw-rw-   0        0        0     3080 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/TEMController/deflectors.py
--rw-rw-rw-   0        0        0    15874 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/TEMController/fei_microscope.py
--rw-rw-rw-   0        0        0    12301 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/TEMController/fei_simu_microscope.py
--rw-rw-rw-   0        0        0    19470 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/TEMController/jeol_microscope.py
--rw-rw-rw-   0        0        0     4153 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/TEMController/lenses.py
--rw-rw-rw-   0        0        0     1806 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/TEMController/microscope.py
--rw-rw-rw-   0        0        0     4675 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/TEMController/microscope_client.py
--rw-rw-rw-   0        0        0    17132 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/TEMController/simu_microscope.py
--rw-rw-rw-   0        0        0    10893 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/TEMController/stage.py
--rw-rw-rw-   0        0        0     3298 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/TEMController/states.py
--rw-rw-rw-   0        0        0     1364 2023-03-13 19:38:15.000000 instamatic-1.8.0/instamatic/__init__.py
--rw-rw-rw-   0        0        0     6002 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/acquire_at_items.py
--rw-rw-rw-   0        0        0      313 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/admin.py
--rw-rw-rw-   0        0        0      602 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/banner.py
--rw-rw-rw-   0        0        0     6216 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/browser.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.566100 instamatic-1.8.0/instamatic/calibrate/
--rw-rw-rw-   0        0        0      246 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/calibrate/__init__.py
--rw-rw-rw-   0        0        0    10873 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/calibrate/calibrate_beamshift.py
--rw-rw-rw-   0        0        0     6044 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/calibrate/calibrate_brightness.py
--rw-rw-rw-   0        0        0    12312 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/calibrate/calibrate_directbeam.py
--rw-rw-rw-   0        0        0     3416 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/calibrate/calibrate_imageshift12.py
--rw-rw-rw-   0        0        0    13872 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/calibrate/calibrate_stage_lowmag.py
--rw-rw-rw-   0        0        0     8757 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/calibrate/calibrate_stage_mag1.py
--rw-rw-rw-   0        0        0    16162 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/calibrate/calibrate_stagematrix.py
--rw-rw-rw-   0        0        0     6536 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/calibrate/center_z.py
--rw-rw-rw-   0        0        0      477 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/calibrate/filenames.py
--rw-rw-rw-   0        0        0     3181 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/calibrate/fit.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.610096 instamatic-1.8.0/instamatic/camera/
--rw-rw-rw-   0        0        0     1237 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/camera/CCDCOM.h
--rw-rw-rw-   0        0        0    22528 2018-08-07 11:46:26.000000 instamatic-1.8.0/instamatic/camera/CCDCOM2_x64_gatan.dll
--rw-rw-rw-   0        0        0    10752 2016-05-18 16:01:08.000000 instamatic-1.8.0/instamatic/camera/CCDCOM2_x64_simulation.dll
--rw-rw-rw-   0        0        0    17920 2019-05-08 11:55:23.000000 instamatic-1.8.0/instamatic/camera/CCDCOM2_x86_gatan.dll
--rw-rw-rw-   0        0        0     8704 2016-05-18 11:17:54.000000 instamatic-1.8.0/instamatic/camera/CCDCOM2_x86_simulation.dll
--rw-rw-rw-   0        0        0    55808 2018-04-13 10:02:59.000000 instamatic-1.8.0/instamatic/camera/EMCameraObj.dll
--rw-rw-rw-   0        0        0       64 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/camera/__init__.py
--rw-rw-rw-   0        0        0     6560 2021-08-09 14:43:06.000000 instamatic-1.8.0/instamatic/camera/camera.py
--rw-rw-rw-   0        0        0     5697 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/camera/camera_client.py
--rw-rw-rw-   0        0        0    18920 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/camera/camera_emmenu.py
--rw-rw-rw-   0        0        0     8190 2021-08-03 11:25:27.000000 instamatic-1.8.0/instamatic/camera/camera_gatan.py
--rw-rw-rw-   0        0        0     6466 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/camera/camera_gatan2.py
--rw-rw-rw-   0        0        0     5161 2021-08-09 14:43:06.000000 instamatic-1.8.0/instamatic/camera/camera_serval.py
--rw-rw-rw-   0        0        0     4689 2021-08-03 13:11:54.000000 instamatic-1.8.0/instamatic/camera/camera_simu.py
--rw-rw-rw-   0        0        0    10695 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/camera/camera_timepix.py
--rw-rw-rw-   0        0        0     3062 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/camera/fakevideostream.py
--rw-rw-rw-   0        0        0     3001 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/camera/gatansocket3.md
--rw-rw-rw-   0        0        0    26641 2021-08-09 14:43:06.000000 instamatic-1.8.0/instamatic/camera/gatansocket3.py
--rw-rw-rw-   0        0        0  1231360 2016-11-11 15:54:14.000000 instamatic-1.8.0/instamatic/camera/mpxhwrelaxd.dll
--rw-rw-rw-   0        0        0        0 2019-05-08 11:55:23.000000 instamatic-1.8.0/instamatic/camera/timepix.lockfile
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.619096 instamatic-1.8.0/instamatic/camera/tpx/
--rw-rw-rw-   0        0        0   262144 2017-12-13 12:38:26.000000 instamatic-1.8.0/instamatic/camera/tpx/171207_with_flatfield.bpc
--rw-rw-rw-   0        0        0      608 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/camera/tpx/171207_with_flatfield.bpc.dacs
--rw-rw-rw-   0        0        0      246 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/camera/tpx/HW.dacs
--rw-rw-rw-   0        0        0       98 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/camera/tpx/config.txt
--rw-rw-rw-   0        0        0     6151 2021-08-09 14:43:06.000000 instamatic-1.8.0/instamatic/camera/videostream.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.629097 instamatic-1.8.0/instamatic/config/
--rw-rw-rw-   0        0        0     8213 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.631096 instamatic-1.8.0/instamatic/config/alignments/
--rw-rw-rw-   0        0        0      308 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/alignments/neutral.yaml
--rw-rw-rw-   0        0        0     5746 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/autoconfig.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.639096 instamatic-1.8.0/instamatic/config/calibration/
--rw-rw-rw-   0        0        0     1377 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/calibration/orius.yaml
--rw-rw-rw-   0        0        0     1525 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/calibration/simulate.yaml
--rw-rw-rw-   0        0        0      777 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/calibration/timepix.yaml
--rw-rw-rw-   0        0        0     2336 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/calibration/tvips-f416.yaml
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.652105 instamatic-1.8.0/instamatic/config/camera/
--rw-rw-rw-   0        0        0      348 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/camera/orius.yaml
--rw-rw-rw-   0        0        0      602 2021-08-09 14:43:06.000000 instamatic-1.8.0/instamatic/config/camera/serval.yaml
--rw-rw-rw-   0        0        0      394 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/camera/simulate.yaml
--rw-rw-rw-   0        0        0      352 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/camera/simulateDLL.yaml
--rw-rw-rw-   0        0        0      417 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/camera/timepix.yaml
--rw-rw-rw-   0        0        0      399 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/camera/tvips-f416.yaml
--rw-rw-rw-   0        0        0      395 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/camera/tvips-xf416.yaml
--rw-rw-rw-   0        0        0     2686 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/config_updater.py
--rw-rw-rw-   0        0        0      317 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/defaults.yaml
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.660628 instamatic-1.8.0/instamatic/config/microscope/
--rw-rw-rw-   0        0        0      529 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/microscope/fei_simu.yaml
--rw-rw-rw-   0        0        0      524 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/microscope/fei_themisZ.yaml
--rw-rw-rw-   0        0        0      954 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/microscope/jeol-1400.yaml
--rw-rw-rw-   0        0        0      525 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/microscope/jeol.yaml
--rw-rw-rw-   0        0        0      529 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/microscope/simulate.yaml
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.662626 instamatic-1.8.0/instamatic/config/scripts/
--rw-rw-rw-   0        0        0      606 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/scripts/readme.md
--rw-rw-rw-   0        0        0     1807 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/settings.yaml
--rw-rw-rw-   0        0        0     1408 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/config/utils.py
--rw-rw-rw-   0        0        0     1261 2021-08-03 11:25:30.000000 instamatic-1.8.0/instamatic/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.664629 instamatic-1.8.0/instamatic/experiments/
--rw-rw-rw-   0        0        0      216 2021-08-03 13:11:55.000000 instamatic-1.8.0/instamatic/experiments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.667624 instamatic-1.8.0/instamatic/experiments/autocred/
--rw-rw-rw-   0        0        0        0 2018-08-01 08:33:35.000000 instamatic-1.8.0/instamatic/experiments/autocred/__init__.py
--rw-rw-rw-   0        0        0    66171 2021-08-09 14:43:06.000000 instamatic-1.8.0/instamatic/experiments/autocred/experiment.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.670623 instamatic-1.8.0/instamatic/experiments/cred/
--rw-rw-rw-   0        0        0        0 2018-08-01 08:33:35.000000 instamatic-1.8.0/instamatic/experiments/cred/__init__.py
--rw-rw-rw-   0        0        0    17624 2021-08-03 13:11:56.000000 instamatic-1.8.0/instamatic/experiments/cred/experiment.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.674626 instamatic-1.8.0/instamatic/experiments/cred_gatan/
--rw-rw-rw-   0        0        0        0 2020-01-23 13:36:43.000000 instamatic-1.8.0/instamatic/experiments/cred_gatan/__init__.py
--rw-rw-rw-   0        0        0    16301 2021-08-03 13:11:57.000000 instamatic-1.8.0/instamatic/experiments/cred_gatan/experiment.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.676624 instamatic-1.8.0/instamatic/experiments/cred_tvips/
--rw-rw-rw-   0        0        0        0 2019-08-13 08:34:08.000000 instamatic-1.8.0/instamatic/experiments/cred_tvips/__init__.py
--rw-rw-rw-   0        0        0    21342 2021-08-03 13:11:57.000000 instamatic-1.8.0/instamatic/experiments/cred_tvips/experiment.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.680634 instamatic-1.8.0/instamatic/experiments/red/
--rw-rw-rw-   0        0        0        0 2018-08-01 08:33:35.000000 instamatic-1.8.0/instamatic/experiments/red/__init__.py
--rw-rw-rw-   0        0        0     8429 2021-08-03 13:11:58.000000 instamatic-1.8.0/instamatic/experiments/red/experiment.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.683625 instamatic-1.8.0/instamatic/experiments/serialed/
--rw-rw-rw-   0        0        0        0 2018-08-01 08:33:35.000000 instamatic-1.8.0/instamatic/experiments/serialed/__init__.py
--rw-rw-rw-   0        0        0    22642 2021-08-09 14:43:06.000000 instamatic-1.8.0/instamatic/experiments/serialed/experiment.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.694625 instamatic-1.8.0/instamatic/formats/
--rw-rw-rw-   0        0        0     3593 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/formats/__init__.py
--rw-rw-rw-   0        0        0     3864 2021-08-09 14:43:06.000000 instamatic-1.8.0/instamatic/formats/adscimage.py
--rw-rw-rw-   0        0        0     2221 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/formats/csvIO.py
--rw-rw-rw-   0        0        0    23476 2021-08-09 14:43:06.000000 instamatic-1.8.0/instamatic/formats/mrc.py
--rw-rw-rw-   0        0        0     3222 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/formats/util.py
--rw-rw-rw-   0        0        0     4505 2021-08-09 14:43:06.000000 instamatic-1.8.0/instamatic/formats/xdscbf.py
--rw-rw-rw-   0        0        0     6011 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/goniotool.py
--rw-rw-rw-   0        0        0     7007 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/gridmontage.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.729626 instamatic-1.8.0/instamatic/gui/
--rw-rw-rw-   0        0        0       27 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/gui/__init__.py
--rw-rw-rw-   0        0        0     4777 2021-08-09 14:43:18.000000 instamatic-1.8.0/instamatic/gui/about_frame.py
--rw-rw-rw-   0        0        0    14836 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/gui/autocred_frame.py
--rw-rw-rw-   0        0        0      836 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/gui/base_module.py
--rw-rw-rw-   0        0        0     5187 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/gui/console_frame.py
--rw-rw-rw-   0        0        0     4523 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/gui/cred_fei_frame.py
--rw-rw-rw-   0        0        0    10229 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/gui/cred_frame.py
--rw-rw-rw-   0        0        0    13897 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/gui/cred_tvips_frame.py
--rw-rw-rw-   0        0        0    11527 2021-07-13 11:13:20.000000 instamatic-1.8.0/instamatic/gui/ctrl_frame.py
--rw-rw-rw-   0        0        0    14999 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/gui/debug_frame.py
--rw-rw-rw-   0        0        0     2588 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/gui/defocus_button.py
--rw-rw-rw-   0        0        0     5284 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/gui/gui.py
--rw-rw-rw-   0        0        0     5619 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/gui/io_frame.py
--rw-rw-rw-   0        0        0     2208 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/gui/jobs.py
--rw-rw-rw-   0        0        0     6279 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/gui/machine_learning_frame.py
--rw-rw-rw-   0        0        0     1301 2021-08-03 11:25:30.000000 instamatic-1.8.0/instamatic/gui/modules.py
--rw-rw-rw-   0        0        0     1096 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/gui/mpl_frame.py
--rw-rw-rw-   0        0        0     5585 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/gui/red_frame.py
--rw-rw-rw-   0        0        0     7026 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/gui/sed_frame.py
--rw-rw-rw-   0        0        0    10064 2021-08-09 14:43:06.000000 instamatic-1.8.0/instamatic/gui/videostream_frame.py
--rw-rw-rw-   0        0        0     2876 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/image_utils.py
--rw-rw-rw-   0        0        0     1353 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/imreg.py
--rw-rw-rw-   0        0        0      922 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/io.py
--rw-rw-rw-   0        0        0     4908 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/main.py
--rw-rw-rw-   0        0        0     2223 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/montage.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.740627 instamatic-1.8.0/instamatic/neural_network/
--rw-rw-rw-   0        0        0       71 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/neural_network/__init__.py
--rw-rw-rw-   0        0        0     2073 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/neural_network/neural_network.py
--rw-rw-rw-   0        0        0      972 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/neural_network/preprocess.py
--rw-rw-rw-   0        0        0      738 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/neural_network/preprocess_SerialRED.py
--rw-rw-rw-   0        0        0  1503408 2017-11-29 12:53:48.000000 instamatic-1.8.0/instamatic/neural_network/weights-py2.p
--rw-rw-rw-   0        0        0  1020951 2017-11-29 12:53:48.000000 instamatic-1.8.0/instamatic/neural_network/weights-py3.p
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.763973 instamatic-1.8.0/instamatic/processing/
--rw-rw-rw-   0        0        0    27647 2023-01-17 16:33:23.000000 instamatic-1.8.0/instamatic/processing/ImgConversion.py
--rw-rw-rw-   0        0        0     2997 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/processing/ImgConversionDM.py
--rw-rw-rw-   0        0        0     3598 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/processing/ImgConversionTPX.py
--rw-rw-rw-   0        0        0     3017 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/processing/ImgConversionTVIPS.py
--rw-rw-rw-   0        0        0     5077 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/processing/XDS_template.py
--rw-rw-rw-   0        0        0     5077 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/processing/XDS_templateDM.py
--rw-rw-rw-   0        0        0     5077 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/processing/XDS_templateTPX.py
--rw-rw-rw-   0        0        0     5077 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/processing/XDS_templateTVIPS.py
--rw-rw-rw-   0        0        0      151 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/processing/__init__.py
--rw-rw-rw-   0        0        0     7643 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/processing/find_crystals.py
--rw-rw-rw-   0        0        0     5829 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/processing/find_crystals_ilastik.py
--rw-rw-rw-   0        0        0     6486 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/processing/find_holes.py
--rw-rw-rw-   0        0        0     7959 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/processing/flatfield.py
--rw-rw-rw-   0        0        0     7966 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/processing/stretch_correction.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.778970 instamatic-1.8.0/instamatic/server/
--rw-rw-rw-   0        0        0     2375 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/server/TEMServer_FEI.py
--rw-rw-rw-   0        0        0        0 2019-11-05 15:27:03.000000 instamatic-1.8.0/instamatic/server/__init__.py
--rw-rw-rw-   0        0        0      327 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/server/cam_client.py
--rw-rw-rw-   0        0        0     7126 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/server/cam_server.py
--rw-rw-rw-   0        0        0     3728 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/server/dials_server.py
--rw-rw-rw-   0        0        0     4687 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/server/goniotool_server.py
--rw-rw-rw-   0        0        0     1483 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/server/serializer.py
--rw-rw-rw-   0        0        0      364 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/server/tem_client.py
--rw-rw-rw-   0        0        0     5552 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/server/tem_server.py
--rw-rw-rw-   0        0        0    10931 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/server/vm_ubuntu_server.py
--rw-rw-rw-   0        0        0     3609 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/server/xds_server.py
--rw-rw-rw-   0        0        0     8940 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/tools.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.788969 instamatic-1.8.0/instamatic/utils/
--rw-rw-rw-   0        0        0      268 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/utils/__init__.py
--rw-rw-rw-   0        0        0     6602 2021-08-09 14:43:06.000000 instamatic-1.8.0/instamatic/utils/beamstop.py
--rw-rw-rw-   0        0        0     1417 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/utils/high_precision_timers.py
--rw-rw-rw-   0        0        0     1844 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/utils/progress.py
--rw-rw-rw-   0        0        0      270 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/utils/singleton.py
--rw-rw-rw-   0        0        0      836 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/utils/spinbox.py
--rw-rw-rw-   0        0        0     8560 2021-07-13 11:13:21.000000 instamatic-1.8.0/instamatic/utils/xds_parser.py
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.520568 instamatic-1.8.0/instamatic.egg-info/
--rw-rw-rw-   0        0        0     7400 2023-03-16 20:38:47.000000 instamatic-1.8.0/instamatic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7017 2023-03-16 20:38:47.000000 instamatic-1.8.0/instamatic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 20:38:47.000000 instamatic-1.8.0/instamatic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1680 2023-03-16 20:38:47.000000 instamatic-1.8.0/instamatic.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-01-17 16:07:30.000000 instamatic-1.8.0/instamatic.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      381 2023-03-16 20:38:47.000000 instamatic-1.8.0/instamatic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-16 20:38:47.000000 instamatic-1.8.0/instamatic.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.795972 instamatic-1.8.0/notebooks/
--rw-rw-rw-   0        0        0     8484 2021-08-03 11:25:30.000000 instamatic-1.8.0/notebooks/data_collection.ipynb
--rw-rw-rw-   0        0        0     4339 2021-08-03 11:25:30.000000 instamatic-1.8.0/notebooks/grid_montage_collection.ipynb
--rw-rw-rw-   0        0        0    13563 2021-08-03 11:25:30.000000 instamatic-1.8.0/notebooks/montage_processing.ipynb
--rw-rw-rw-   0        0        0    12418 2021-08-03 11:25:30.000000 instamatic-1.8.0/notebooks/nav.nav
--rw-rw-rw-   0        0        0      458 2021-08-09 14:49:27.000000 instamatic-1.8.0/notebooks/readme.md
--rw-rw-rw-   0        0        0      101 2023-03-13 19:09:51.000000 instamatic-1.8.0/pyproject.toml
--rw-rw-rw-   0        0        0      276 2021-07-13 11:13:21.000000 instamatic-1.8.0/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.813971 instamatic-1.8.0/scripts/
--rw-rw-rw-   0        0        0        0 2019-05-07 12:26:02.000000 instamatic-1.8.0/scripts/__init__.py
--rw-rw-rw-   0        0        0     8454 2021-08-09 14:43:06.000000 instamatic-1.8.0/scripts/browser.py
--rw-rw-rw-   0        0        0     2204 2021-07-13 11:13:21.000000 instamatic-1.8.0/scripts/center_images_smv.py
--rw-rw-rw-   0        0        0     4170 2021-07-13 11:13:21.000000 instamatic-1.8.0/scripts/diagnose_beam_drift.py
--rw-rw-rw-   0        0        0     4710 2021-08-09 14:43:06.000000 instamatic-1.8.0/scripts/learn.py
--rw-rw-rw-   0        0        0     1522 2021-07-13 11:13:21.000000 instamatic-1.8.0/scripts/make_interval_movie.py
--rw-rw-rw-   0        0        0     2417 2021-07-13 11:13:21.000000 instamatic-1.8.0/scripts/make_serialed_movie.py
--rw-rw-rw-   0        0        0     6277 2021-07-13 11:13:21.000000 instamatic-1.8.0/scripts/process_dm.py
--rw-rw-rw-   0        0        0     6500 2021-07-13 11:13:21.000000 instamatic-1.8.0/scripts/process_tpx.py
--rw-rw-rw-   0        0        0     9069 2023-01-17 16:33:23.000000 instamatic-1.8.0/scripts/process_tvips.py
--rw-rw-rw-   0        0        0     1218 2021-07-13 11:13:21.000000 instamatic-1.8.0/scripts/viewer.py
--rw-rw-rw-   0        0        0     3590 2023-03-16 20:38:47.834968 instamatic-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-03-13 19:09:51.000000 instamatic-1.8.0/setup.py
--rwxrwxrwx   0        0        0       41 2021-07-13 11:13:21.000000 instamatic-1.8.0/setup_win.bat
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.822975 instamatic-1.8.0/tests/
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.825976 instamatic-1.8.0/tests/config/
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.827971 instamatic-1.8.0/tests/config/calibration/
--rw-rw-rw-   0        0        0     1525 2021-07-13 11:13:21.000000 instamatic-1.8.0/tests/config/calibration/test.yaml
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.829975 instamatic-1.8.0/tests/config/camera/
--rw-rw-rw-   0        0        0      244 2021-07-13 11:13:21.000000 instamatic-1.8.0/tests/config/camera/test.yaml
--rw-rw-rw-   0        0        0      230 2021-07-13 11:13:21.000000 instamatic-1.8.0/tests/config/defaults.yaml
-drwxrwxrwx   0        0        0        0 2023-03-16 20:38:47.830969 instamatic-1.8.0/tests/config/microscope/
--rw-rw-rw-   0        0        0      529 2021-07-13 11:13:21.000000 instamatic-1.8.0/tests/config/microscope/test.yaml
--rw-rw-rw-   0        0        0      418 2021-07-13 11:13:21.000000 instamatic-1.8.0/tests/config/settings.yaml
--rw-rw-rw-   0        0        0      365 2021-07-13 11:13:21.000000 instamatic-1.8.0/tests/conftest.py
--rw-rw-rw-   0        0        0      502 2021-07-13 11:13:21.000000 instamatic-1.8.0/tests/test_camera.py
--rw-rw-rw-   0        0        0     4996 2023-03-13 19:09:51.000000 instamatic-1.8.0/tests/test_ctrl.py
--rw-rw-rw-   0        0        0     1821 2021-08-03 13:12:07.000000 instamatic-1.8.0/tests/test_experiments.py
--rw-rw-rw-   0        0        0     1485 2021-07-13 11:13:21.000000 instamatic-1.8.0/tests/test_formats.py
--rw-rw-rw-   0        0        0      123 2021-07-13 11:13:21.000000 instamatic-1.8.0/tests/test_grid_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.033219 instamatic-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-19 06:33:59.000000 instamatic-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-19 06:33:59.000000 instamatic-1.9.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-19 06:33:59.000000 instamatic-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-19 06:34:15.033219 instamatic-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-19 06:33:59.000000 instamatic-1.9.0/THANKS.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:14.997219 instamatic-1.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/formats.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/gui.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/make_programs_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20542 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/programs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/setup.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/tem_api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/tvips.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:14.997219 instamatic-1.9.0/instamatic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.001219 instamatic-1.9.0/instamatic/TEMController/
+-rw-r--r--   0 runner    (1001) docker     (123)    24729 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/TEMController.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/deflectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15842 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/fei_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/fei_simu_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19453 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/jeol_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/lenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/microscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/microscope_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/simu_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/acquire_at_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/banner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.001219 instamatic-1.9.0/instamatic/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_beamshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_directbeam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_imageshift12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_stage_lowmag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_stage_mag1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16127 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_stagematrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/center_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/filenames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.009219 instamatic-1.9.0/instamatic/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/CCDCOM.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22528 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/CCDCOM2_x64_gatan.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/CCDCOM2_x64_simulation.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/CCDCOM2_x86_gatan.dll
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/CCDCOM2_x86_simulation.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    55808 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/EMCameraObj.dll
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_emmenu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_gatan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_gatan2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_merlin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_serval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_simu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_timepix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/fakevideostream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/gatansocket3.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/gatansocket3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/merlin_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1231360 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/mpxhwrelaxd.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/timepix.lockfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.009219 instamatic-1.9.0/instamatic/camera/tpx/
+-rw-r--r--   0 runner    (1001) docker     (123)   262144 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/tpx/171207_with_flatfield.bpc
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/tpx/171207_with_flatfield.bpc.dacs
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/tpx/HW.dacs
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/tpx/config.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/videostream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.009219 instamatic-1.9.0/instamatic/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/config/alignments/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/alignments/neutral.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/autoconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/config/calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/calibration/orius.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/calibration/simulate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/calibration/timepix.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/calibration/tvips-f416.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/config/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/merlin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/orius.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/serval.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/simulate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/simulateDLL.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/timepix.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/tvips-f416.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/tvips-xf416.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/config_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/defaults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/config/microscope/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/microscope/fei_simu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/microscope/fei_themisZ.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/microscope/jeol-1400.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/microscope/jeol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/microscope/simulate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/config/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/scripts/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/experiments/autocred/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/autocred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64484 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/autocred/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/experiments/cred/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/cred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/cred/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.017219 instamatic-1.9.0/instamatic/experiments/cred_gatan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/cred_gatan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15867 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/cred_gatan/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.017219 instamatic-1.9.0/instamatic/experiments/cred_tvips/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/cred_tvips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/cred_tvips/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.017219 instamatic-1.9.0/instamatic/experiments/red/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/red/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/red/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.017219 instamatic-1.9.0/instamatic/experiments/serialed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/serialed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21939 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/serialed/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.017219 instamatic-1.9.0/instamatic/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/formats/adscimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/formats/csvIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22681 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/formats/mrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/formats/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/formats/xdscbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/goniotool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gridmontage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.021219 instamatic-1.9.0/instamatic/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/about_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/autocred_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/console_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/cred_fei_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/cred_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/cred_tvips_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/ctrl_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/debug_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/defocus_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/io_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/machine_learning_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/mpl_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/red_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/sed_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/videostream_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/imreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/montage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.021219 instamatic-1.9.0/instamatic/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/neural_network/neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/neural_network/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/neural_network/preprocess_SerialRED.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.025219 instamatic-1.9.0/instamatic/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    26808 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/ImgConversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/ImgConversionDM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/ImgConversionTPX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/ImgConversionTVIPS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/XDS_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/XDS_templateDM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/XDS_templateTPX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/XDS_templateTVIPS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/find_crystals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/find_crystals_ilastik.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/find_holes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/flatfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/stretch_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.025219 instamatic-1.9.0/instamatic/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/TEMServer_FEI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/cam_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/cam_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/dials_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/goniotool_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/tem_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/tem_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/vm_ubuntu_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/xds_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.025219 instamatic-1.9.0/instamatic/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/beamstop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/high_precision_timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/xds_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.001219 instamatic-1.9.0/instamatic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.029219 instamatic-1.9.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-05-19 06:33:59.000000 instamatic-1.9.0/notebooks/data_collection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-19 06:33:59.000000 instamatic-1.9.0/notebooks/grid_montage_collection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13148 2023-05-19 06:33:59.000000 instamatic-1.9.0/notebooks/montage_processing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-05-19 06:33:59.000000 instamatic-1.9.0/notebooks/nav.nav
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-19 06:33:59.000000 instamatic-1.9.0/notebooks/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-19 06:33:59.000000 instamatic-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-19 06:33:59.000000 instamatic-1.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.029219 instamatic-1.9.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/center_images_smv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/diagnose_beam_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/learn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/make_interval_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/make_serialed_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/process_dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/process_tpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/process_tvips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-19 06:34:15.033219 instamatic-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 06:33:59.000000 instamatic-1.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-19 06:33:59.000000 instamatic-1.9.0/setup_win.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.029219 instamatic-1.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.029219 instamatic-1.9.0/tests/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.033219 instamatic-1.9.0/tests/config/calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/config/calibration/test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.033219 instamatic-1.9.0/tests/config/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/config/camera/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/config/defaults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.033219 instamatic-1.9.0/tests/config/microscope/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/config/microscope/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/config/settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/test_ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/test_grid_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/test_merlin_io.py
```

### Comparing `instamatic-1.8.0/LICENCE` & `instamatic-1.9.0/LICENCE`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2021, Stef Smeets
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2021, Stef Smeets
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `instamatic-1.8.0/MANIFEST.in` & `instamatic-1.9.0/MANIFEST.in`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-include .pre-commit-config.yaml
-include THANKS.md
-include LICENCE
-include notebooks/*.ipynb
-include notebooks/nav.nav
-include notebooks/readme.md
-include docs/*.md
-include docs/*.png
-include docs/*.py
-include requirements.txt
-include scripts/*.py
-include setup_win.bat
-include tests/*.py
-include tests/config/*.yaml
-include tests/config/*/*.yaml
-include instamatic/camera/*.dll
-include instamatic/camera/*.h
-include instamatic/camera/*.lockfile
-include instamatic/camera/*.md
-include instamatic/camera/tpx/*.bpc
-include instamatic/camera/tpx/*.dacs
-include instamatic/camera/tpx/*.txt
-include instamatic/config/*.yaml
-include instamatic/config/alignments/*.yaml
-include instamatic/config/calibration/*.yaml
-include instamatic/config/camera/*.yaml
-include instamatic/config/microscope/*.yaml
-include instamatic/config/scripts/*.md
-include instamatic.neural_network/*.p
+include .pre-commit-config.yaml
+include THANKS.md
+include LICENCE
+include notebooks/*.ipynb
+include notebooks/nav.nav
+include notebooks/readme.md
+include docs/*.md
+include docs/*.png
+include docs/*.py
+include requirements.txt
+include scripts/*.py
+include setup_win.bat
+include tests/*.py
+include tests/config/*.yaml
+include tests/config/*/*.yaml
+include instamatic/camera/*.dll
+include instamatic/camera/*.h
+include instamatic/camera/*.lockfile
+include instamatic/camera/*.md
+include instamatic/camera/tpx/*.bpc
+include instamatic/camera/tpx/*.dacs
+include instamatic/camera/tpx/*.txt
+include instamatic/config/*.yaml
+include instamatic/config/alignments/*.yaml
+include instamatic/config/calibration/*.yaml
+include instamatic/config/camera/*.yaml
+include instamatic/config/microscope/*.yaml
+include instamatic/config/scripts/*.md
+include instamatic.neural_network/*.p
```

### Comparing `instamatic-1.8.0/THANKS.md` & `instamatic-1.9.0/THANKS.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Code contributors
------------------
-
-See [Github contributors list](https://github.com/nipy/nipype/graphs/contributors)
-
-Special thanks
---------------
-
-- Magdalena O. Cichocka
-  - Testing and feedback on cRED implementation
-
-- Jonas Ångström
-  - Neural network implementation
-  - Early scripts for data processing
-
-- Wei Wan
-  - DLLs for timepix/orius camera interface
-
-Funding
--------
-
-Development of `Instamatic` was supported by the Swiss National Science Foundation through the following projects:
-
-- 2016-2017: [Development of serial crystallography methods for structure solution of polycrystalline materials using electron diffraction](http://p3.snf.ch/project-165282)
-- 2018: [Development of serial electron crystallography methodology for quantitative phase analysis](http://p3.snf.ch/Project-177761)
+Code contributors
+-----------------
+
+See [Github contributors list](https://github.com/nipy/nipype/graphs/contributors)
+
+Special thanks
+--------------
+
+- Magdalena O. Cichocka
+  - Testing and feedback on cRED implementation
+
+- Jonas Ångström
+  - Neural network implementation
+  - Early scripts for data processing
+
+- Wei Wan
+  - DLLs for timepix/orius camera interface
+
+Funding
+-------
+
+Development of `Instamatic` was supported by the Swiss National Science Foundation through the following projects:
+
+- 2016-2017: [Development of serial crystallography methods for structure solution of polycrystalline materials using electron diffraction](http://p3.snf.ch/project-165282)
+- 2018: [Development of serial electron crystallography methodology for quantitative phase analysis](http://p3.snf.ch/Project-177761)
```

### Comparing `instamatic-1.8.0/docs/conf.py` & `instamatic-1.9.0/docs/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-import sys
-from pathlib import Path
-
-root = Path(__file__).absolute().parent.parent
-sys.path.insert(0, str(root))
-
-DOCSDIR = '.'
-BUILDDIR = '_build'
-TEMPLATESDIR = '_templates'
-STATICDIR = '_static'
-SOURCEDIR = '../instamatic'
-
-
-# -- Run apidoc plug-in manually, as readthedocs doesn't support it -------
-# See https://github.com/rtfd/readthedocs.org/issues/1139
-def run_apidoc(app):
-    ignore_paths = []
-
-    cmd = ('--separate --no-toc --force --module-first '
-           f'-t {TEMPLATESDIR} '
-           f'-o {DOCSDIR} '
-           f'{SOURCEDIR} ')
-
-    args = cmd.split() + ignore_paths
-
-    from sphinx.ext import apidoc
-    apidoc.main(args)
-
-
-# Convert readme.md and others to rst to be included in index.html
-def make_markdown(app):
-    import subprocess
-    for inp, out in (('setup.md', 'setup.rst'),
-                     ('config.md', 'config.rst'),
-                     ('formats.md', 'formats.rst'),
-                     ('gui.md', 'gui.rst'),
-                     ('programs.md', 'programs.rst'),
-                     ('tem_api.md', 'tem_api.rst'),
-                     ('tvips.md', 'tvips.rst'),
-                     ('../readme.md', 'readme.rst')):
-        cmd = f'pandoc --from=markdown --to=rst --output={out} {inp}'
-        args = cmd.split()
-        subprocess.run(args)
-
-
-# https://www.sphinx-doc.org/en/master/extdev/appapi.html#sphinx-core-events
-# https://github.com/readthedocs/readthedocs.org/issues/2276
-def setup(app):
-    app.connect('builder-inited', make_markdown)
-    app.connect('builder-inited', run_apidoc)
-
-
-extensions = [
-    'sphinx.ext.autodoc',
-    # 'sphinx.ext.coverage',
-    # 'sphinx.ext.doctest',
-    # 'sphinx.ext.intersphinx',
-    # 'sphinx.ext.mathjax',
-    'sphinx.ext.napoleon',
-    'nbsphinx',
-    'nbsphinx_link',
-    # 'sphinx.ext.todo',
-    # 'sphinx.ext.viewcode',
-    'autodocsumm',
-]
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
-
-# The suffix(es) of source filenames.
-# You can specify multiple suffix as a list of string:
-source_suffix = ['.rst', '.md']
-
-# The master toctree document.
-master_doc = 'index'
-
-# General information about the project.
-project = 'instamatic'
-copyright = '2021, '
-author = 'Stef Smeets'
-
-# The short X.Y version.
-version = release = '1.8.0'
-
-# The language for content autogenerated by Sphinx.
-language = 'english'
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = [BUILDDIR, 'Thumbs.db', '.DS_Store']
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = [STATICDIR]
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = False
-
-# Use autoapi.extension to run sphinx-apidoc
-autoapi_dirs = [SOURCEDIR]
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-html_theme = 'sphinx_rtd_theme'
-# options for rtd-theme
-# html_theme_options = {
-#     'display_version': True,
-#     'prev_next_buttons_location': 'bottom',
-#     'style_external_links': False,
-#     # toc options
-#     'collapse_navigation': True,
-#     'sticky_navigation': True,
-#     'navigation_depth': 4,
-#     'includehidden': True,
-#     'titles_only': False,
-# }
-
-autodoc_default_options = {
-    'autosummary': True,
-    'special-members': '__init__',
-}
-
-nbsphinx_allow_errors = True
-nbsphinx_execute = 'never'
-
-autodoc_mock_imports = [
-    'h5py',
-    'virtualbox',
-    'pywinauto',
-    'pyserialem',
-    'predicrystal',
-    'lmfit',
-    'mrcfile',
-    'comtypes',
-    'msvcrt',
-]
-
-intersphinx_mapping = {
-    'python': ('https://docs.python.org/3', None),
-    'numpy': ('https://docs.scipy.org/doc/numpy/', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy/reference/', None),
-    'scikit-image': ('https://scikit-image.org/docs/stable/', None),
-    'matplotlib': ('https://matplotlib.org/stable/', None),
-}
+import sys
+from pathlib import Path
+
+root = Path(__file__).absolute().parent.parent
+sys.path.insert(0, str(root))
+
+DOCSDIR = '.'
+BUILDDIR = '_build'
+TEMPLATESDIR = '_templates'
+STATICDIR = '_static'
+SOURCEDIR = '../instamatic'
+
+
+# -- Run apidoc plug-in manually, as readthedocs doesn't support it -------
+# See https://github.com/rtfd/readthedocs.org/issues/1139
+def run_apidoc(app):
+    ignore_paths = []
+
+    cmd = ('--separate --no-toc --force --module-first '
+           f'-t {TEMPLATESDIR} '
+           f'-o {DOCSDIR} '
+           f'{SOURCEDIR} ')
+
+    args = cmd.split() + ignore_paths
+
+    from sphinx.ext import apidoc
+    apidoc.main(args)
+
+
+# Convert readme.md and others to rst to be included in index.html
+def make_markdown(app):
+    import subprocess
+    for inp, out in (('setup.md', 'setup.rst'),
+                     ('config.md', 'config.rst'),
+                     ('formats.md', 'formats.rst'),
+                     ('gui.md', 'gui.rst'),
+                     ('programs.md', 'programs.rst'),
+                     ('tem_api.md', 'tem_api.rst'),
+                     ('tvips.md', 'tvips.rst'),
+                     ('../readme.md', 'readme.rst')):
+        cmd = f'pandoc --from=markdown --to=rst --output={out} {inp}'
+        args = cmd.split()
+        subprocess.run(args)
+
+
+# https://www.sphinx-doc.org/en/master/extdev/appapi.html#sphinx-core-events
+# https://github.com/readthedocs/readthedocs.org/issues/2276
+def setup(app):
+    app.connect('builder-inited', make_markdown)
+    app.connect('builder-inited', run_apidoc)
+
+
+extensions = [
+    'sphinx.ext.autodoc',
+    # 'sphinx.ext.coverage',
+    # 'sphinx.ext.doctest',
+    # 'sphinx.ext.intersphinx',
+    # 'sphinx.ext.mathjax',
+    'sphinx.ext.napoleon',
+    'nbsphinx',
+    'nbsphinx_link',
+    # 'sphinx.ext.todo',
+    # 'sphinx.ext.viewcode',
+    'autodocsumm',
+]
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ['_templates']
+
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+source_suffix = ['.rst', '.md']
+
+# The master toctree document.
+master_doc = 'index'
+
+# General information about the project.
+project = 'instamatic'
+copyright = '2021, '
+author = 'Stef Smeets'
+
+# The short X.Y version.
+version = release = '1.9.0'
+
+# The language for content autogenerated by Sphinx.
+language = 'english'
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This patterns also effect to html_static_path and html_extra_path
+exclude_patterns = [BUILDDIR, 'Thumbs.db', '.DS_Store']
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = [STATICDIR]
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = 'sphinx'
+
+# If true, `todo` and `todoList` produce output, else they produce nothing.
+todo_include_todos = False
+
+# Use autoapi.extension to run sphinx-apidoc
+autoapi_dirs = [SOURCEDIR]
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+html_theme = 'sphinx_rtd_theme'
+# options for rtd-theme
+# html_theme_options = {
+#     'display_version': True,
+#     'prev_next_buttons_location': 'bottom',
+#     'style_external_links': False,
+#     # toc options
+#     'collapse_navigation': True,
+#     'sticky_navigation': True,
+#     'navigation_depth': 4,
+#     'includehidden': True,
+#     'titles_only': False,
+# }
+
+autodoc_default_options = {
+    'autosummary': True,
+    'special-members': '__init__',
+}
+
+nbsphinx_allow_errors = True
+nbsphinx_execute = 'never'
+
+autodoc_mock_imports = [
+    'h5py',
+    'virtualbox',
+    'pywinauto',
+    'pyserialem',
+    'predicrystal',
+    'lmfit',
+    'mrcfile',
+    'comtypes',
+    'msvcrt',
+]
+
+intersphinx_mapping = {
+    'python': ('https://docs.python.org/3', None),
+    'numpy': ('https://docs.scipy.org/doc/numpy/', None),
+    'scipy': ('https://docs.scipy.org/doc/scipy/reference/', None),
+    'scikit-image': ('https://scikit-image.org/docs/stable/', None),
+    'matplotlib': ('https://matplotlib.org/stable/', None),
+}
```

### Comparing `instamatic-1.8.0/docs/config.md` & `instamatic-1.9.0/docs/config.md`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 ```
 
 ## camera.yaml:
 
 This file holds the specifications of the camera. This file is must be located the `config/camera` directory, and can have any name as defined in `settings.yaml`.
 
 **interface**  
-Give the interface of the camera interface to connect to, for example: `timepix`/`emmenu`/`simulate`/`gatan`. Leave blank to load the camera specs, but do not load the camera module (this also turns off the videostream gui).
+Give the interface of the camera interface to connect to, for example: `timepix`/`emmenu`/`simulate`/`gatan`/'merlin'. Leave blank to load the camera specs, but do not load the camera module (this also turns off the videostream gui).
 
 **default_binsize**  
 Set the default binsize, default: `1`.
 
 **default_exposure**  
 Set the default exposure in seconds, i.e. `0.02`.
```

### Comparing `instamatic-1.8.0/docs/formats.md` & `instamatic-1.9.0/docs/formats.md`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/docs/gui.md` & `instamatic-1.9.0/docs/gui.md`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/docs/make_programs_md.py` & `instamatic-1.9.0/docs/make_programs_md.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/docs/programs.md` & `instamatic-1.9.0/docs/programs.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,568 +1,568 @@
-# Programs and scripts
-
-There are several programs coming with `instamatic`. These docs are autogenerated from the program description (*i.e.* `instamatic -h`).
-
-- **Main**
-  + [instamatic](#instamatic) (`instamatic.main:main`)
-  + [instamatic.controller](#instamaticcontroller) (`instamatic.TEMController.TEMController:main_entry`)
-- **Experiments**
-  + [instamatic.serialed](#instamaticserialed) (`instamatic.experiments.serialed.experiment:main`)
-  + [instamatic.camera](#instamaticcamera) (`instamatic.camera.camera:main_entry`)
-- **Calibrate**
-  + [instamatic.calibrate_stage_lowmag](#instamaticcalibrate_stage_lowmag) (`instamatic.calibrate.calibrate_stage_lowmag:main_entry`)
-  + [instamatic.calibrate_stage_mag1](#instamaticcalibrate_stage_mag1) (`instamatic.calibrate.calibrate_stage_mag1:main_entry`)
-  + [instamatic.calibrate_beamshift](#instamaticcalibrate_beamshift) (`instamatic.calibrate.calibrate_beamshift:main_entry`)
-  + [instamatic.calibrate_directbeam](#instamaticcalibrate_directbeam) (`instamatic.calibrate.calibrate_directbeam:main_entry`)
-  + [instamatic.calibrate_stagematrix](#instamaticcalibrate_stagematrix) (`instamatic.calibrate.calibrate_stagematrix:main_entry`)
-  + [instamatic.flatfield](#instamaticflatfield) (`instamatic.processing.flatfield:main_entry`)
-  + [instamatic.stretch_correction](#instamaticstretch_correction) (`instamatic.processing.stretch_correction:main_entry`)
-- **Tools**
-  + [instamatic.browser](#instamaticbrowser) (`scripts.browser:main`)
-  + [instamatic.viewer](#instamaticviewer) (`scripts.viewer:main`)
-  + [instamatic.defocus_helper](#instamaticdefocus_helper) (`instamatic.gui.defocus_button:main`)
-  + [instamatic.find_crystals](#instamaticfind_crystals) (`instamatic.processing.find_crystals:main_entry`)
-  + [instamatic.find_crystals_ilastik](#instamaticfind_crystals_ilastik) (`instamatic.processing.find_crystals_ilastik:main_entry`)
-  + [instamatic.learn](#instamaticlearn) (`scripts.learn:main_entry`)
-- **Server**
-  + [instamatic.temserver](#instamatictemserver) (`instamatic.server.tem_server:main`)
-  + [instamatic.camserver](#instamaticcamserver) (`instamatic.server.cam_server:main`)
-  + [instamatic.dialsserver](#instamaticdialsserver) (`instamatic.server.dials_server:main`)
-  + [instamatic.VMserver](#instamaticVMserver) (`instamatic.server.vm_ubuntu_server:main`)
-  + [instamatic.xdsserver](#instamaticxdsserver) (`instamatic.server.xds_server:main`)
-  + [instamatic.temserver_fei](#instamatictemserver_fei) (`instamatic.server.TEMServer_FEI:main`)
-  + [instamatic.goniotoolserver](#instamaticgoniotoolserver) (`instamatic.server.goniotool_server:main`)
-- **Setup**
-  + [instamatic.autoconfig](#instamaticautoconfig) (`instamatic.config.autoconfig:main`)
-  + [instamatic.install](#instamaticinstall) (Cmder)
-
-
-## instamatic
-
-Start instamatic with various functions (see below). If no arguments are given, start the instamatic GUI. The GUI is modular and can be defined using the config system. The GUI can be used to control the microscope and run the experiments. The GUI itself is further described on the GUI page.
-
-**Usage:**  
-```bash
-instamatic [-h] [-s SCRIPT] [-n NAV_FILE] [-a] [-l LOCATE] [-o SHOW]
-           [-i]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-s SCRIPT`, `--script SCRIPT`:  
- Run the script given  
-`-n NAV_FILE`, `--nav NAV_FILE`:  
- Load the given .nav file  
-`-a`, `--acquire_at_items`:  
- Run the script file `--script` at every point marked with `Acquire` in the nav file `--nav`.  
-`-l LOCATE`, `--locate LOCATE`:  
- Locate a requested directory and exit, i.e. `config`, `data`, `scripts`, `base`, 'work`, `logs`  
-`-o SHOW`, `--open SHOW`:  
-Open the requested directory and exit, see `--locate`.  
-`-i`, `--info`:  
-Show info about the current instamatic installation.  
-
-
-## instamatic.controller
-
-Connect to the microscope and camera, and open an IPython terminal to interactively control the microscope. Useful for testing! It initializes the TEMController (accessible through the `ctrl` variable) using the parameters given in the `config`.
-
-**Usage:**  
-```bash
-instamatic.controller [-h] [-u] [-c TEM_NAME] [-t CAM_NAME]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-u`, `--simulate`:  
-Simulate microscope connection (default: False)  
-`-c TEM_NAME`, `--camera TEM_NAME`:  
- Camera configuration to load.  
-`-t CAM_NAME`, `--tem CAM_NAME`:  
- TEM configuration to load.  
-
-
-## instamatic.serialed
-
-Command line program to run the serial ED data collection routine.
-
-**Usage:**  
-```bash
-instamatic.serialed [-h]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.camera
-
-Simple program to acquire image data from the camera.
-
-**Usage:**  
-```bash
-instamatic.camera [-h] [-b N] [-e N] [-o image.png] [-d] [-s]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-b N`, `--binsize N`:  
-Binsize to use. Must be one of 1, 2, or 4 (default 1)  
-`-e N`, `--exposure N`:  
-Exposure time (default 0.5)  
-`-o image.png`, `--out image.png`:  
- Where to store image  
-`-d`, `--display`:  
-Show the image (default True)  
-`-s`, `--series`:  
-Enable mode to take a series of images (default False)  
-
-
-## instamatic.calibrate_stage_lowmag
-
-Program to calibrate the lowmag mode (100x) of the microscope (Deprecated).
-
-**Usage:**  
-```bash
-instamatic.calibrate_stage_lowmag [-h] [IMG [IMG ...]]
-```
-**Positional arguments:**  
-`IMG`:  
-Perform calibration using pre-collected images. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
-
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.calibrate_stage_mag1
-
-Program to calibrate the mag1 mode of the microscope (Deprecated).
-
-**Usage:**  
-```bash
-instamatic.calibrate_stage_mag1 [-h] [IMG [IMG ...]]
-```
-**Positional arguments:**  
-`IMG`:  
-Perform calibration using pre-collected images. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
-
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.calibrate_beamshift
-
-Program to calibrate the beamshift of the microscope (Deprecated).
-
-**Usage:**  
-```bash
-instamatic.calibrate_beamshift [-h] [IMG [IMG ...]]
-```
-**Positional arguments:**  
-`IMG`:  
-Perform calibration using pre-collected images. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
-
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.calibrate_directbeam
-
-Program to calibrate the diffraction shift (PLA) to correct for beamshift movements (Deprecated).
-
-**Usage:**  
-```bash
-instamatic.calibrate_directbeam [-h] [IMG [IMG ...]]
-```
-**Positional arguments:**  
-`IMG`:  
-Perform calibration using pre-collected images. They must be formatted as such: DiffShift:pattern.tiff BeamShift:pattern.tiff, where `pattern` is a globbing pattern that finds the images corresponding to the key BeamShift or DiffShift. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
-
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.calibrate_stagematrix
-
-Run the stagematrix calibration routine for all magnifications
-specified. Return the updates values for the configuration file.
-
-Calibrate the stage movement (nm) and the position of the camera
-(pixels) at a specific magnification.
-
-The stagematrix takes the image binning into account.
-
-**Usage:**  
-```bash
-instamatic.calibrate_stagematrix [-h] [-m MODE] [-k K [K ...]] [-A]
-                                 [-v X] [-l STAGE_LENGTH] [-a N] [-b N]
-                                 [-s]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-m MODE`, `--mode MODE`:  
-Select the imaging mode (mag1/mag2/lowmag/samag). If `all` is specified, all imaging modes+mags are calibrated.If the imaging mode and magnification are not given, the currentvalues are used.  
-`-k K [K ...]`, `--mag K [K ...]`:  
- Select the imaging magnification(s).  
-`-A`, `--all_mags`:  
-Run calibration routine for all mags over selected mode.  
-`-v X`, `--overlap X`:  
-Specify the approximate overlap between images for cross correlation.  
-`-l STAGE_LENGTH`, `--stage_length STAGE_LENGTH`:  
- Specify the minimum length (in stage coordinates) the calibration should cover.  
-`-a N`, `--min_n_steps N`:  
- Specify the minimum number of steps to take along X and Y for the calibration.  
-`-b N`, `--max_n_steps N`:  
- Specify the maximum number of steps to take along X and Y for the calibration. This is used for higher magnifications.  
-`-s`, `--save`:  
-Save the data to the data directory [C:\instamatic].  
-
-
-## instamatic.flatfield
-
-This is a program that can collect and apply flatfield/darkfield corrections [link](https://en.wikipedia.org/wiki/Flat-field_correction). To do so, use a spread, bright beam on a hole in the carbon, or a clear piece of carbon film, and run:
-
-    instamatic.flatfield --collect
-
-This will collect 100 images and average them to determine the flatfield image. A darkfield image is also collected by applying the same routine with the beam blanked. Dead pixels are identified as pixels with 0 intensities. To apply these corrections:
-
-    instamatic.flatfield image.tiff [image.tiff ..] -f flatfield.tiff [-d darkfield.tiff] [-o drc]
-
-This will apply the flatfield correction (`-f`) and optionally the darkfield correction (`-d`) to images given as argument, and place the corrected files in directory `corrected` or as specified using `-o`.
-
-**Usage:**  
-```bash
-instamatic.flatfield [-h] [-f flatfield.tiff] [-d darkfield.tiff]
-                     [-o DRC] [-c]
-                     [image.tiff [image.tiff ...]]
-```
-**Positional arguments:**  
-`image.tiff`:  
-Image file paths/pattern  
-
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-f flatfield.tiff`, `--flatfield flatfield.tiff`:  
- Path to flatfield file  
-`-d darkfield.tiff`, `--darkfield darkfield.tiff`:  
- Path to darkfield file  
-`-o DRC`, `--output DRC`:  
-Output directory for image files  
-`-c`, `--collect`:  
-Collect flatfield/darkfield images on microscope  
-
-
-## instamatic.stretch_correction
-
-Program to determine the stretch correction from a series of powder diffraction patterns (collected on a gold or aluminium powder). It will open a GUI to interactively identify the powder rings, and calculate the orientation (azimuth) and extent (amplitude) of the long axis compared to the short axis. These can be used in the `config` under `camera.stretch_azimuth` and `camera.stretch_percentage`.
-
-**Usage:**  
-```bash
-instamatic.stretch_correction [-h] powder_pattern.tiff
-```
-**Positional arguments:**  
-`powder_pattern.tiff`:  
-Diffraction pattern (TIFF) from a nanocrystalline powder showing Debye-Scherrer rings.  
-
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.browser
-
-Program for browsing through electron diffraction images collected by `instamatic`.
-
-Example:
-
-    instamatic.browser images/*.tiff -r results.csv
-
-**Usage:**  
-```bash
-instamatic.browser [-h] [-s] [FILE]
-```
-**Positional arguments:**  
-`FILE`:  
-File pattern to image files  
-
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-s`, `--stitch`:  
-Stitch images together.  
-
-
-## instamatic.viewer
-
-Simple image viewer to open any image collected collected using instamatic. Supported formats include `TIFF`, `MRC`, [`HDF5`](http://www.h5py.org/), and [`SMV`](https://strucbio.biologie.uni-konstanz.de/ccp4wiki/index.php/SMV_file_format).
-
-**Usage:**  
-```bash
-instamatic.viewer [-h] IMG
-```
-**Positional arguments:**  
-`IMG`:  
-Image to display (TIFF, HDF5, MRC, SMV).  
-
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.defocus_helper
-
-Tiny button to focus and defocus the diffraction pattern.
-
-**Usage:**  
-```bash
-instamatic.defocus_helper [-h]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.find_crystals
-
-Find crystals in images.
-
-**Usage:**  
-```bash
-instamatic.find_crystals [-h] [IMG [IMG ...]]
-```
-**Positional arguments:**  
-`IMG`:  
-Images to find crystals in.  
-
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.find_crystals_ilastik
-
-Find crystals in images using Ilastik.
-
-Takes a `.nav` file and `.mrc` file as input.
-Performs pixel and object classification using the Ilastik interface in
-[predicrystal](https://gitlab.com/aj-lab/predicrystal). Crystals are
-filtered by their distance. The resulting data is stored in a new `.nav`
-file compatible with `SerialEM` or `Instamatic`.
-
-**Usage:**  
-```bash
-instamatic.find_crystals_ilastik [-h] [-n <path>] [-m <path>]
-                                 [-c <name>] [-f D] [-d <path>]
-                                 [--mapscaleind]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-n <path>`, `--nav <path>`, `--nav_location <path>`:  
- The full path to the .nav file. Enter as raw string  
-`-m <path>`, `--mrc <path>`, `--mrc_location <path>`:  
- The full path to the .mrc file (not the global map). Enter as raw string  
-`-c <name>`, `--classifier <name>`:  
- Use the classifier as defined in /classifiers/classifiers.yaml  
-`-f D`, `--filter_dist D`, `--filter_distance D`:  
- Specify what distance the crystals should be separated  
-`-d <path>`, `--output <path>`, `--output_name <path>`:  
- The destination of the .nav file created  
-`--mapscaleind`:  
-Generate `MapScaleInd.yaml` for `predicrystal` from config.  
-
-
-## instamatic.learn
-
-Predict whether a crystal is of good or bad quality by its diffraction pattern.
-
-**Usage:**  
-```bash
-instamatic.learn [-h] PAT
-```
-**Positional arguments:**  
-`PAT`:  
-File pattern to glob for images (HDF5), i.e. `images/*.h5`.  
-
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.temserver
-
-Connects to the TEM and starts a server for microscope communication. Opens a socket on port localhost:8088.
-
-This program initializes a connection to the TEM as defined in the config. On some setups it must be run in admin mode in order to establish a connection (on JEOL TEMs, wait for the beep!). The purpose of this program is to isolate the microscope connection in a separate process for improved stability of the interface in case instamatic crashes or is started and stopped frequently. For running the GUI, the temserver is required. Another reason is that it allows for remote connections from different PCs. The connection goes over a TCP socket.
-
-The host and port are defined in `config/settings.yaml`.
-
-The data sent over the socket is a serialized dictionary with the following elements:
-
-- `func_name`: Name of the function to call (str)
-- `args`: (Optional) List of arguments for the function (list)
-- `kwargs`: (Optiona) Dictionary of keyword arguments for the function (dict)
-
-The response is returned as a serialized object.
-
-**Usage:**  
-```bash
-instamatic.temserver [-h] [-t MICROSCOPE]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-t MICROSCOPE`, `--microscope MICROSCOPE`:  
- Override microscope to use.  
-
-
-## instamatic.camserver
-
-Connects to the camera and starts a server for camera communication. Opens a socket on port localhost:8087.
-
-This program initializes a connection to the camera as defined in the config. This separates the communication from the main process and allows for remote connections from different PCs. The connection goes over a TCP socket.
-
-The host and port are defined in `config/settings.yaml`.
-
-The data sent over the socket is a pickled dictionary with the following elements:
-
-- `attr_name`: Name of the function to call or attribute to return (str)
-- `args`: (Optional) List of arguments for the function (list)
-- `kwargs`: (Optiona) Dictionary of keyword arguments for the function (dict)
-
-The response is returned as a pickle object.
-
-**Usage:**  
-```bash
-instamatic.camserver [-h] [-c CAMERA]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-c CAMERA`, `--camera CAMERA`:  
- Override camera to use.  
-
-
-## instamatic.dialsserver
-
-Starts a simple server to send indexing jobs to. Runs `-h` for every job sent to it. Opens a socket on port localhost:8089.
-
-The data sent to the server is a dict containing the following elements:
-
-- `path`: Path to the data directory (str)
-- `rotrange`: Total rotation range in degrees (float)
-- `nframes`: Number of data frames (int)
-- `osc`: Oscillation range in degrees (float)
-
-**Usage:**  
-```bash
-instamatic.dialsserver [-h]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.VMserver
-
-The script sets up socket connection between `instamatic` and `VirtualBox` software via `virtualbox` python API. Therefore, `VirtualBox` and the corresponding SDK need to be installed before running this command. This script is developed particularly for the possibility of running `XDS` under windows 7 or newer, a system which a lot of TEM computers may be using.
-
-After installation of VirtualBox and the corresponding SDK, `XDS` needs to be installed correctly in the guest Ubuntu system. In addition, a shared folder between `VirtualBox` and windows system needs to be set up properly in order for the server to work.
-
-The host and port are defined in `config/settings.yaml`.
-
-**Usage:**  
-```bash
-instamatic.VMserver [-h] [-shelxt] [-c a b c al be ga] [-s SPGR]
-                    [-m Xn [Ym ...]]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-shelxt`:  
-Run SHELXT when xds ASCII HKL file is generated.  
-`-c a b c al be ga`, `--unitcell a b c al be ga`:  
- Six numbers of the unit cell parameters.  
-`-s SPGR`, `--spgr SPGR`:  
-Space group.  
-`-m Xn [Ym ...]`, `--composition Xn [Ym ...]`:  
- Unit cell composition, i.e. `-m H2 O1`.  
-
-
-## instamatic.xdsserver
-
-Starts a simple XDS server to send indexing jobs to. Runs XDS for every job sent to it. Opens a socket on port localhost:8089.
-
-The data sent to the server as a bytes string containing the data path (must contain `cRED_log.txt`).
-
-**Usage:**  
-```bash
-instamatic.xdsserver [-h]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.temserver_fei
-
-Utility script to enable rotation control from a dmscript. See [https://github.com/instamatic-dev/instamatic/tree/master/dmscript] for usage.
-
-**Usage:**  
-```bash
-instamatic.temserver_fei [-h]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.goniotoolserver
-
-Connects to `Goniotool.exe` and starts a server for network communication. Opens a socket on port localhost:8090.
-
-The host and port are defined in `config/settings.yaml`.
-
-The data sent over the socket is a serialized dictionary with the following elements:
-
-- `func_name`: Name of the function to call (str)
-- `args`: (Optional) List of arguments for the function (list)
-- `kwargs`: (Optiona) Dictionary of keyword arguments for the function (dict)
-
-The response is returned as a pickle object.
-
-**Usage:**  
-```bash
-instamatic.goniotoolserver [-h]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.autoconfig
-
-This tool will help to set up the configuration files for `instamatic`.
-It establishes a connection to the microscope and reads out the camera lengths and magnification ranges.
-
-**Usage:**  
-```bash
-instamatic.autoconfig [-h]
-```
-**Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.install
-
-This script sets up the paths for `instamatic`. It is necessary to run it at after first installation, and sometimes when the program is updated, or when the instamatic directory has moved.
-
-Usage:
-
-    instamatic.install
+# Programs and scripts
+
+There are several programs coming with `instamatic`. These docs are autogenerated from the program description (*i.e.* `instamatic -h`).
+
+- **Main**
+  + [instamatic](#instamatic) (`instamatic.main:main`)
+  + [instamatic.controller](#instamaticcontroller) (`instamatic.TEMController.TEMController:main_entry`)
+- **Experiments**
+  + [instamatic.serialed](#instamaticserialed) (`instamatic.experiments.serialed.experiment:main`)
+  + [instamatic.camera](#instamaticcamera) (`instamatic.camera.camera:main_entry`)
+- **Calibrate**
+  + [instamatic.calibrate_stage_lowmag](#instamaticcalibrate_stage_lowmag) (`instamatic.calibrate.calibrate_stage_lowmag:main_entry`)
+  + [instamatic.calibrate_stage_mag1](#instamaticcalibrate_stage_mag1) (`instamatic.calibrate.calibrate_stage_mag1:main_entry`)
+  + [instamatic.calibrate_beamshift](#instamaticcalibrate_beamshift) (`instamatic.calibrate.calibrate_beamshift:main_entry`)
+  + [instamatic.calibrate_directbeam](#instamaticcalibrate_directbeam) (`instamatic.calibrate.calibrate_directbeam:main_entry`)
+  + [instamatic.calibrate_stagematrix](#instamaticcalibrate_stagematrix) (`instamatic.calibrate.calibrate_stagematrix:main_entry`)
+  + [instamatic.flatfield](#instamaticflatfield) (`instamatic.processing.flatfield:main_entry`)
+  + [instamatic.stretch_correction](#instamaticstretch_correction) (`instamatic.processing.stretch_correction:main_entry`)
+- **Tools**
+  + [instamatic.browser](#instamaticbrowser) (`scripts.browser:main`)
+  + [instamatic.viewer](#instamaticviewer) (`scripts.viewer:main`)
+  + [instamatic.defocus_helper](#instamaticdefocus_helper) (`instamatic.gui.defocus_button:main`)
+  + [instamatic.find_crystals](#instamaticfind_crystals) (`instamatic.processing.find_crystals:main_entry`)
+  + [instamatic.find_crystals_ilastik](#instamaticfind_crystals_ilastik) (`instamatic.processing.find_crystals_ilastik:main_entry`)
+  + [instamatic.learn](#instamaticlearn) (`scripts.learn:main_entry`)
+- **Server**
+  + [instamatic.temserver](#instamatictemserver) (`instamatic.server.tem_server:main`)
+  + [instamatic.camserver](#instamaticcamserver) (`instamatic.server.cam_server:main`)
+  + [instamatic.dialsserver](#instamaticdialsserver) (`instamatic.server.dials_server:main`)
+  + [instamatic.VMserver](#instamaticVMserver) (`instamatic.server.vm_ubuntu_server:main`)
+  + [instamatic.xdsserver](#instamaticxdsserver) (`instamatic.server.xds_server:main`)
+  + [instamatic.temserver_fei](#instamatictemserver_fei) (`instamatic.server.TEMServer_FEI:main`)
+  + [instamatic.goniotoolserver](#instamaticgoniotoolserver) (`instamatic.server.goniotool_server:main`)
+- **Setup**
+  + [instamatic.autoconfig](#instamaticautoconfig) (`instamatic.config.autoconfig:main`)
+  + [instamatic.install](#instamaticinstall) (Cmder)
+
+
+## instamatic
+
+Start instamatic with various functions (see below). If no arguments are given, start the instamatic GUI. The GUI is modular and can be defined using the config system. The GUI can be used to control the microscope and run the experiments. The GUI itself is further described on the GUI page.
+
+**Usage:**  
+```bash
+instamatic [-h] [-s SCRIPT] [-n NAV_FILE] [-a] [-l LOCATE] [-o SHOW]
+           [-i]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+`-s SCRIPT`, `--script SCRIPT`:  
+ Run the script given  
+`-n NAV_FILE`, `--nav NAV_FILE`:  
+ Load the given .nav file  
+`-a`, `--acquire_at_items`:  
+ Run the script file `--script` at every point marked with `Acquire` in the nav file `--nav`.  
+`-l LOCATE`, `--locate LOCATE`:  
+ Locate a requested directory and exit, i.e. `config`, `data`, `scripts`, `base`, 'work`, `logs`  
+`-o SHOW`, `--open SHOW`:  
+Open the requested directory and exit, see `--locate`.  
+`-i`, `--info`:  
+Show info about the current instamatic installation.  
+
+
+## instamatic.controller
+
+Connect to the microscope and camera, and open an IPython terminal to interactively control the microscope. Useful for testing! It initializes the TEMController (accessible through the `ctrl` variable) using the parameters given in the `config`.
+
+**Usage:**  
+```bash
+instamatic.controller [-h] [-u] [-c TEM_NAME] [-t CAM_NAME]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+`-u`, `--simulate`:  
+Simulate microscope connection (default: False)  
+`-c TEM_NAME`, `--camera TEM_NAME`:  
+ Camera configuration to load.  
+`-t CAM_NAME`, `--tem CAM_NAME`:  
+ TEM configuration to load.  
+
+
+## instamatic.serialed
+
+Command line program to run the serial ED data collection routine.
+
+**Usage:**  
+```bash
+instamatic.serialed [-h]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.camera
+
+Simple program to acquire image data from the camera.
+
+**Usage:**  
+```bash
+instamatic.camera [-h] [-b N] [-e N] [-o image.png] [-d] [-s]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+`-b N`, `--binsize N`:  
+Binsize to use. Must be one of 1, 2, or 4 (default 1)  
+`-e N`, `--exposure N`:  
+Exposure time (default 0.5)  
+`-o image.png`, `--out image.png`:  
+ Where to store image  
+`-d`, `--display`:  
+Show the image (default True)  
+`-s`, `--series`:  
+Enable mode to take a series of images (default False)  
+
+
+## instamatic.calibrate_stage_lowmag
+
+Program to calibrate the lowmag mode (100x) of the microscope (Deprecated).
+
+**Usage:**  
+```bash
+instamatic.calibrate_stage_lowmag [-h] [IMG [IMG ...]]
+```
+**Positional arguments:**  
+`IMG`:  
+Perform calibration using pre-collected images. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
+
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.calibrate_stage_mag1
+
+Program to calibrate the mag1 mode of the microscope (Deprecated).
+
+**Usage:**  
+```bash
+instamatic.calibrate_stage_mag1 [-h] [IMG [IMG ...]]
+```
+**Positional arguments:**  
+`IMG`:  
+Perform calibration using pre-collected images. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
+
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.calibrate_beamshift
+
+Program to calibrate the beamshift of the microscope (Deprecated).
+
+**Usage:**  
+```bash
+instamatic.calibrate_beamshift [-h] [IMG [IMG ...]]
+```
+**Positional arguments:**  
+`IMG`:  
+Perform calibration using pre-collected images. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
+
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.calibrate_directbeam
+
+Program to calibrate the diffraction shift (PLA) to correct for beamshift movements (Deprecated).
+
+**Usage:**  
+```bash
+instamatic.calibrate_directbeam [-h] [IMG [IMG ...]]
+```
+**Positional arguments:**  
+`IMG`:  
+Perform calibration using pre-collected images. They must be formatted as such: DiffShift:pattern.tiff BeamShift:pattern.tiff, where `pattern` is a globbing pattern that finds the images corresponding to the key BeamShift or DiffShift. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
+
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.calibrate_stagematrix
+
+Run the stagematrix calibration routine for all magnifications
+specified. Return the updates values for the configuration file.
+
+Calibrate the stage movement (nm) and the position of the camera
+(pixels) at a specific magnification.
+
+The stagematrix takes the image binning into account.
+
+**Usage:**  
+```bash
+instamatic.calibrate_stagematrix [-h] [-m MODE] [-k K [K ...]] [-A]
+                                 [-v X] [-l STAGE_LENGTH] [-a N] [-b N]
+                                 [-s]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+`-m MODE`, `--mode MODE`:  
+Select the imaging mode (mag1/mag2/lowmag/samag). If `all` is specified, all imaging modes+mags are calibrated.If the imaging mode and magnification are not given, the currentvalues are used.  
+`-k K [K ...]`, `--mag K [K ...]`:  
+ Select the imaging magnification(s).  
+`-A`, `--all_mags`:  
+Run calibration routine for all mags over selected mode.  
+`-v X`, `--overlap X`:  
+Specify the approximate overlap between images for cross correlation.  
+`-l STAGE_LENGTH`, `--stage_length STAGE_LENGTH`:  
+ Specify the minimum length (in stage coordinates) the calibration should cover.  
+`-a N`, `--min_n_steps N`:  
+ Specify the minimum number of steps to take along X and Y for the calibration.  
+`-b N`, `--max_n_steps N`:  
+ Specify the maximum number of steps to take along X and Y for the calibration. This is used for higher magnifications.  
+`-s`, `--save`:  
+Save the data to the data directory [C:\instamatic].  
+
+
+## instamatic.flatfield
+
+This is a program that can collect and apply flatfield/darkfield corrections [link](https://en.wikipedia.org/wiki/Flat-field_correction). To do so, use a spread, bright beam on a hole in the carbon, or a clear piece of carbon film, and run:
+
+    instamatic.flatfield --collect
+
+This will collect 100 images and average them to determine the flatfield image. A darkfield image is also collected by applying the same routine with the beam blanked. Dead pixels are identified as pixels with 0 intensities. To apply these corrections:
+
+    instamatic.flatfield image.tiff [image.tiff ..] -f flatfield.tiff [-d darkfield.tiff] [-o drc]
+
+This will apply the flatfield correction (`-f`) and optionally the darkfield correction (`-d`) to images given as argument, and place the corrected files in directory `corrected` or as specified using `-o`.
+
+**Usage:**  
+```bash
+instamatic.flatfield [-h] [-f flatfield.tiff] [-d darkfield.tiff]
+                     [-o DRC] [-c]
+                     [image.tiff [image.tiff ...]]
+```
+**Positional arguments:**  
+`image.tiff`:  
+Image file paths/pattern  
+
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+`-f flatfield.tiff`, `--flatfield flatfield.tiff`:  
+ Path to flatfield file  
+`-d darkfield.tiff`, `--darkfield darkfield.tiff`:  
+ Path to darkfield file  
+`-o DRC`, `--output DRC`:  
+Output directory for image files  
+`-c`, `--collect`:  
+Collect flatfield/darkfield images on microscope  
+
+
+## instamatic.stretch_correction
+
+Program to determine the stretch correction from a series of powder diffraction patterns (collected on a gold or aluminium powder). It will open a GUI to interactively identify the powder rings, and calculate the orientation (azimuth) and extent (amplitude) of the long axis compared to the short axis. These can be used in the `config` under `camera.stretch_azimuth` and `camera.stretch_percentage`.
+
+**Usage:**  
+```bash
+instamatic.stretch_correction [-h] powder_pattern.tiff
+```
+**Positional arguments:**  
+`powder_pattern.tiff`:  
+Diffraction pattern (TIFF) from a nanocrystalline powder showing Debye-Scherrer rings.  
+
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.browser
+
+Program for browsing through electron diffraction images collected by `instamatic`.
+
+Example:
+
+    instamatic.browser images/*.tiff -r results.csv
+
+**Usage:**  
+```bash
+instamatic.browser [-h] [-s] [FILE]
+```
+**Positional arguments:**  
+`FILE`:  
+File pattern to image files  
+
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+`-s`, `--stitch`:  
+Stitch images together.  
+
+
+## instamatic.viewer
+
+Simple image viewer to open any image collected collected using instamatic. Supported formats include `TIFF`, `MRC`, [`HDF5`](http://www.h5py.org/), and [`SMV`](https://strucbio.biologie.uni-konstanz.de/ccp4wiki/index.php/SMV_file_format).
+
+**Usage:**  
+```bash
+instamatic.viewer [-h] IMG
+```
+**Positional arguments:**  
+`IMG`:  
+Image to display (TIFF, HDF5, MRC, SMV).  
+
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.defocus_helper
+
+Tiny button to focus and defocus the diffraction pattern.
+
+**Usage:**  
+```bash
+instamatic.defocus_helper [-h]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.find_crystals
+
+Find crystals in images.
+
+**Usage:**  
+```bash
+instamatic.find_crystals [-h] [IMG [IMG ...]]
+```
+**Positional arguments:**  
+`IMG`:  
+Images to find crystals in.  
+
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.find_crystals_ilastik
+
+Find crystals in images using Ilastik.
+
+Takes a `.nav` file and `.mrc` file as input.
+Performs pixel and object classification using the Ilastik interface in
+[predicrystal](https://gitlab.com/aj-lab/predicrystal). Crystals are
+filtered by their distance. The resulting data is stored in a new `.nav`
+file compatible with `SerialEM` or `Instamatic`.
+
+**Usage:**  
+```bash
+instamatic.find_crystals_ilastik [-h] [-n <path>] [-m <path>]
+                                 [-c <name>] [-f D] [-d <path>]
+                                 [--mapscaleind]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+`-n <path>`, `--nav <path>`, `--nav_location <path>`:  
+ The full path to the .nav file. Enter as raw string  
+`-m <path>`, `--mrc <path>`, `--mrc_location <path>`:  
+ The full path to the .mrc file (not the global map). Enter as raw string  
+`-c <name>`, `--classifier <name>`:  
+ Use the classifier as defined in /classifiers/classifiers.yaml  
+`-f D`, `--filter_dist D`, `--filter_distance D`:  
+ Specify what distance the crystals should be separated  
+`-d <path>`, `--output <path>`, `--output_name <path>`:  
+ The destination of the .nav file created  
+`--mapscaleind`:  
+Generate `MapScaleInd.yaml` for `predicrystal` from config.  
+
+
+## instamatic.learn
+
+Predict whether a crystal is of good or bad quality by its diffraction pattern.
+
+**Usage:**  
+```bash
+instamatic.learn [-h] PAT
+```
+**Positional arguments:**  
+`PAT`:  
+File pattern to glob for images (HDF5), i.e. `images/*.h5`.  
+
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.temserver
+
+Connects to the TEM and starts a server for microscope communication. Opens a socket on port localhost:8088.
+
+This program initializes a connection to the TEM as defined in the config. On some setups it must be run in admin mode in order to establish a connection (on JEOL TEMs, wait for the beep!). The purpose of this program is to isolate the microscope connection in a separate process for improved stability of the interface in case instamatic crashes or is started and stopped frequently. For running the GUI, the temserver is required. Another reason is that it allows for remote connections from different PCs. The connection goes over a TCP socket.
+
+The host and port are defined in `config/settings.yaml`.
+
+The data sent over the socket is a serialized dictionary with the following elements:
+
+- `func_name`: Name of the function to call (str)
+- `args`: (Optional) List of arguments for the function (list)
+- `kwargs`: (Optiona) Dictionary of keyword arguments for the function (dict)
+
+The response is returned as a serialized object.
+
+**Usage:**  
+```bash
+instamatic.temserver [-h] [-t MICROSCOPE]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+`-t MICROSCOPE`, `--microscope MICROSCOPE`:  
+ Override microscope to use.  
+
+
+## instamatic.camserver
+
+Connects to the camera and starts a server for camera communication. Opens a socket on port localhost:8087.
+
+This program initializes a connection to the camera as defined in the config. This separates the communication from the main process and allows for remote connections from different PCs. The connection goes over a TCP socket.
+
+The host and port are defined in `config/settings.yaml`.
+
+The data sent over the socket is a pickled dictionary with the following elements:
+
+- `attr_name`: Name of the function to call or attribute to return (str)
+- `args`: (Optional) List of arguments for the function (list)
+- `kwargs`: (Optiona) Dictionary of keyword arguments for the function (dict)
+
+The response is returned as a pickle object.
+
+**Usage:**  
+```bash
+instamatic.camserver [-h] [-c CAMERA]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+`-c CAMERA`, `--camera CAMERA`:  
+ Override camera to use.  
+
+
+## instamatic.dialsserver
+
+Starts a simple server to send indexing jobs to. Runs `-h` for every job sent to it. Opens a socket on port localhost:8089.
+
+The data sent to the server is a dict containing the following elements:
+
+- `path`: Path to the data directory (str)
+- `rotrange`: Total rotation range in degrees (float)
+- `nframes`: Number of data frames (int)
+- `osc`: Oscillation range in degrees (float)
+
+**Usage:**  
+```bash
+instamatic.dialsserver [-h]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.VMserver
+
+The script sets up socket connection between `instamatic` and `VirtualBox` software via `virtualbox` python API. Therefore, `VirtualBox` and the corresponding SDK need to be installed before running this command. This script is developed particularly for the possibility of running `XDS` under windows 7 or newer, a system which a lot of TEM computers may be using.
+
+After installation of VirtualBox and the corresponding SDK, `XDS` needs to be installed correctly in the guest Ubuntu system. In addition, a shared folder between `VirtualBox` and windows system needs to be set up properly in order for the server to work.
+
+The host and port are defined in `config/settings.yaml`.
+
+**Usage:**  
+```bash
+instamatic.VMserver [-h] [-shelxt] [-c a b c al be ga] [-s SPGR]
+                    [-m Xn [Ym ...]]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+`-shelxt`:  
+Run SHELXT when xds ASCII HKL file is generated.  
+`-c a b c al be ga`, `--unitcell a b c al be ga`:  
+ Six numbers of the unit cell parameters.  
+`-s SPGR`, `--spgr SPGR`:  
+Space group.  
+`-m Xn [Ym ...]`, `--composition Xn [Ym ...]`:  
+ Unit cell composition, i.e. `-m H2 O1`.  
+
+
+## instamatic.xdsserver
+
+Starts a simple XDS server to send indexing jobs to. Runs XDS for every job sent to it. Opens a socket on port localhost:8089.
+
+The data sent to the server as a bytes string containing the data path (must contain `cRED_log.txt`).
+
+**Usage:**  
+```bash
+instamatic.xdsserver [-h]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.temserver_fei
+
+Utility script to enable rotation control from a dmscript. See [https://github.com/instamatic-dev/instamatic/tree/master/dmscript] for usage.
+
+**Usage:**  
+```bash
+instamatic.temserver_fei [-h]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.goniotoolserver
+
+Connects to `Goniotool.exe` and starts a server for network communication. Opens a socket on port localhost:8090.
+
+The host and port are defined in `config/settings.yaml`.
+
+The data sent over the socket is a serialized dictionary with the following elements:
+
+- `func_name`: Name of the function to call (str)
+- `args`: (Optional) List of arguments for the function (list)
+- `kwargs`: (Optiona) Dictionary of keyword arguments for the function (dict)
+
+The response is returned as a pickle object.
+
+**Usage:**  
+```bash
+instamatic.goniotoolserver [-h]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.autoconfig
+
+This tool will help to set up the configuration files for `instamatic`.
+It establishes a connection to the microscope and reads out the camera lengths and magnification ranges.
+
+**Usage:**  
+```bash
+instamatic.autoconfig [-h]
+```
+**Optional arguments:**  
+`-h`, `--help`:  
+show this help message and exit  
+
+
+## instamatic.install
+
+This script sets up the paths for `instamatic`. It is necessary to run it at after first installation, and sometimes when the program is updated, or when the instamatic directory has moved.
+
+Usage:
+
+    instamatic.install
```

### Comparing `instamatic-1.8.0/docs/setup.md` & `instamatic-1.9.0/docs/setup.md`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/docs/tem_api.md` & `instamatic-1.9.0/docs/tem_api.md`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/docs/tvips.md` & `instamatic-1.9.0/docs/tvips.md`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/TEMController/TEMController.py` & `instamatic-1.9.0/instamatic/TEMController/TEMController.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import time
 from collections import namedtuple
 from concurrent.futures import ThreadPoolExecutor
 from typing import Tuple
 
 import numpy as np
 
-from .deflectors import *
-from .lenses import *
-from .microscope import Microscope
-from .stage import *
-from .states import *
 from instamatic import config
 from instamatic.camera import Camera
 from instamatic.exceptions import TEMControllerError
 from instamatic.formats import write_tiff
 from instamatic.image_utils import rotate_image
 
+from .deflectors import *
+from .lenses import *
+from .microscope import Microscope
+from .stage import *
+from .states import *
 
 _ctrl = None  # store reference of ctrl so it can be accessed without re-initializing
 
 default_cam = config.camera.name
 default_tem = config.microscope.name
 
 use_tem_server = config.settings.use_tem_server
@@ -40,15 +40,14 @@
         Open the camera as a stream (this enables `TEMController.show_stream()`)
 
     Returns
     -------
     ctrl : `TEMController`
         Return TEM control object
     """
-
     print(f"Microscope: {tem_name}{' (server)' if use_tem_server else ''}")
     tem = Microscope(tem_name, use_server=use_tem_server)
 
     if cam_name:
         if use_cam_server:
             cam_tag = ' (server)'
         elif stream:
@@ -263,15 +262,14 @@
             Current TEM mode ("lowmag", "mag1")
 
         Returns
         -------
         stagematrix : np.array[2, 2]
             Affine transformation matrix to convert from stage to pixel coordinates
         """
-
         if not mode:
             mode = self.mode.get()
         if not mag:
             mag = self.magnification.value
         if not binning:
             binning = self.cam.getBinning()
 
@@ -439,15 +437,14 @@
         """Store microscope parameters to dict.
 
         keys: tuple of str (optional)
             If any keys are specified, dict is returned with only the given properties
 
         self.to_dict('all') or self.to_dict() will return all properties
         """
-
         # Each of these costs about 40-60 ms per call on a JEOL 2100, stage is 265 ms per call
         funcs = {
             'FunctionMode': self.tem.getFunctionMode,
             'GunShift': self.gunshift.get,
             'GunTilt': self.guntilt.get,
             'BeamShift': self.beamshift.get,
             'BeamTilt': self.beamtilt.get,
@@ -473,15 +470,14 @@
                 # print(f"No such key: `{key}`")
                 pass
 
         return dct
 
     def from_dict(self, dct: dict):
         """Restore microscope parameters from dict."""
-
         funcs = {
             # 'FunctionMode': self.tem.setFunctionMode,
             'GunShift': self.gunshift.set,
             'GunTilt': self.guntilt.set,
             'BeamShift': self.beamshift.set,
             'BeamTilt': self.beamtilt.set,
             'ImageShift1': self.imageshift1.set,
```

### Comparing `instamatic-1.8.0/instamatic/TEMController/deflectors.py` & `instamatic-1.9.0/instamatic/TEMController/deflectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from collections import namedtuple
 from typing import Tuple
 
-
 DeflectorTuple = namedtuple('DeflectorTuple', ['x', 'y'])
 
 
 class Deflector:
     """Generic microscope deflector object defined by X/Y values Must be
     subclassed to set the self._getter, self._setter functions."""
```

### Comparing `instamatic-1.8.0/instamatic/TEMController/fei_microscope.py` & `instamatic-1.9.0/instamatic/TEMController/fei_microscope.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import logging
 import time
 
 import comtypes.client
 from numpy import pi
 
 from instamatic import config
-from instamatic.exceptions import FEIValueError
-from instamatic.exceptions import TEMCommunicationError
+from instamatic.exceptions import FEIValueError, TEMCommunicationError
+
 logger = logging.getLogger(__name__)
 
 
 # speed table (deg/s):
 # 1.00: 21.14
 # 0.90: 19.61
 # 0.80: 18.34
```

### Comparing `instamatic-1.8.0/instamatic/TEMController/fei_simu_microscope.py` & `instamatic-1.9.0/instamatic/TEMController/fei_simu_microscope.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import logging
 import random
 import time
 
 import comtypes.client
 
 from instamatic import config
-from instamatic.exceptions import FEIValueError
-from instamatic.exceptions import TEMCommunicationError
+from instamatic.exceptions import FEIValueError, TEMCommunicationError
+
 logger = logging.getLogger(__name__)
 
 
 FUNCTION_MODES = {0: 'LM', 1: 'Mi', 2: 'SA', 3: 'Mh', 4: 'LAD', 5: 'D'}
 
 MIN = 0.0
 MAX = 1.0
```

### Comparing `instamatic-1.8.0/instamatic/TEMController/jeol_microscope.py` & `instamatic-1.9.0/instamatic/TEMController/jeol_microscope.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import logging
 import time
 from typing import Tuple
 
 import comtypes.client
 
 from instamatic import config
-from instamatic.exceptions import JEOLValueError
-from instamatic.exceptions import TEMCommunicationError
+from instamatic.exceptions import JEOLValueError, TEMCommunicationError, TEMValueError
+
 logger = logging.getLogger(__name__)
 
 NTRLMAPPING = {
     'GUN1': 0,
     'GUN2': 1,
     'CLA1': 2,
     'CLA2': 3,
```

### Comparing `instamatic-1.8.0/instamatic/TEMController/lenses.py` & `instamatic-1.9.0/instamatic/TEMController/lenses.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/TEMController/microscope.py` & `instamatic-1.9.0/instamatic/TEMController/microscope.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 default_tem_interface = config.microscope.interface
 
 __all__ = ['Microscope', 'get_tem']
 
 
 def get_tem(interface: str):
     """Grab tem class with the specific 'interface'."""
-
     simulate = config.settings.simulate
 
     if config.settings.tem_require_admin:
         from instamatic import admin
         if not admin.is_admin():
             raise PermissionError('Access to the TEM interface requires admin rights.')
 
@@ -35,15 +34,14 @@
     name: str
         Specify which microscope to use, must be one of `jeol`, `fei_simu`, `simulate`
     use_server: bool
         Connect to microscope server running on the host/port defined in the config file
 
     returns: TEM interface class
     """
-
     if name is None:
         interface = default_tem_interface
         name = interface
     elif name != config.settings.microscope:
         config.load_microscope_config(microscope_name=name)
         interface = config.microscope.interface
     else:
```

### Comparing `instamatic-1.8.0/instamatic/TEMController/microscope_client.py` & `instamatic-1.9.0/instamatic/TEMController/microscope_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,16 @@
 import socket
 import subprocess as sp
 import threading
 import time
 from functools import wraps
 
 from instamatic import config
-from instamatic.exceptions import exception_list
-from instamatic.exceptions import TEMCommunicationError
-from instamatic.server.serializer import dumper
-from instamatic.server.serializer import loader
-
+from instamatic.exceptions import TEMCommunicationError, exception_list
+from instamatic.server.serializer import dumper, loader
 
 HOST = config.settings.tem_server_host
 PORT = config.settings.tem_server_port
 BUFSIZE = 1024
 
 
 class ServerError(Exception):
@@ -74,15 +71,14 @@
 
     def connect(self):
         self.s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.s.connect((HOST, PORT))
         print(f'Connected to TEM server ({HOST}:{PORT})')
 
     def __getattr__(self, func_name):
-
         try:
             wrapped = self._dct[func_name]
         except KeyError as e:
             raise AttributeError(f'`{self.__class__.__name__}` object has no attribute `{func_name}`') from e
 
         @wraps(wrapped)
         def wrapper(*args, **kwargs):
@@ -91,15 +87,14 @@
                    'kwargs': kwargs}
             return self._eval_dct(dct)
 
         return wrapper
 
     def _eval_dct(self, dct):
         """Takes approximately 0.2-0.3 ms per call if HOST=='localhost'."""
-
         self.s.send(dumper(dct))
 
         response = self.s.recv(self._bufsize)
 
         if response:
             status, data = loader(response)
```

### Comparing `instamatic-1.8.0/instamatic/TEMController/simu_microscope.py` & `instamatic-1.9.0/instamatic/TEMController/simu_microscope.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import random
 import time
 from typing import Tuple
 
 from instamatic import config
 from instamatic.exceptions import TEMValueError
 
-
 NTRLMAPPING = {
     'GUN1': 0,
     'GUN2': 1,
     'CLA1': 2,
     'CLA2': 3,
     'SHIFT': 4,
     'TILT': 5,
```

### Comparing `instamatic-1.8.0/instamatic/TEMController/stage.py` & `instamatic-1.9.0/instamatic/TEMController/stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import time
 from collections import namedtuple
 from contextlib import contextmanager
 from typing import Tuple
 
 import numpy as np
 
-
 # namedtuples to store results from .get()
 StagePositionTuple = namedtuple('StagePositionTuple', ['x', 'y', 'z', 'a', 'b'])
 
 
 class Stage:
     """Stage control."""
 
@@ -106,16 +105,17 @@
 
     @xy.setter
     def xy(self, values: Tuple[int, int]):
         x, y = values
         self.set(x=x, y=y, wait=self._wait)
 
     def move_in_projection(self, delta_x: int, delta_y: int) -> None:
-        r"""y and z are always perpendicular to the sample stage. To achieve the movement
-        in the projection, x and yshould be broken down into the components z' and y'.
+        r"""y and z are always perpendicular to the sample stage. To achieve the
+        movement in the projection, x and yshould be broken down into the
+        components z' and y'.
 
         y = y' * cos(a)
         z = y' * sin(a)
 
         z'|  / z
           | /
           |/_____ y'
@@ -258,15 +258,14 @@
         step: float,
             stepsize in nm
         settle_delay: float,
             delay between movements in seconds to allow the stage to settle
         wait: bool,
             block until stage movement is complete (JEOL only)
         """
-
         stage = self.get()
 
         if shift_x:
             target_x = stage.x + shift_x
             if target_x > stage.x:
                 pre_x = stage.x - step
             elif target_x < stage.x:
```

### Comparing `instamatic-1.8.0/instamatic/TEMController/states.py` & `instamatic-1.9.0/instamatic/TEMController/states.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/acquire_at_items.py` & `instamatic-1.9.0/instamatic/acquire_at_items.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             for interval, funcs in self._acquire.items():
                 print(f'Acquire[{interval}]:', ', '.join([func.__name__ for func in funcs]))
 
             self._acquire_intervals = np.array(list(self._acquire.keys()))
 
         if post_acquire:
             self._post_acquire = self.validate(post_acquire)
-            print(f'Post-acquire:', ', '.join([func.__name__ for func in self._post_acquire]))
+            print('Post-acquire:', ', '.join([func.__name__ for func in self._post_acquire]))
 
         self.backlash = backlash
 
     # blank placeholders
     _acquire = ()
     _pre_acquire = ()
     _post_acquire = ()
@@ -135,16 +135,16 @@
         """Start serial acquisition protocol.
 
         Parameters
         ----------
         start_index : int
             Start acquisition from this item.
         """
-        import time
         import msvcrt
+        import time
 
         ctrl = self.ctrl
         nav_items = self.nav_items[start_index:]
 
         ntot = len(nav_items)
 
         print(f'\nAcquiring on {ntot} items.')
```

### Comparing `instamatic-1.8.0/instamatic/banner.py` & `instamatic-1.9.0/instamatic/banner.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/browser.py` & `instamatic-1.9.0/instamatic/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
         if self.levels > 1:
             self.update_ax2(ind)
         if self.levels > 2:
             self.update_ax3(ind)
 
         if ind == self.current_ind and (t1 - self.t0 < double_click_delay):
-            print(f'Moving stage to:', self.coord)
+            print('Moving stage to:', self.coord)
             self.ctrl.stage.xy = self.coord
 
         self.t0 = time.perf_counter()
         self.current_ind = ind
         self.fig.canvas.draw()
 
     def process_click_ax1(self, ind: int = 0):
```

### Comparing `instamatic-1.8.0/instamatic/calibrate/calibrate_beamshift.py` & `instamatic-1.9.0/instamatic/calibrate/calibrate_beamshift.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import pickle
 import sys
 
 import matplotlib.pyplot as plt
 import numpy as np
 from skimage.registration import phase_cross_correlation
 
-from .filenames import *
-from .fit import fit_affine_transformation
 from instamatic import config
-from instamatic.image_utils import autoscale
-from instamatic.image_utils import imgscale
+from instamatic.image_utils import autoscale, imgscale
 from instamatic.processing.find_holes import find_holes
-from instamatic.tools import find_beam_center
-from instamatic.tools import printer
+from instamatic.tools import find_beam_center, printer
+
+from .filenames import *
+from .fit import fit_affine_transformation
+
 logger = logging.getLogger(__name__)
 
 
 class CalibBeamShift:
     """Simple class to hold the methods to perform transformations from one
     setting to another based on calibration results."""
 
@@ -129,15 +129,14 @@
     binsize: `int` or None
 
     In case paramers are not defined, camera specific default parameters are retrieved
 
     return:
         instance of Calibration class with conversion methods
     """
-
     exposure = kwargs.get('exposure', ctrl.cam.default_exposure)
     binsize = kwargs.get('binsize', ctrl.cam.default_binsize)
 
     if not gridsize:
         gridsize = config.camera.calib_beamshift.get('gridsize', 5)
     if not stepsize:
         stepsize = config.camera.calib_beamshift.get('stepsize', 250)
@@ -166,15 +165,15 @@
     x_grid, y_grid = np.meshgrid(np.arange(-n, n + 1) * stepsize, np.arange(-n, n + 1) * stepsize)
     tot = gridsize * gridsize
 
     i = 0
     for dx, dy in np.stack([x_grid, y_grid]).reshape(2, -1).T:
         ctrl.beamshift.set(x=x_cent + dx, y=y_cent + dy)
 
-        printer('Position: {}/{}: {}'.format(i + 1, tot, ctrl.beamshift))
+        printer(f'Position: {i + 1}/{tot}: {ctrl.beamshift}')
 
         outfile = os.path.join(outdir, 'calib_beamshift_{i:04d}') if save_images else None
 
         comment = f'Calib image {i}: dx={dx} - dy={dy}'
         img, h = ctrl.get_image(exposure=exposure, binsize=binsize, out=outfile, comment=comment, header_keys='BeamShift')
         img = imgscale(img, scale)
```

### Comparing `instamatic-1.8.0/instamatic/calibrate/calibrate_brightness.py` & `instamatic-1.9.0/instamatic/calibrate/calibrate_brightness.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import logging
 import pickle
 import sys
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-from .filenames import *
 from instamatic.image_utils import autoscale
 from instamatic.processing.find_holes import find_holes
 from instamatic.tools import find_beam_center
+
+from .filenames import *
+
 logger = logging.getLogger(__name__)
 
 
 class CalibBrightness:
     """Brightness calibration routine."""
 
     def __init__(self, slope, intercept):
@@ -84,15 +86,14 @@
     exposure: `float`
         exposure time
     binsize: `int`
 
     return:
         instance of CalibBrightness class with conversion methods
     """
-
     raise NotImplementedError('calibrate_brightness_live function needs fixing...')
 
     exposure = kwargs.get('exposure', ctrl.cam.default_exposure)
     binsize = kwargs.get('binsize', ctrl.cam.default_binsize)
 
     values = []
     start = ctrl.brightness.value
@@ -136,15 +137,14 @@
 
     fns: `str`
         Set of images to determine size of beam from
 
     return:
         instance of Calibration class with conversion methods
     """
-
     values = []
 
     for fn in fns:
         print()
         print('Image:', fn)
         img, h = load_img(fn)
         brightness = float(h['Brightness'])
```

### Comparing `instamatic-1.8.0/instamatic/calibrate/calibrate_directbeam.py` & `instamatic-1.9.0/instamatic/calibrate/calibrate_directbeam.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import pickle
 import sys
 
 import matplotlib.pyplot as plt
 import numpy as np
 from skimage.registration import phase_cross_correlation
 
-from .filenames import *
-from .fit import fit_affine_transformation
 from instamatic import config
-from instamatic.image_utils import autoscale
-from instamatic.image_utils import imgscale
+from instamatic.image_utils import autoscale, imgscale
 from instamatic.tools import printer
+
+from .filenames import *
+from .fit import fit_affine_transformation
+
 logger = logging.getLogger(__name__)
 
 
 refine_params = {
     'DiffShift': {'rotation': True, 'translation': False, 'shear': False},
     'BeamShift': {'rotation': True, 'translation': False, 'shear': False},
 }
@@ -191,15 +192,14 @@
     binsize: `int` or None
 
     In case paramers are not defined, camera specific default parameters are
 
     return:
         instance of Calibration class with conversion methods
     """
-
     if ctrl.mode != 'diff':
         print(' >> Switching to diffraction mode')
         ctrl.mode.set('diff')
 
     exposure = kwargs.get('exposure', ctrl.cam.default_exposure)
     binsize = kwargs.get('binsize', ctrl.cam.default_binsize)
```

### Comparing `instamatic-1.8.0/instamatic/calibrate/calibrate_imageshift12.py` & `instamatic-1.9.0/instamatic/calibrate/calibrate_imageshift12.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 
 import numpy as np
 from skimage.registration import phase_cross_correlation
 from tqdm.auto import tqdm
 
 from instamatic.calibrate.fit import fit_affine_transformation
+
 logger = logging.getLogger(__name__)
 
 
 def Calibrate_Imageshift(ctrl, diff_defocus, stepsize, logger, key='IS1'):
-
     if key != 'S':
         input(f"""Calibrate {key}
     -------------------
      1. Go to diffraction mode.
      2. Focus the diffraction spots.
      3. Center the beam with PLA.
```

### Comparing `instamatic-1.8.0/instamatic/calibrate/calibrate_stage_lowmag.py` & `instamatic-1.9.0/instamatic/calibrate/calibrate_stage_lowmag.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import pickle
 import sys
 
 import matplotlib.pyplot as plt
 import numpy as np
 from skimage.registration import phase_cross_correlation
 
+from instamatic.formats import read_image
+from instamatic.image_utils import autoscale, imgscale
+
 from .filenames import *
 from .fit import fit_affine_transformation
-from instamatic.formats import read_image
-from instamatic.image_utils import autoscale
-from instamatic.image_utils import imgscale
+
 logger = logging.getLogger(__name__)
 
 
 class CalibStage:
     """Simple class to hold the methods to perform transformations from one
     setting to another based on calibration results."""
 
@@ -221,15 +222,14 @@
     exposure: `float`
         exposure time
     binsize: `int`
 
     return:
         instance of Calibration class with conversion methods
     """
-
     exposure = kwargs.get('exposure', ctrl.cam.default_exposure)
     binsize = kwargs.get('binsize', ctrl.cam.default_binsize)
 
     outfile = 'calib_start' if save_images else None
 
     # Accurate reading fo the center positions is needed so that we can come back to it,
     #  because this will be our anchor point
```

### Comparing `instamatic-1.8.0/instamatic/calibrate/calibrate_stage_mag1.py` & `instamatic-1.9.0/instamatic/calibrate/calibrate_stage_mag1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 import sys
 import time
 
 import numpy as np
 from skimage.registration import phase_cross_correlation
 
-from .calibrate_stage_lowmag import CalibStage
-from .filenames import *
 from instamatic import config
 from instamatic.formats import read_image
-from instamatic.image_utils import autoscale
-from instamatic.image_utils import imgscale
+from instamatic.image_utils import autoscale, imgscale
 from instamatic.io import get_new_work_subdirectory
+
+from .calibrate_stage_lowmag import CalibStage
+from .filenames import *
+
 logger = logging.getLogger(__name__)
 
 
 def plot_it(arr1, arr2, params):
     import matplotlib.pyplot as plt
     angle = params['angle'].value
     sx = params['sx'].value
@@ -55,15 +56,14 @@
     exposure: `float`
         Exposure time in seconds
     binsize: `int`
 
     return:
         instance of Calibration class with conversion methods
     """
-
     work_drc = get_new_work_subdirectory(stem='calib_mag1')
 
     settle_delay = 1.0  # seconds
 
     # make sure the angle == 0.0
     for _ in range(3):
         ctrl.stage.a = 0.0
```

### Comparing `instamatic-1.8.0/instamatic/calibrate/calibrate_stagematrix.py` & `instamatic-1.9.0/instamatic/calibrate/calibrate_stagematrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import numpy as np
 import yaml
 from scipy import stats
 from skimage.registration import phase_cross_correlation
 
 from instamatic import config
 from instamatic.calibrate.fit import fit_affine_transformation
-from instamatic.formats import read_tiff
-from instamatic.formats import write_tiff
+from instamatic.formats import read_tiff, write_tiff
 from instamatic.image_utils import rotate_image
 from instamatic.io import get_new_work_subdirectory
 
 np.set_printoptions(suppress=True)
 
 data_drc = config.locations['data']
 
@@ -65,15 +64,15 @@
     stagematrix: np.ndarray (2x2)
         Stage matrix used to transform the camera coordinates to stage
         coordinates
     """
     drc = Path(drc)
     fn = drc / 'log.yaml'
 
-    d = yaml.full_load(open(fn, 'r'))
+    d = yaml.full_load(open(fn))
 
     binning = d['binning']
     args = d['args']
 
     stage_shifts = []  # um
     pairs = []
```

### Comparing `instamatic-1.8.0/instamatic/calibrate/center_z.py` & `instamatic-1.9.0/instamatic/calibrate/center_z.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         ctrl.stage.set(a=a_i - 0.5, wait=True)
         return 1
 
 
 def center_z_height(ctrl, verbose=False):
     """Automated routine to find the z-height.
 
-    Koster, A. J., et al. "Automated microscopy for electron tomography."
-    Ultramicroscopy 46.1-4 (1992): 207-227.
+    Koster, A. J., et al. "Automated microscopy for electron
+    tomography." Ultramicroscopy 46.1-4 (1992): 207-227.
     http://www.msg.ucsf.edu/agard/Publications/52-Koster.pdf
     """
     print('\033[k', 'Finding eucentric height...', end='\r')
     if ctrl.mode != 'mag1':
         ctrl.mode.set('mag1')
 
     ctrl.brightness.value = 65535
@@ -85,15 +85,14 @@
             ctrl.stage.set(a=a0, z=z_center + 2000)
             ctrl.stage.set(a=a0, z=z_center)
 
         print('\033[k', 'Eucentric height set. Find the crystal again and start data collection!', end='\r')
 
 
 def find_crystal_max(img, magnification, spread, offset):
-
     crystal_positions = find_crystals_timepix(img, magnification, spread=spread, offset=offset)
     crystal_area = [crystal.area_pixel for crystal in crystal_positions if crystal.isolated]
     maxind = crystal_area.index(max(crystal_area))
 
     crystal_inter = max(crystal_area)
     crystal_inter_pos = (crystal_positions[maxind].x, crystal_positions[maxind].y)
 
@@ -102,15 +101,14 @@
 
 def center_z_height_HYMethod(ctrl, increment=2000, rotation=15, spread=2, offset=10, verbose=False):
     """Hongyi's empirical method for centering z height on our JEOL LAB6.
 
     Rotate the stage positively. If the particle moves upwards, adjust
     height to be higher. Vice versa.
     """
-
     print('\033[k', 'Finding eucentric height...', end='\r')
     if ctrl.mode != 'mag1':
         ctrl.mode.set('mag1')
 
     ctrl.brightness.value = 65535
     ctrl.magnification.value = 2500
     magnification = ctrl.magnification.value
```

### Comparing `instamatic-1.8.0/instamatic/calibrate/fit.py` & `instamatic-1.9.0/instamatic/calibrate/fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from collections import namedtuple
 
 import lmfit
 import numpy as np
 
-
 FitResult = namedtuple('FitResult', 'r t angle sx sy tx ty k1 k2 params'.split())
 
 
 def fit_affine_transformation(a, b,
                               rotation: bool = True,
                               scaling: bool = True,
                               translation: bool = False,
```

### Comparing `instamatic-1.8.0/instamatic/camera/CCDCOM.h` & `instamatic-1.9.0/instamatic/camera/CCDCOM.h`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/camera/CCDCOM2_x64_gatan.dll` & `instamatic-1.9.0/instamatic/camera/CCDCOM2_x64_gatan.dll`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/camera/CCDCOM2_x64_simulation.dll` & `instamatic-1.9.0/instamatic/camera/CCDCOM2_x64_simulation.dll`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/camera/CCDCOM2_x86_gatan.dll` & `instamatic-1.9.0/instamatic/camera/CCDCOM2_x86_gatan.dll`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/camera/CCDCOM2_x86_simulation.dll` & `instamatic-1.9.0/instamatic/camera/CCDCOM2_x86_simulation.dll`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/camera/EMCameraObj.dll` & `instamatic-1.9.0/instamatic/camera/EMCameraObj.dll`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/camera/camera.py` & `instamatic-1.9.0/instamatic/camera/camera.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,196 +1,200 @@
-import logging
-from pathlib import Path
-
-from instamatic import config
-logger = logging.getLogger(__name__)
-
-__all__ = ['Camera']
-
-default_cam_interface = config.camera.interface
-
-
-def get_cam(interface: str = None):
-    """Grabs the camera object defined by `interface`"""
-
-    simulate = config.settings.simulate
-
-    if simulate or interface == 'simulate':
-        from instamatic.camera.camera_simu import CameraSimu as cam
-    elif interface == 'simulateDLL':
-        from instamatic.camera.camera_gatan import CameraDLL as cam
-    elif interface in ('orius', 'gatan'):
-        from instamatic.camera.camera_gatan import CameraDLL as cam
-    elif interface == 'gatansocket':
-        from instamatic.camera.camera_gatan2 import CameraGatan2 as cam
-    elif interface in ('timepix', 'pytimepix'):
-        from instamatic.camera import camera_timepix as cam
-    elif interface in ('emmenu', 'tvips'):
-        from instamatic.camera.camera_emmenu import CameraEMMENU as cam
-    elif interface == 'serval':
-        from instamatic.camera.camera_serval import CameraServal as cam
-    else:
-        raise ValueError(f'No such camera interface: {interface}')
-
-    return cam
-
-
-def Camera(name: str = None, as_stream: bool = False, use_server: bool = False):
-    """Initialize the camera identified by the 'name' parameter if `as_stream`
-    is True, it will return a VideoStream object if `as_stream` is False, it
-    will return the raw Camera object."""
-
-    if name is None:
-        name = config.camera.name
-    elif name != config.settings.camera:
-        # load specific config/interface
-        config.load_camera_config(camera_name=name)
-
-    interface = config.camera.interface
-
-    if use_server:
-        from instamatic.camera.camera_client import CamClient
-        cam = CamClient(name=name, interface=interface)
-        as_stream = False  # precaution
-    else:
-        cam_cls = get_cam(interface)
-
-        if interface in ('timepix', 'pytimepix'):
-            tpx_config = Path(__file__).parent / 'tpx' / 'config.txt'  # TODO: put this somewhere central
-            cam = cam_cls.initialize(tpx_config, name=name)
-        elif interface in ('emmenu', 'tvips'):
-            cam = cam_cls(name=name)
-            as_stream = False  # override `as_stream` for this interface
-        else:
-            cam = cam_cls(name=name)
-
-    if as_stream:
-        if cam.streamable:
-            from .videostream import VideoStream
-        else:
-            from .fakevideostream import VideoStream
-        return VideoStream(cam)
-    else:
-        return cam
-
-
-def main_entry():
-    import argparse
-    from instamatic.formats import write_tiff
-
-    description = """Simple program to acquire image data from the camera."""
-
-    parser = argparse.ArgumentParser(
-        description=description,
-        formatter_class=argparse.RawDescriptionHelpFormatter)
-
-    parser.add_argument('-b', '--binsize',
-                        action='store', type=int, metavar='N', dest='binsize',
-                        help="""Binsize to use. Must be one of 1, 2, or 4 (default 1)""")
-
-    parser.add_argument('-e', '--exposure',
-                        action='store', type=float, metavar='N', dest='exposure',
-                        help="""Exposure time (default 0.5)""")
-
-    parser.add_argument('-o', '--out',
-                        action='store', type=str, metavar='image.png', dest='outfile',
-                        help="""Where to store image""")
-
-    parser.add_argument('-d', '--display',
-                        action='store_true', dest='show_fig',
-                        help="""Show the image (default True)""")
-
-    parser.add_argument('-s', '--series',
-                        action='store_true', dest='take_series',
-                        help="""Enable mode to take a series of images (default False)""")
-
-    parser.set_defaults(
-        binsize=1,
-        exposure=1,
-        outfile=None,
-        show_fig=False,
-        test=False,
-        take_series=False,
-    )
-
-    options = parser.parse_args()
-
-    binsize = options.binsize
-    exposure = options.exposure
-
-    outfile = options.outfile
-    show_fig = options.show_fig
-
-    take_series = options.take_series
-
-    from instamatic import TEMController
-    ctrl = TEMController.initialize()
-
-    if take_series:
-        i = 1
-        print('\nUsage:')
-        print('    set b/e/i X -> set binsize/exposure/file number to X')
-        print('    XXX         -> Add comment to header')
-        print('    exit        -> exit the program')
-    while take_series:
-        outfile = f'image_{i:04d}'
-        inp = input(f'\nHit enter to take an image: \n >> [{outfile}] ')
-        if inp == 'exit':
-            break
-        elif inp.startswith('set'):
-            try:
-                key, value = inp.split()[1:3]
-            except ValueError:
-                print('Input not understood')
-                continue
-            if key == 'e':
-                try:
-                    value = float(value)
-                except ValueError as e:
-                    print(e)
-                if value > 0:
-                    exposure = value
-            elif key == 'b':
-                try:
-                    value = int(value)
-                except ValueError as e:
-                    print(e)
-                if value in (1, 2, 4):
-                    binsize = value
-            elif key == 'i':
-                try:
-                    value = int(value)
-                except ValueError as e:
-                    print(e)
-                if value > 0:
-                    i = value
-            print(f'binsize = {binsize} | exposure = {exposure} | file #{i}')
-        else:
-            arr, h = ctrl.get_image(binsize=binsize, exposure=exposure, comment=inp)
-
-            write_tiff(outfile, arr, header=h)
-
-            i += 1
-    else:
-        import matplotlib.pyplot as plt
-
-        arr, h = ctrl.get_image(binsize=binsize, exposure=exposure)
-
-        if show_fig:
-            plt.imshow(arr, cmap='gray', interpolation='none')
-            plt.show()
-
-        if outfile:
-            write_tiff(outfile, arr, header=h)
-        else:
-            write_tiff('out', arr, header=h)
-
-
-if __name__ == '__main__':
-    # main_entry()
-    cam = Camera(use_server=True)
-    arr = cam.getImage(exposure=0.1)
-    print(arr)
-    print(arr.shape)
-
-    from IPython import embed
-    embed(banner1='')
+import logging
+from pathlib import Path
+
+from instamatic import config
+
+logger = logging.getLogger(__name__)
+
+__all__ = ['Camera']
+
+default_cam_interface = config.camera.interface
+
+
+def get_cam(interface: str = None):
+    """Grabs the camera object defined by `interface`"""
+
+    simulate = config.settings.simulate
+
+    if simulate or interface == 'simulate':
+        from instamatic.camera.camera_simu import CameraSimu as cam
+    elif interface == 'simulateDLL':
+        from instamatic.camera.camera_gatan import CameraDLL as cam
+    elif interface in ('orius', 'gatan'):
+        from instamatic.camera.camera_gatan import CameraDLL as cam
+    elif interface == 'gatansocket':
+        from instamatic.camera.camera_gatan2 import CameraGatan2 as cam
+    elif interface in ('timepix', 'pytimepix'):
+        from instamatic.camera import camera_timepix as cam
+    elif interface in ('emmenu', 'tvips'):
+        from instamatic.camera.camera_emmenu import CameraEMMENU as cam
+    elif interface == 'serval':
+        from instamatic.camera.camera_serval import CameraServal as cam
+    elif interface == 'merlin':
+        from instamatic.camera.camera_merlin import CameraMerlin as cam
+    else:
+        raise ValueError(f'No such camera interface: {interface}')
+
+    return cam
+
+
+def Camera(name: str = None, as_stream: bool = False, use_server: bool = False):
+    """Initialize the camera identified by the 'name' parameter if `as_stream`
+    is True, it will return a VideoStream object if `as_stream` is False, it
+    will return the raw Camera object."""
+
+    if name is None:
+        name = config.camera.name
+    elif name != config.settings.camera:
+        # load specific config/interface
+        config.load_camera_config(camera_name=name)
+
+    interface = config.camera.interface
+
+    if use_server:
+        from instamatic.camera.camera_client import CamClient
+        cam = CamClient(name=name, interface=interface)
+        as_stream = False  # precaution
+    else:
+        cam_cls = get_cam(interface)
+
+        if interface in ('timepix', 'pytimepix'):
+            tpx_config = Path(__file__).parent / 'tpx' / 'config.txt'  # TODO: put this somewhere central
+            cam = cam_cls.initialize(tpx_config, name=name)
+        elif interface in ('emmenu', 'tvips'):
+            cam = cam_cls(name=name)
+            as_stream = False  # override `as_stream` for this interface
+        else:
+            cam = cam_cls(name=name)
+
+    if as_stream:
+        if cam.streamable:
+            from .videostream import VideoStream
+        else:
+            from .fakevideostream import VideoStream
+        return VideoStream(cam)
+    else:
+        return cam
+
+
+def main_entry():
+    import argparse
+
+    from instamatic.formats import write_tiff
+
+    description = """Simple program to acquire image data from the camera."""
+
+    parser = argparse.ArgumentParser(
+        description=description,
+        formatter_class=argparse.RawDescriptionHelpFormatter)
+
+    parser.add_argument('-b', '--binsize',
+                        action='store', type=int, metavar='N', dest='binsize',
+                        help="""Binsize to use. Must be one of 1, 2, or 4 (default 1)""")
+
+    parser.add_argument('-e', '--exposure',
+                        action='store', type=float, metavar='N', dest='exposure',
+                        help="""Exposure time (default 0.5)""")
+
+    parser.add_argument('-o', '--out',
+                        action='store', type=str, metavar='image.png', dest='outfile',
+                        help="""Where to store image""")
+
+    parser.add_argument('-d', '--display',
+                        action='store_true', dest='show_fig',
+                        help="""Show the image (default True)""")
+
+    parser.add_argument('-s', '--series',
+                        action='store_true', dest='take_series',
+                        help="""Enable mode to take a series of images (default False)""")
+
+    parser.set_defaults(
+        binsize=1,
+        exposure=1,
+        outfile=None,
+        show_fig=False,
+        test=False,
+        take_series=False,
+    )
+
+    options = parser.parse_args()
+
+    binsize = options.binsize
+    exposure = options.exposure
+
+    outfile = options.outfile
+    show_fig = options.show_fig
+
+    take_series = options.take_series
+
+    from instamatic import TEMController
+    ctrl = TEMController.initialize()
+
+    if take_series:
+        i = 1
+        print('\nUsage:')
+        print('    set b/e/i X -> set binsize/exposure/file number to X')
+        print('    XXX         -> Add comment to header')
+        print('    exit        -> exit the program')
+    while take_series:
+        outfile = f'image_{i:04d}'
+        inp = input(f'\nHit enter to take an image: \n >> [{outfile}] ')
+        if inp == 'exit':
+            break
+        elif inp.startswith('set'):
+            try:
+                key, value = inp.split()[1:3]
+            except ValueError:
+                print('Input not understood')
+                continue
+            if key == 'e':
+                try:
+                    value = float(value)
+                except ValueError as e:
+                    print(e)
+                if value > 0:
+                    exposure = value
+            elif key == 'b':
+                try:
+                    value = int(value)
+                except ValueError as e:
+                    print(e)
+                if value in (1, 2, 4):
+                    binsize = value
+            elif key == 'i':
+                try:
+                    value = int(value)
+                except ValueError as e:
+                    print(e)
+                if value > 0:
+                    i = value
+            print(f'binsize = {binsize} | exposure = {exposure} | file #{i}')
+        else:
+            arr, h = ctrl.get_image(binsize=binsize, exposure=exposure, comment=inp)
+
+            write_tiff(outfile, arr, header=h)
+
+            i += 1
+    else:
+        import matplotlib.pyplot as plt
+
+        arr, h = ctrl.get_image(binsize=binsize, exposure=exposure)
+
+        if show_fig:
+            plt.imshow(arr, cmap='gray', interpolation='none')
+            plt.show()
+
+        if outfile:
+            write_tiff(outfile, arr, header=h)
+        else:
+            write_tiff('out', arr, header=h)
+
+
+if __name__ == '__main__':
+    # main_entry()
+    cam = Camera(use_server=True)
+    arr = cam.getImage(exposure=0.1)
+    print(arr)
+    print(arr.shape)
+
+    from IPython import embed
+    embed(banner1='')
```

### Comparing `instamatic-1.8.0/instamatic/camera/camera_client.py` & `instamatic-1.9.0/instamatic/camera/camera_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 import subprocess as sp
 import time
 from functools import wraps
 
 import numpy as np
 
 from instamatic import config
-from instamatic.exceptions import exception_list
-from instamatic.exceptions import TEMCommunicationError
+from instamatic.exceptions import TEMCommunicationError, exception_list
 from instamatic.server.serializer import pickle_dumper as dumper
 from instamatic.server.serializer import pickle_loader as loader
 
-
 if config.settings.cam_use_shared_memory:
     from multiprocessing import shared_memory
 
 HOST = config.settings.cam_server_host
 PORT = config.settings.cam_server_port
 BUFSIZE = 4096
 
@@ -96,15 +94,14 @@
 
     def connect(self):
         self.s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.s.connect((HOST, PORT))
         print(f'Connected to CAM server ({HOST}:{PORT})')
 
     def __getattr__(self, attr_name):
-
         if attr_name in self._dct:
             wrapped = self._dct[attr_name]
         elif attr_name in self._attr_dct:
             dct = {'attr_name': attr_name}
             return self._eval_dct(dct)
         else:
             raise AttributeError(f'`{self.__class__.__name__}` object has no attribute `{attr_name}`')
@@ -183,7 +180,13 @@
         if self.verbose:
             print(f'Retrieve data from buffer `{name}`')
 
         buffer = self.buffers[name]
         data = buffer[:]
 
         return data
+
+    def block(self):
+        raise NotImplementedError('This camera cannot be streamed.')
+
+    def unblock(self):
+        raise NotImplementedError('This camera cannot be streamed.')
```

### Comparing `instamatic-1.8.0/instamatic/camera/camera_emmenu.py` & `instamatic-1.9.0/instamatic/camera/camera_emmenu.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 from pathlib import Path
 
 import comtypes.client
 import numpy as np
 
 from instamatic import config
+
 logger = logging.getLogger(__name__)
 
 
 type_dict = {
     1: 'GetDataByte',
     2: 'GetDataUShort',
     3: 'GetDataShort',
```

### Comparing `instamatic-1.8.0/instamatic/camera/camera_gatan.py` & `instamatic-1.9.0/instamatic/camera/camera_gatan.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,230 +1,233 @@
-import atexit
-import ctypes
-import logging
-import platform
-import time
-from ctypes import addressof
-from ctypes import byref
-from ctypes import c_bool
-from ctypes import c_double
-from ctypes import c_float
-from ctypes import c_int
-from ctypes import c_long
-from ctypes import c_wchar_p
-from ctypes import create_unicode_buffer
-from ctypes import POINTER
-from pathlib import Path
-
-import numpy as np
-
-from instamatic import config
-logger = logging.getLogger(__name__)
-
-
-SYMBOLS = {}
-
-if platform.architecture()[0] == '32bit':
-    DLLPATH_SIMU = 'CCDCOM2_x86_simulation.dll'
-    DLLPATH_GATAN = 'CCDCOM2_x86_gatan.dll'
-
-    SYMBOLS['actual'] = {
-        'acquireImageNewFloat': 'acquireImageNewFloat',
-        'acquireImageNewInt': 'acquireImageNewInt',
-        'cameraCount': None,
-        'cameraDimensions': 'cameraDimensions',
-        'cameraName': 'cameraName',
-        'CCDCOM2_release': 'CCDCOM2_release',
-        'initCCDCOM': 'initCCDCOM',
-        'isCameraInfoAvailable': 'isCameraInfoAvailable',
-        'releaseCCDCOM': 'releaseCCDCOM',
-    }
-    SYMBOLS['simu'] = {
-        'acquireImageNewFloat': '?acquireImageNewFloat@@YAHHHHHHN_NPAPAMPAH2@Z',
-        'acquireImageNewInt': '?acquireImageNewInt@@YAHHHHHPAH00HN_N@Z',
-        'cameraCount': '?cameraCount@@YAHXZ',
-        'cameraDimensions': '?cameraDimensions@@YA_NPAH0@Z',
-        'cameraName': '?cameraName@@YA_NPA_WH@Z',
-        'CCDCOM2_release': '?CCDCOM2_release@@YAXPAM@Z',
-        'initCCDCOM': '?initCCDCOM@@YAHH@Z',
-        'isCameraInfoAvailable': '?isCameraInfoAvailable@@YA_NXZ',
-        'releaseCCDCOM': '?releaseCCDCOM@@YAXXZ',
-    }
-else:
-    DLLPATH_SIMU = 'CCDCOM2_x64_simulation.dll'
-    DLLPATH_GATAN = 'CCDCOM2_x64_gatan.dll'
-
-    SYMBOLS['actual'] = {
-        'acquireImageNewFloat': '?acquireImageNewFloat@@YAHHHHHHN_NPEAPEAMPEAH2@Z',
-        'acquireImageNewInt': '?acquireImageNewInt@@YAHHHHHPEAH00HN_N@Z',
-        'cameraCount': '?cameraCount@@YAHXZ',
-        'cameraDimensions': '?cameraDimensions@@YA_NPEAH0@Z',
-        'cameraName': '?cameraName@@YA_NPEA_WH@Z',
-        'CCDCOM2_release': '?CCDCOM2_release@@YAXPEAM@Z',
-        'initCCDCOM': '?initCCDCOM@@YAHH@Z',
-        'isCameraInfoAvailable': '?isCameraInfoAvailable@@YA_NXZ',
-        'releaseCCDCOM': '?releaseCCDCOM@@YAXXZ',
-    }
-
-    SYMBOLS['simu'] = SYMBOLS['actual']
-
-
-class CameraDLL:
-    """Interface with the CCDCOM DLLs to connect to the gatan software."""
-
-    def __init__(self, name: str = 'gatan'):
-        """Initialize camera module.
-
-        name:
-            'gatan'
-            'simulateDLL'
-        """
-        super().__init__()
-
-        cameradir = Path(__file__).parent
-
-        if name == 'simulateDLL':
-            libpath = cameradir / DLLPATH_SIMU
-            symbols = SYMBOLS['simu']
-        elif name == 'gatan':
-            libpath = cameradir / DLLPATH_GATAN
-            symbols = SYMBOLS['actual']
-        else:
-            raise ValueError(f'No such camera: {name}')
-
-        self.name = name
-
-        try:
-            lib = ctypes.cdll.LoadLibrary(str(libpath))
-        except OSError as e:
-            print(e)
-            raise RuntimeError(f'Cannot load DLL: {libpath}')
-
-        # Use dependency walker to get function names from DLL: http://www.dependencywalker.com/
-        self._acquireImageNewFloat = getattr(lib, symbols['acquireImageNewFloat'])
-        self._acquireImageNewFloat.argtypes = [c_int, c_int, c_int, c_int, c_int, c_double, c_bool, POINTER(
-            POINTER(c_float)), POINTER(c_int), POINTER(c_int)]
-
-        # self._cameraCount = getattr(lib, symbols['cameraCount'])
-        # self._cameraCount.restype = c_int
-
-        self._cameraDimensions = getattr(lib, symbols['cameraDimensions'])
-        self._cameraDimensions.argtypes = [POINTER(c_long), POINTER(c_long)]
-
-        self._cameraName = getattr(lib, symbols['cameraName'])
-        self._cameraName.argtypes = [c_wchar_p, c_int]
-        self._cameraName.restype = c_bool
-
-        self._CCDCOM2release = getattr(lib, symbols['CCDCOM2_release'])
-        self._CCDCOM2release.argtypes = [POINTER(c_float)]
-
-        self._initCCDCOM = getattr(lib, symbols['initCCDCOM'])
-        self._initCCDCOM.restype = c_int
-
-        self._isCameraInfoAvailable = getattr(lib, symbols['isCameraInfoAvailable'])
-        self._isCameraInfoAvailable.restype = c_bool
-
-        self._releaseCCDCOM = getattr(lib, symbols['releaseCCDCOM'])
-
-        self.establishConnection()
-
-        self.load_defaults()
-
-        msg = f'Camera {self.getName()} initialized'
-        logger.info(msg)
-
-        # dim_x, dim_y = self.getImageDimensions()
-        # print(f"Dimensions {dim_x}x{dim_y}")
-        # print(f"Info {self.isCameraInfoAvailable()} | Count {self.getCameraCount()}")
-
-        atexit.register(self.releaseConnection)
-
-    def load_defaults(self):
-        if self.name != config.settings.camera:
-            config.load_camera_config(camera_name=self.name)
-
-        self.__dict__.update(config.camera.mapping)
-
-        self.streamable = False
-
-    def getImage(self, exposure=None, binsize=None, **kwargs) -> np.ndarray:
-        """Image acquisition routine.
-
-        exposure: exposure time in seconds
-        binsize: which binning to use
-        showindm: show image in digital micrograph
-        xmin, xmax, ymin, ymax: retrieve image with smaller size from a subset of pixels
-        """
-
-        if not exposure:
-            exposure = self.default_exposure
-        if not binsize:
-            binsize = self.default_binsize
-
-        xmin = kwargs.get('xmin', 0)
-        xmax = kwargs.get('xmax', self.dimensions[0])
-        ymin = kwargs.get('ymin', 0)
-        ymax = kwargs.get('ymax', self.dimensions[1])
-        showindm = kwargs.get('showindm', False)
-
-        if binsize not in self.possible_binsizes:
-            raise ValueError(
-                f'Cannot use binsize={binsize}..., should be one of {self.possible_binsizes}')
-
-        pdata = POINTER(c_float)()
-        pnImgWidth = c_int(0)
-        pnImgHeight = c_int(0)
-        self._acquireImageNewFloat(ymin, xmin, ymax, xmax, binsize, exposure, showindm, byref(
-            pdata), byref(pnImgWidth), byref(pnImgHeight))
-        xres = pnImgWidth.value
-        yres = pnImgHeight.value
-        print(f'shape: {xres} {yres}, binsize: {binsize}')
-        arr = np.ctypeslib.as_array(
-            (c_float * xres * yres).from_address(addressof(pdata.contents)))
-        # memory is not shared between python and C, so we need to copy array
-        arr = arr.copy()
-        # next we can release pdata memory so that it isn't kept in memory
-        self._CCDCOM2release(pdata)
-
-        if self.name == 'simulateDLL':
-            # add some noise to static simulated images
-            arr *= np.random.random((xres, yres)) + 0.5
-            time.sleep(exposure)
-
-        return arr
-
-    def isCameraInfoAvailable(self) -> bool:
-        """Return the status of the camera."""
-        return self._isCameraInfoAvailable()
-
-    def getCameraDimensions(self) -> (int, int):
-        """Return the dimensions reported by the camera."""
-        pnWidth = c_int(0)
-        pnHeight = c_int(0)
-        self._cameraDimensions(byref(pnWidth), byref(pnHeight))
-        return pnWidth.value, pnHeight.value
-
-    def getName(self) -> str:
-        """Return the name reported by the camera."""
-        buf = create_unicode_buffer(20)
-        self._cameraName(buf, 20)
-        return buf.value
-
-    def establishConnection(self) -> None:
-        """Establish connection to the camera."""
-        res = self._initCCDCOM(20120101)
-        if res != 1:
-            raise RuntimeError(f'Could not establish camera connection to {self.name}')
-
-    def releaseConnection(self) -> None:
-        """Release the connection to the camera."""
-        name = self.getName()
-        self._releaseCCDCOM()
-        msg = f'Connection to camera {name} released'
-        logger.info(msg)
-
-
-if __name__ == '__main__':
-    cam = CameraDLL()
-
-    from IPython import embed
-    embed()
+import atexit
+import ctypes
+import logging
+import platform
+import time
+from ctypes import (
+    POINTER,
+    addressof,
+    byref,
+    c_bool,
+    c_double,
+    c_float,
+    c_int,
+    c_long,
+    c_wchar_p,
+    create_unicode_buffer,
+)
+from pathlib import Path
+
+import numpy as np
+
+from instamatic import config
+
+logger = logging.getLogger(__name__)
+
+
+SYMBOLS = {}
+
+if platform.architecture()[0] == '32bit':
+    DLLPATH_SIMU = 'CCDCOM2_x86_simulation.dll'
+    DLLPATH_GATAN = 'CCDCOM2_x86_gatan.dll'
+
+    SYMBOLS['actual'] = {
+        'acquireImageNewFloat': 'acquireImageNewFloat',
+        'acquireImageNewInt': 'acquireImageNewInt',
+        'cameraCount': None,
+        'cameraDimensions': 'cameraDimensions',
+        'cameraName': 'cameraName',
+        'CCDCOM2_release': 'CCDCOM2_release',
+        'initCCDCOM': 'initCCDCOM',
+        'isCameraInfoAvailable': 'isCameraInfoAvailable',
+        'releaseCCDCOM': 'releaseCCDCOM',
+    }
+    SYMBOLS['simu'] = {
+        'acquireImageNewFloat': '?acquireImageNewFloat@@YAHHHHHHN_NPAPAMPAH2@Z',
+        'acquireImageNewInt': '?acquireImageNewInt@@YAHHHHHPAH00HN_N@Z',
+        'cameraCount': '?cameraCount@@YAHXZ',
+        'cameraDimensions': '?cameraDimensions@@YA_NPAH0@Z',
+        'cameraName': '?cameraName@@YA_NPA_WH@Z',
+        'CCDCOM2_release': '?CCDCOM2_release@@YAXPAM@Z',
+        'initCCDCOM': '?initCCDCOM@@YAHH@Z',
+        'isCameraInfoAvailable': '?isCameraInfoAvailable@@YA_NXZ',
+        'releaseCCDCOM': '?releaseCCDCOM@@YAXXZ',
+    }
+else:
+    DLLPATH_SIMU = 'CCDCOM2_x64_simulation.dll'
+    DLLPATH_GATAN = 'CCDCOM2_x64_gatan.dll'
+
+    SYMBOLS['actual'] = {
+        'acquireImageNewFloat': '?acquireImageNewFloat@@YAHHHHHHN_NPEAPEAMPEAH2@Z',
+        'acquireImageNewInt': '?acquireImageNewInt@@YAHHHHHPEAH00HN_N@Z',
+        'cameraCount': '?cameraCount@@YAHXZ',
+        'cameraDimensions': '?cameraDimensions@@YA_NPEAH0@Z',
+        'cameraName': '?cameraName@@YA_NPEA_WH@Z',
+        'CCDCOM2_release': '?CCDCOM2_release@@YAXPEAM@Z',
+        'initCCDCOM': '?initCCDCOM@@YAHH@Z',
+        'isCameraInfoAvailable': '?isCameraInfoAvailable@@YA_NXZ',
+        'releaseCCDCOM': '?releaseCCDCOM@@YAXXZ',
+    }
+
+    SYMBOLS['simu'] = SYMBOLS['actual']
+
+
+class CameraDLL:
+    """Interface with the CCDCOM DLLs to connect to the gatan software."""
+
+    def __init__(self, name: str = 'gatan'):
+        """Initialize camera module.
+
+        name:
+            'gatan'
+            'simulateDLL'
+        """
+        super().__init__()
+
+        cameradir = Path(__file__).parent
+
+        if name == 'simulateDLL':
+            libpath = cameradir / DLLPATH_SIMU
+            symbols = SYMBOLS['simu']
+        elif name == 'gatan':
+            libpath = cameradir / DLLPATH_GATAN
+            symbols = SYMBOLS['actual']
+        else:
+            raise ValueError(f'No such camera: {name}')
+
+        self.name = name
+
+        try:
+            lib = ctypes.cdll.LoadLibrary(str(libpath))
+        except OSError as e:
+            print(e)
+            raise RuntimeError(f'Cannot load DLL: {libpath}')
+
+        # Use dependency walker to get function names from DLL: http://www.dependencywalker.com/
+        self._acquireImageNewFloat = getattr(lib, symbols['acquireImageNewFloat'])
+        self._acquireImageNewFloat.argtypes = [c_int, c_int, c_int, c_int, c_int, c_double, c_bool, POINTER(
+            POINTER(c_float)), POINTER(c_int), POINTER(c_int)]
+
+        # self._cameraCount = getattr(lib, symbols['cameraCount'])
+        # self._cameraCount.restype = c_int
+
+        self._cameraDimensions = getattr(lib, symbols['cameraDimensions'])
+        self._cameraDimensions.argtypes = [POINTER(c_long), POINTER(c_long)]
+
+        self._cameraName = getattr(lib, symbols['cameraName'])
+        self._cameraName.argtypes = [c_wchar_p, c_int]
+        self._cameraName.restype = c_bool
+
+        self._CCDCOM2release = getattr(lib, symbols['CCDCOM2_release'])
+        self._CCDCOM2release.argtypes = [POINTER(c_float)]
+
+        self._initCCDCOM = getattr(lib, symbols['initCCDCOM'])
+        self._initCCDCOM.restype = c_int
+
+        self._isCameraInfoAvailable = getattr(lib, symbols['isCameraInfoAvailable'])
+        self._isCameraInfoAvailable.restype = c_bool
+
+        self._releaseCCDCOM = getattr(lib, symbols['releaseCCDCOM'])
+
+        self.establishConnection()
+
+        self.load_defaults()
+
+        msg = f'Camera {self.getName()} initialized'
+        logger.info(msg)
+
+        # dim_x, dim_y = self.getImageDimensions()
+        # print(f"Dimensions {dim_x}x{dim_y}")
+        # print(f"Info {self.isCameraInfoAvailable()} | Count {self.getCameraCount()}")
+
+        atexit.register(self.releaseConnection)
+
+    def load_defaults(self):
+        if self.name != config.settings.camera:
+            config.load_camera_config(camera_name=self.name)
+
+        self.__dict__.update(config.camera.mapping)
+
+        self.streamable = False
+
+    def getImage(self, exposure=None, binsize=None, **kwargs) -> np.ndarray:
+        """Image acquisition routine.
+
+        exposure: exposure time in seconds
+        binsize: which binning to use
+        showindm: show image in digital micrograph
+        xmin, xmax, ymin, ymax: retrieve image with smaller size from a subset of pixels
+        """
+
+        if not exposure:
+            exposure = self.default_exposure
+        if not binsize:
+            binsize = self.default_binsize
+
+        xmin = kwargs.get('xmin', 0)
+        xmax = kwargs.get('xmax', self.dimensions[0])
+        ymin = kwargs.get('ymin', 0)
+        ymax = kwargs.get('ymax', self.dimensions[1])
+        showindm = kwargs.get('showindm', False)
+
+        if binsize not in self.possible_binsizes:
+            raise ValueError(
+                f'Cannot use binsize={binsize}..., should be one of {self.possible_binsizes}')
+
+        pdata = POINTER(c_float)()
+        pnImgWidth = c_int(0)
+        pnImgHeight = c_int(0)
+        self._acquireImageNewFloat(ymin, xmin, ymax, xmax, binsize, exposure, showindm, byref(
+            pdata), byref(pnImgWidth), byref(pnImgHeight))
+        xres = pnImgWidth.value
+        yres = pnImgHeight.value
+        print(f'shape: {xres} {yres}, binsize: {binsize}')
+        arr = np.ctypeslib.as_array(
+            (c_float * xres * yres).from_address(addressof(pdata.contents)))
+        # memory is not shared between python and C, so we need to copy array
+        arr = arr.copy()
+        # next we can release pdata memory so that it isn't kept in memory
+        self._CCDCOM2release(pdata)
+
+        if self.name == 'simulateDLL':
+            # add some noise to static simulated images
+            arr *= np.random.random((xres, yres)) + 0.5
+            time.sleep(exposure)
+
+        return arr
+
+    def isCameraInfoAvailable(self) -> bool:
+        """Return the status of the camera."""
+        return self._isCameraInfoAvailable()
+
+    def getCameraDimensions(self) -> (int, int):
+        """Return the dimensions reported by the camera."""
+        pnWidth = c_int(0)
+        pnHeight = c_int(0)
+        self._cameraDimensions(byref(pnWidth), byref(pnHeight))
+        return pnWidth.value, pnHeight.value
+
+    def getName(self) -> str:
+        """Return the name reported by the camera."""
+        buf = create_unicode_buffer(20)
+        self._cameraName(buf, 20)
+        return buf.value
+
+    def establishConnection(self) -> None:
+        """Establish connection to the camera."""
+        res = self._initCCDCOM(20120101)
+        if res != 1:
+            raise RuntimeError(f'Could not establish camera connection to {self.name}')
+
+    def releaseConnection(self) -> None:
+        """Release the connection to the camera."""
+        name = self.getName()
+        self._releaseCCDCOM()
+        msg = f'Connection to camera {name} released'
+        logger.info(msg)
+
+
+if __name__ == '__main__':
+    cam = CameraDLL()
+
+    from IPython import embed
+    embed()
```

### Comparing `instamatic-1.8.0/instamatic/camera/camera_gatan2.py` & `instamatic-1.9.0/instamatic/camera/camera_gatan2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 from pathlib import Path
 
 import numpy as np
 
 from instamatic import config
 from instamatic.camera.gatansocket3 import GatanSocket
+
 logger = logging.getLogger(__name__)
 
 
 class CameraGatan2:
     """Connect to Digital Microsgraph using the SerialEM Plugin."""
 
     def __init__(self, name: str = 'gatan2'):
@@ -174,15 +175,14 @@
     def get_tag(self, key: str, delete: bool = False) -> float:
         """Get the tag given by `key`.
 
         Clear the tag if `delete` is specfified`
         get_tag = f'number value\nGetPersistentNumberNote("{key}", value)\nExit(value)'
         value = self.g.ExecuteGetDoubleScript(get_tag)
         """
-
         if delete:
             self.delete_tag(key)
 
         return value
 
     def delete_tag(self, key: str) -> None:
         """Delete the tag `key` in DM."""
```

### Comparing `instamatic-1.8.0/instamatic/camera/camera_serval.py` & `instamatic-1.9.0/instamatic/camera/camera_serval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,157 +1,158 @@
-import atexit
-import logging
-from pathlib import Path
-
-import numpy as np
-from serval_toolkit.camera import Camera as ServalCamera
-
-from instamatic import config
-logger = logging.getLogger(__name__)
-
-# Start servers in serval_toolkit:
-# 1. `java -jar .\emu\tpx3_emu.jar`
-# 2. `java -jar .\server\serv-2.1.3.jar`
-# 3. launch `instamatic`
-
-
-class CameraServal:
-    """Interfaces with Serval from ASI."""
-
-    def __init__(self, name='serval'):
-        """Initialize camera module."""
-        super().__init__()
-
-        self.name = name
-
-        self.load_defaults()
-
-        self.establishConnection()
-
-        msg = f'Camera {self.getName()} initialized'
-        logger.info(msg)
-
-        atexit.register(self.releaseConnection)
-
-    def load_defaults(self):
-        if self.name != config.settings.camera:
-            config.load_camera_config(camera_name=self.name)
-
-        self.streamable = True
-
-        self.__dict__.update(config.camera.mapping)
-
-    def getImage(self, exposure=None, binsize=None, **kwargs) -> np.ndarray:
-        """Image acquisition routine. If the exposure and binsize are not
-        given, the default values are read from the config file.
-
-        exposure:
-            Exposure time in seconds.
-        binsize:
-            Which binning to use.
-        """
-        if exposure is None:
-            exposure = self.default_exposure
-        if not binsize:
-            binsize = self.default_binsize
-
-        # Upload exposure settings (Note: will do nothing if no change in settings)
-        self.conn.set_detector_config(ExposureTime=exposure,
-                TriggerPeriod=exposure + 0.00050001)
-
-        # Check if measurement is running. If not: start
-        db = self.conn.dashboard
-        if db['Measurement'] is None or db['Measurement']['Status'] != 'DA_RECORDING':
-            self.conn.measurement_start()
-
-        # Start the acquisition
-        self.conn.trigger_start()
-
-        # Request a frame. Will be streamed *after* the exposure finishes
-        img = self.conn.get_image_stream(nTriggers = 1, disable_tqdm = True)[0]
-        arr = np.array(img)
-        return arr
-
-    def getMovie(self, n_frames, exposure=None, binsize=None, **kwargs):
-        """Movie acquisition routine. If the exposure and binsize are not
-        given, the default values are read from the config file.
-
-        n_frames:
-            Number of frames to collect
-        exposure:
-            Exposure time in seconds.
-        binsize:
-            Which binning to use.
-        """
-        if exposure is None:
-            exposure = self.default_exposure
-        if not binsize:
-            binsize = self.default_binsize
-
-        self.conn.set_detector_config(TriggerMode = 'CONTINUOUS')
-
-        arr = self.conn.get_images(
-            nTriggers=n_frames,
-            ExposureTime=exposure,
-            TriggerPeriod=exposure,
-        )
-
-        return arr
-
-    def getImageDimensions(self) -> (int, int):
-        """Get the binned dimensions reported by the camera."""
-        binning = self.getBinning()
-        dim_x, dim_y = self.getCameraDimensions()
-
-        dim_x = int(dim_x / binning)
-        dim_y = int(dim_y / binning)
-
-        return dim_x, dim_y
-
-    def getCameraDimensions(self) -> (int, int):
-        """Get the dimensions reported by the camera."""
-        return self.dimensions
-
-    def getName(self) -> str:
-        """Get the name reported by the camera."""
-        return self.name
-
-    def establishConnection(self) -> None:
-        """Establish connection to the camera."""
-        self.conn = ServalCamera()
-        self.conn.connect(self.url)
-        self.conn.set_chip_config_files(
-            bpc_file_path=self.bpc_file_path,
-            dacs_file_path=self.dacs_file_path)
-        self.conn.set_detector_config(**self.detector_config)
-        # Check pixel depth. If 24 bit mode is used, the pgm format does not work
-        # (has support up to 16 bits) so use tiff in that case. In other cases (1, 6, 12 bits)
-        # use pgm since it is more efficient
-        self.pixel_depth = self.conn.detector_config['PixelDepth']
-        if self.pixel_depth == 24:
-            file_format = 'tiff'
-        else:
-            file_format = 'pgm'
-        self.conn.destination = {
-                "Image":
-                    [{
-                    # Where to place the preview files (HTTP end-point: GET localhost:8080/measurement/image)
-                    "Base": "http://localhost",
-                    # What (image) format to provide the files in.
-                    "Format": file_format,
-                    # What data to build a frame from
-                    "Mode": "count"
-            }]
-        }
-
-    def releaseConnection(self) -> None:
-        """Release the connection to the camera."""
-        self.conn.measurement_stop()
-        name = self.getName()
-        msg = f"Connection to camera '{name}' released"
-        logger.info(msg)
-
-
-if __name__ == '__main__':
-    cam = CameraServal()
-    from IPython import embed
-    embed()
+import atexit
+import logging
+from pathlib import Path
+
+import numpy as np
+from serval_toolkit.camera import Camera as ServalCamera
+
+from instamatic import config
+
+logger = logging.getLogger(__name__)
+
+# Start servers in serval_toolkit:
+# 1. `java -jar .\emu\tpx3_emu.jar`
+# 2. `java -jar .\server\serv-2.1.3.jar`
+# 3. launch `instamatic`
+
+
+class CameraServal:
+    """Interfaces with Serval from ASI."""
+
+    def __init__(self, name='serval'):
+        """Initialize camera module."""
+        super().__init__()
+
+        self.name = name
+
+        self.load_defaults()
+
+        self.establishConnection()
+
+        msg = f'Camera {self.getName()} initialized'
+        logger.info(msg)
+
+        atexit.register(self.releaseConnection)
+
+    def load_defaults(self):
+        if self.name != config.settings.camera:
+            config.load_camera_config(camera_name=self.name)
+
+        self.streamable = True
+
+        self.__dict__.update(config.camera.mapping)
+
+    def getImage(self, exposure=None, binsize=None, **kwargs) -> np.ndarray:
+        """Image acquisition routine. If the exposure and binsize are not
+        given, the default values are read from the config file.
+
+        exposure:
+            Exposure time in seconds.
+        binsize:
+            Which binning to use.
+        """
+        if exposure is None:
+            exposure = self.default_exposure
+        if not binsize:
+            binsize = self.default_binsize
+
+        # Upload exposure settings (Note: will do nothing if no change in settings)
+        self.conn.set_detector_config(ExposureTime=exposure,
+                                      TriggerPeriod=exposure + 0.00050001)
+
+        # Check if measurement is running. If not: start
+        db = self.conn.dashboard
+        if db['Measurement'] is None or db['Measurement']['Status'] != 'DA_RECORDING':
+            self.conn.measurement_start()
+
+        # Start the acquisition
+        self.conn.trigger_start()
+
+        # Request a frame. Will be streamed *after* the exposure finishes
+        img = self.conn.get_image_stream(nTriggers=1, disable_tqdm=True)[0]
+        arr = np.array(img)
+        return arr
+
+    def getMovie(self, n_frames, exposure=None, binsize=None, **kwargs):
+        """Movie acquisition routine. If the exposure and binsize are not
+        given, the default values are read from the config file.
+
+        n_frames:
+            Number of frames to collect
+        exposure:
+            Exposure time in seconds.
+        binsize:
+            Which binning to use.
+        """
+        if exposure is None:
+            exposure = self.default_exposure
+        if not binsize:
+            binsize = self.default_binsize
+
+        self.conn.set_detector_config(TriggerMode='CONTINUOUS')
+
+        arr = self.conn.get_images(
+            nTriggers=n_frames,
+            ExposureTime=exposure,
+            TriggerPeriod=exposure,
+        )
+
+        return arr
+
+    def getImageDimensions(self) -> (int, int):
+        """Get the binned dimensions reported by the camera."""
+        binning = self.getBinning()
+        dim_x, dim_y = self.getCameraDimensions()
+
+        dim_x = int(dim_x / binning)
+        dim_y = int(dim_y / binning)
+
+        return dim_x, dim_y
+
+    def getCameraDimensions(self) -> (int, int):
+        """Get the dimensions reported by the camera."""
+        return self.dimensions
+
+    def getName(self) -> str:
+        """Get the name reported by the camera."""
+        return self.name
+
+    def establishConnection(self) -> None:
+        """Establish connection to the camera."""
+        self.conn = ServalCamera()
+        self.conn.connect(self.url)
+        self.conn.set_chip_config_files(
+            bpc_file_path=self.bpc_file_path,
+            dacs_file_path=self.dacs_file_path)
+        self.conn.set_detector_config(**self.detector_config)
+        # Check pixel depth. If 24 bit mode is used, the pgm format does not work
+        # (has support up to 16 bits) so use tiff in that case. In other cases (1, 6, 12 bits)
+        # use pgm since it is more efficient
+        self.pixel_depth = self.conn.detector_config['PixelDepth']
+        if self.pixel_depth == 24:
+            file_format = 'tiff'
+        else:
+            file_format = 'pgm'
+        self.conn.destination = {
+            'Image':
+            [{
+                # Where to place the preview files (HTTP end-point: GET localhost:8080/measurement/image)
+                'Base': 'http://localhost',
+                        # What (image) format to provide the files in.
+                        'Format': file_format,
+                        # What data to build a frame from
+                        'Mode': 'count',
+            }],
+        }
+
+    def releaseConnection(self) -> None:
+        """Release the connection to the camera."""
+        self.conn.measurement_stop()
+        name = self.getName()
+        msg = f"Connection to camera '{name}' released"
+        logger.info(msg)
+
+
+if __name__ == '__main__':
+    cam = CameraServal()
+    from IPython import embed
+    embed()
```

### Comparing `instamatic-1.8.0/instamatic/camera/camera_simu.py` & `instamatic-1.9.0/instamatic/camera/camera_simu.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,167 +1,168 @@
-import atexit
-import logging
-import time
-
-import numpy as np
-
-from instamatic import config
-logger = logging.getLogger(__name__)
-
-
-class CameraSimu:
-    """Simple class that simulates the camera interface and mocks the method
-    calls."""
-
-    def __init__(self, name='simulate'):
-        """Initialize camera module."""
-        super().__init__()
-
-        self.name = name
-
-        self.establishConnection()
-
-        self.load_defaults()
-
-        msg = f'Camera {self.getName()} initialized'
-        logger.info(msg)
-
-        atexit.register(self.releaseConnection)
-
-        # EMMENU variables
-        self._image_index = 0
-        self._exposure = self.default_exposure
-        self._autoincrement = True
-        self._start_record_time = -1
-
-    def load_defaults(self):
-        if self.name != config.settings.camera:
-            config.load_camera_config(camera_name=self.name)
-
-        self.streamable = True
-
-        self.__dict__.update(config.camera.mapping)
-
-    def getImage(self, exposure=None, binsize=None, **kwargs) -> np.ndarray:
-        """Image acquisition routine. If the exposure and binsize are not
-        given, the default values are read from the config file.
-
-        exposure:
-            Exposure time in seconds.
-        binsize:
-            Which binning to use.
-        """
-
-        if exposure is None:
-            exposure = self.default_exposure
-        if not binsize:
-            binsize = self.default_binsize
-
-        dim_x, dim_y = self.getCameraDimensions()
-
-        dim_x = int(dim_x / binsize)
-        dim_y = int(dim_y / binsize)
-
-        time.sleep(exposure)
-
-        arr = np.random.randint(256, size=(dim_x, dim_y))
-
-        return arr
-
-    def acquireImage(self) -> int:
-        """For TVIPS compatibility."""
-        return 1
-
-    def isCameraInfoAvailable(self) -> bool:
-        """Check if the camera is available."""
-        return True
-
-    def getImageDimensions(self) -> (int, int):
-        """Get the binned dimensions reported by the camera."""
-        binning = self.getBinning()
-        dim_x, dim_y = self.getCameraDimensions()
-
-        dim_x = int(dim_x / binning)
-        dim_y = int(dim_y / binning)
-
-        return dim_x, dim_y
-
-    def getCameraDimensions(self) -> (int, int):
-        """Get the dimensions reported by the camera."""
-        return self.dimensions
-
-    def getName(self) -> str:
-        """Get the name reported by the camera."""
-        return self.name
-
-    def establishConnection(self) -> None:
-        """Establish connection to the camera."""
-        res = 1
-        if res != 1:
-            raise RuntimeError(f'Could not establish camera connection to {self.name}')
-
-    def releaseConnection(self) -> None:
-        """Release the connection to the camera."""
-        name = self.getName()
-        msg = f"Connection to camera '{name}' released"
-        logger.info(msg)
-
-    # Mimic EMMENU API
-
-    def getEMMenuVersion(self) -> str:
-        return 'simu'
-
-    def getCameraType(self) -> str:
-        return 'SimuType'
-
-    def getCurrentConfigName(self) -> str:
-        return 'SimuCfg'
-
-    def set_autoincrement(self, value):
-        self._autoincrement = value
-
-    def get_autoincrement(self):
-        return self._autoincrement
-
-    def set_image_index(self, value):
-        self._image_index = value
-
-    def get_image_index(self):
-        return self._image_index
-
-    def stop_record(self) -> None:
-        t1 = self._start_record_time
-        if t1 >= 0:
-            t2 = time.perf_counter()
-            n_images = int((t2 - t1) / self._exposure)
-            new_index = self.get_image_index() + n_images
-            self.set_image_index(new_index)
-            print('stop_record', t1, t2, self._exposure, new_index)
-            self._start_record_time = -1
-        else:
-            pass
-
-    def start_record(self) -> None:
-        self._start_record_time = time.perf_counter()
-
-    def stop_liveview(self) -> None:
-        self.stop_record()
-        print('Liveview stopped')
-
-    def start_liveview(self, delay=3.0) -> None:
-        time.sleep(delay)
-        print('Liveview started')
-
-    def set_exposure(self, exposure_time: int) -> None:
-        self._exposure = exposure_time / 1000
-
-    def get_exposure(self) -> int:
-        return self._exposure
-
-    def get_timestamps(self, start_index, end_index):
-        return list(range(20))
-
-    def getBinning(self):
-        return self.default_binsize
-
-    def writeTiffs(self, start_index: int, stop_index: int, path: str, clear_buffer=True) -> None:
-        pass
+import atexit
+import logging
+import time
+
+import numpy as np
+
+from instamatic import config
+
+logger = logging.getLogger(__name__)
+
+
+class CameraSimu:
+    """Simple class that simulates the camera interface and mocks the method
+    calls."""
+
+    def __init__(self, name='simulate'):
+        """Initialize camera module."""
+        super().__init__()
+
+        self.name = name
+
+        self.establishConnection()
+
+        self.load_defaults()
+
+        msg = f'Camera {self.getName()} initialized'
+        logger.info(msg)
+
+        atexit.register(self.releaseConnection)
+
+        # EMMENU variables
+        self._image_index = 0
+        self._exposure = self.default_exposure
+        self._autoincrement = True
+        self._start_record_time = -1
+
+    def load_defaults(self):
+        if self.name != config.settings.camera:
+            config.load_camera_config(camera_name=self.name)
+
+        self.streamable = True
+
+        self.__dict__.update(config.camera.mapping)
+
+    def getImage(self, exposure=None, binsize=None, **kwargs) -> np.ndarray:
+        """Image acquisition routine. If the exposure and binsize are not
+        given, the default values are read from the config file.
+
+        exposure:
+            Exposure time in seconds.
+        binsize:
+            Which binning to use.
+        """
+
+        if exposure is None:
+            exposure = self.default_exposure
+        if not binsize:
+            binsize = self.default_binsize
+
+        dim_x, dim_y = self.getCameraDimensions()
+
+        dim_x = int(dim_x / binsize)
+        dim_y = int(dim_y / binsize)
+
+        time.sleep(exposure)
+
+        arr = np.random.randint(256, size=(dim_x, dim_y))
+
+        return arr
+
+    def acquireImage(self) -> int:
+        """For TVIPS compatibility."""
+        return 1
+
+    def isCameraInfoAvailable(self) -> bool:
+        """Check if the camera is available."""
+        return True
+
+    def getImageDimensions(self) -> (int, int):
+        """Get the binned dimensions reported by the camera."""
+        binning = self.getBinning()
+        dim_x, dim_y = self.getCameraDimensions()
+
+        dim_x = int(dim_x / binning)
+        dim_y = int(dim_y / binning)
+
+        return dim_x, dim_y
+
+    def getCameraDimensions(self) -> (int, int):
+        """Get the dimensions reported by the camera."""
+        return self.dimensions
+
+    def getName(self) -> str:
+        """Get the name reported by the camera."""
+        return self.name
+
+    def establishConnection(self) -> None:
+        """Establish connection to the camera."""
+        res = 1
+        if res != 1:
+            raise RuntimeError(f'Could not establish camera connection to {self.name}')
+
+    def releaseConnection(self) -> None:
+        """Release the connection to the camera."""
+        name = self.getName()
+        msg = f"Connection to camera '{name}' released"
+        logger.info(msg)
+
+    # Mimic EMMENU API
+
+    def getEMMenuVersion(self) -> str:
+        return 'simu'
+
+    def getCameraType(self) -> str:
+        return 'SimuType'
+
+    def getCurrentConfigName(self) -> str:
+        return 'SimuCfg'
+
+    def set_autoincrement(self, value):
+        self._autoincrement = value
+
+    def get_autoincrement(self):
+        return self._autoincrement
+
+    def set_image_index(self, value):
+        self._image_index = value
+
+    def get_image_index(self):
+        return self._image_index
+
+    def stop_record(self) -> None:
+        t1 = self._start_record_time
+        if t1 >= 0:
+            t2 = time.perf_counter()
+            n_images = int((t2 - t1) / self._exposure)
+            new_index = self.get_image_index() + n_images
+            self.set_image_index(new_index)
+            print('stop_record', t1, t2, self._exposure, new_index)
+            self._start_record_time = -1
+        else:
+            pass
+
+    def start_record(self) -> None:
+        self._start_record_time = time.perf_counter()
+
+    def stop_liveview(self) -> None:
+        self.stop_record()
+        print('Liveview stopped')
+
+    def start_liveview(self, delay=3.0) -> None:
+        time.sleep(delay)
+        print('Liveview started')
+
+    def set_exposure(self, exposure_time: int) -> None:
+        self._exposure = exposure_time / 1000
+
+    def get_exposure(self) -> int:
+        return self._exposure
+
+    def get_timestamps(self, start_index, end_index):
+        return list(range(20))
+
+    def getBinning(self):
+        return self.default_binsize
+
+    def writeTiffs(self, start_index: int, stop_index: int, path: str, clear_buffer=True) -> None:
+        pass
```

### Comparing `instamatic-1.8.0/instamatic/camera/camera_timepix.py` & `instamatic-1.9.0/instamatic/camera/camera_timepix.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ctypes import *
 from pathlib import Path
 
 import numpy as np
 
 from instamatic import config
 from instamatic.utils import high_precision_timers
+
 high_precision_timers.enable()
 
 # SoPhy > File > Medipix/Timepix control > Save parametrized settings
 # Save updated config for timepix camera
 CONFIG_PYTIMEPIX = 'tpx'
 
 
@@ -214,15 +215,14 @@
 
     def readMatrix(self, arr=None, sz=512 * 512):
         """Reads a frame from all connected devices, decodes the data and
         stores the pixel counts in array data.
 
         i16 *data # data storage array u32 sz    # size of array
         """
-
         if arr is None:
             arr = np.empty(sz, dtype=np.int16)
 
         ref = np.ctypeslib.as_ctypes(arr)
         sz = ctypes.c_uint32(sz)
 
         # readout speed
@@ -236,36 +236,33 @@
         time-out to us microseconds. Note that the timer resolution is 10 us.
         After the Relaxd shutter opens (either explicitly by software or by an
         external trigger), it closes again after the set time.
 
         bool enable
         int us = 10 # microseconds
         """
-
         enable = c_bool(enable)
         us = c_int(us)
 
         self.lib.EMCameraObj_enableTimer(self.obj, enable, us)
 
     def resetMatrix(self):
         self.lib.EMCameraObj_resetMatrix(self.obj)
 
     def timerExpired(self):
         return self.lib.EMCameraObj_timerExpired(self.obj)
 
     def setAcqPars(self, pars):
         """AcqParams *pars."""
-
         raise NotImplementedError
         pars = AcqParams
         self.lib.EMCameraObj_setAcqPars(self.obj, byref(pars))
 
     def isBusy(self, busy):
         """bool *busy."""
-
         busy = c_bool(busy)
         self.lib.EMCameraObj_isBusy(self.obj, byref(busy))
 
     def acquireData(self, exposure=0.001):
         microseconds = int(exposure * 1e6)  # seconds to microseconds
         self.enableTimer(True, microseconds)
 
@@ -310,15 +307,15 @@
 
 def initialize(config, name='pytimepix'):
     from pathlib import Path
 
     base = Path(config).parent
 
     # read config.txt
-    with open(config, 'r') as f:
+    with open(config) as f:
         for line in f:
             inp = line.split()
             if inp[0] == 'HWID':
                 hwId = int(inp[1])
             if inp[0] == 'HWDACS':
                 hwDacs = base / inp[1]
             if inp[0] == 'PIXELDACS':
```

### Comparing `instamatic-1.8.0/instamatic/camera/fakevideostream.py` & `instamatic-1.9.0/instamatic/camera/fakevideostream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import threading
 
 import numpy as np
 
-from .camera import Camera
 from instamatic.image_utils import autoscale
 
+from .camera import Camera
+
 
 class VideoStream(threading.Thread):
     """This class mimicks the VideoStream interface (API compatible), but
     allows for displaying the image in the GUI by faking a 'continuous'
     signal."""
 
     def __init__(self, cam='simulate'):
```

### Comparing `instamatic-1.8.0/instamatic/camera/gatansocket3.md` & `instamatic-1.9.0/instamatic/camera/gatansocket3.md`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/camera/mpxhwrelaxd.dll` & `instamatic-1.9.0/instamatic/camera/mpxhwrelaxd.dll`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/camera/tpx/171207_with_flatfield.bpc` & `instamatic-1.9.0/instamatic/camera/tpx/171207_with_flatfield.bpc`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/camera/tpx/171207_with_flatfield.bpc.dacs` & `instamatic-1.9.0/instamatic/camera/tpx/171207_with_flatfield.bpc.dacs`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/camera/videostream.py` & `instamatic-1.9.0/instamatic/camera/videostream.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,202 +1,205 @@
-import atexit
-import threading
-
-from .camera import Camera
-
-
-class ImageGrabber:
-    """Continuously read out the camera for continuous acquisition.
-
-    When the continousCollectionEvent is set, the camera will set the exposure to `frametime`, otherwise, the default camera exposure is used.
-
-    The callback function is used to send the frame back to the parent routine.
-    """
-
-    def __init__(self, cam, callback, frametime: float = 0.05):
-        super().__init__()
-
-        self.callback = callback
-        self.cam = cam
-
-        self.default_exposure = self.cam.default_exposure
-        self.default_binsize = self.cam.default_binsize
-        self.dimensions = self.cam.dimensions
-        self.name = self.cam.name
-
-        self.frame = None
-        self.thread = None
-        self.stopEvent = None
-
-        self.stash = None
-
-        self.frametime = frametime
-        self.exposure = self.frametime
-        self.binsize = self.cam.default_binsize
-
-        self.lock = threading.Lock()
-
-        self.stopEvent = threading.Event()
-        self.acquireInitiateEvent = threading.Event()
-        self.acquireCompleteEvent = threading.Event()
-        self.continuousCollectionEvent = threading.Event()
-
-    def run(self):
-        while not self.stopEvent.is_set():
-
-            if self.acquireInitiateEvent.is_set():
-                self.acquireInitiateEvent.clear()
-
-                frame = self.cam.getImage(exposure=self.exposure, binsize=self.binsize)
-                self.callback(frame, acquire=True)
-
-            elif not self.continuousCollectionEvent.is_set():
-                frame = self.cam.getImage(exposure=self.frametime, binsize=self.binsize)
-                self.callback(frame)
-
-    def start_loop(self):
-        self.thread = threading.Thread(target=self.run, args=(), daemon=True)
-        self.thread.start()
-
-    def stop(self):
-        self.stopEvent.set()
-        self.thread.join()
-
-
-class VideoStream(threading.Thread):
-    """Handle the continuous stream of incoming data from the ImageGrabber."""
-
-    def __init__(self, cam='simulate'):
-        threading.Thread.__init__(self)
-
-        if isinstance(cam, str):
-            self.cam = Camera(name=cam)
-        else:
-            self.cam = cam
-
-        self.lock = threading.Lock()
-
-        self.default_exposure = self.cam.default_exposure
-        self.default_binsize = self.cam.default_binsize
-        self.dimensions = self.cam.dimensions
-        self.name = self.cam.name
-
-        self.frametime = self.default_exposure
-        self.frame = None
-
-        self.grabber = self.setup_grabber()
-
-        self.streamable = self.cam.streamable
-
-        self.start()
-
-    def __getattr__(self, attrname):
-        """Pass attribute lookups to self.cam to prevent AttributeError."""
-        try:
-            return object.__getattribute__(self, attrname)
-        except AttributeError as e:
-            reraise_on_fail = e
-            try:
-                return getattr(self.cam, attrname)
-            except AttributeError:
-                raise reraise_on_fail
-
-    def start(self):
-        self.grabber.start_loop()
-
-    def send_frame(self, frame, acquire=False):
-        if acquire:
-            self.grabber.lock.acquire(True)
-            self.acquired_frame = self.frame = frame
-            self.grabber.lock.release()
-            self.grabber.acquireCompleteEvent.set()
-        else:
-            self.grabber.lock.acquire(True)
-            self.frame = frame
-            self.grabber.lock.release()
-
-    def setup_grabber(self):
-        grabber = ImageGrabber(self.cam, callback=self.send_frame, frametime=self.frametime)
-        atexit.register(grabber.stop)
-        return grabber
-
-    def getImage(self, exposure=None, binsize=None):
-        current_frametime = self.grabber.frametime
-
-        # set to 0 to prevent it lagging data acquisition
-        self.grabber.frametime = 0
-        if exposure:
-            self.grabber.exposure = exposure
-        if binsize:
-            self.grabber.binsize = binsize
-
-        self.grabber.acquireInitiateEvent.set()
-
-        self.grabber.acquireCompleteEvent.wait()
-
-        self.grabber.lock.acquire(True)
-        frame = self.acquired_frame
-        self.grabber.lock.release()
-
-        self.grabber.acquireCompleteEvent.clear()
-        self.grabber.frametime = current_frametime
-        return frame
-
-    def update_frametime(self, frametime):
-        self.frametime = frametime
-        self.grabber.frametime = frametime
-
-    def close(self):
-        self.grabber.stop()
-
-    def block(self):
-        self.grabber.continuousCollectionEvent.set()
-
-    def unblock(self):
-        self.grabber.continuousCollectionEvent.clear()
-
-    def continuous_collection(self, exposure=0.1, n=100, callback=None):
-        """Function to continuously collect data Blocks the videostream while
-        collecting data, and only shows collected images.
-
-        exposure: float
-            exposure time
-        n: int
-            number of frames to collect
-            if defined, returns a list of collected frames
-        callback: function
-            This function is called on every iteration with the image as first argument
-            Should return True or False if data collection is to continue
-        """
-        buffer = []
-
-        go_on = True
-        i = 0
-
-        self.block()
-        while go_on:
-            i += 1
-
-            img = self.getImage(exposure=exposure)
-
-            if callback:
-                go_on = callback(img)
-            else:
-                buffer.append(img)
-                go_on = i < n
-
-        self.unblock()
-
-        if not callback:
-            return buffer
-
-    def show_stream(self):
-        from instamatic.gui import videostream_frame
-        t = threading.Thread(target=videostream_frame.start_gui, args=(self, ), daemon=True)
-        t.start()
-
-
-if __name__ == '__main__':
-    stream = VideoStream(cam='timepix')
-    from IPython import embed
-    embed()
-    stream.stop()
+import atexit
+import threading
+
+from .camera import Camera
+
+
+class ImageGrabber:
+    """Continuously read out the camera for continuous acquisition.
+
+    When the continousCollectionEvent is set, the camera will set the
+    exposure to `frametime`, otherwise, the default camera exposure is
+    used.
+
+    The callback function is used to send the frame back to the parent
+    routine.
+    """
+
+    def __init__(self, cam, callback, frametime: float = 0.05):
+        super().__init__()
+
+        self.callback = callback
+        self.cam = cam
+
+        self.default_exposure = self.cam.default_exposure
+        self.default_binsize = self.cam.default_binsize
+        self.dimensions = self.cam.dimensions
+        self.name = self.cam.name
+
+        self.frame = None
+        self.thread = None
+        self.stopEvent = None
+
+        self.stash = None
+
+        self.frametime = frametime
+        self.exposure = self.frametime
+        self.binsize = self.cam.default_binsize
+
+        self.lock = threading.Lock()
+
+        self.stopEvent = threading.Event()
+        self.acquireInitiateEvent = threading.Event()
+        self.acquireCompleteEvent = threading.Event()
+        self.continuousCollectionEvent = threading.Event()
+
+    def run(self):
+        while not self.stopEvent.is_set():
+
+            if self.acquireInitiateEvent.is_set():
+                self.acquireInitiateEvent.clear()
+
+                frame = self.cam.getImage(exposure=self.exposure, binsize=self.binsize)
+                self.callback(frame, acquire=True)
+
+            elif not self.continuousCollectionEvent.is_set():
+                frame = self.cam.getImage(exposure=self.frametime, binsize=self.binsize)
+                self.callback(frame)
+
+    def start_loop(self):
+        self.thread = threading.Thread(target=self.run, args=(), daemon=True)
+        self.thread.start()
+
+    def stop(self):
+        self.stopEvent.set()
+        self.thread.join()
+
+
+class VideoStream(threading.Thread):
+    """Handle the continuous stream of incoming data from the ImageGrabber."""
+
+    def __init__(self, cam='simulate'):
+        threading.Thread.__init__(self)
+
+        if isinstance(cam, str):
+            self.cam = Camera(name=cam)
+        else:
+            self.cam = cam
+
+        self.lock = threading.Lock()
+
+        self.default_exposure = self.cam.default_exposure
+        self.default_binsize = self.cam.default_binsize
+        self.dimensions = self.cam.dimensions
+        self.name = self.cam.name
+
+        self.frametime = self.default_exposure
+        self.frame = None
+
+        self.grabber = self.setup_grabber()
+
+        self.streamable = self.cam.streamable
+
+        self.start()
+
+    def __getattr__(self, attrname):
+        """Pass attribute lookups to self.cam to prevent AttributeError."""
+        try:
+            return object.__getattribute__(self, attrname)
+        except AttributeError as e:
+            reraise_on_fail = e
+            try:
+                return getattr(self.cam, attrname)
+            except AttributeError:
+                raise reraise_on_fail
+
+    def start(self):
+        self.grabber.start_loop()
+
+    def send_frame(self, frame, acquire=False):
+        if acquire:
+            self.grabber.lock.acquire(True)
+            self.acquired_frame = self.frame = frame
+            self.grabber.lock.release()
+            self.grabber.acquireCompleteEvent.set()
+        else:
+            self.grabber.lock.acquire(True)
+            self.frame = frame
+            self.grabber.lock.release()
+
+    def setup_grabber(self):
+        grabber = ImageGrabber(self.cam, callback=self.send_frame, frametime=self.frametime)
+        atexit.register(grabber.stop)
+        return grabber
+
+    def getImage(self, exposure=None, binsize=None):
+        current_frametime = self.grabber.frametime
+
+        # set to 0 to prevent it lagging data acquisition
+        self.grabber.frametime = 0
+        if exposure:
+            self.grabber.exposure = exposure
+        if binsize:
+            self.grabber.binsize = binsize
+
+        self.grabber.acquireInitiateEvent.set()
+
+        self.grabber.acquireCompleteEvent.wait()
+
+        self.grabber.lock.acquire(True)
+        frame = self.acquired_frame
+        self.grabber.lock.release()
+
+        self.grabber.acquireCompleteEvent.clear()
+        self.grabber.frametime = current_frametime
+        return frame
+
+    def update_frametime(self, frametime):
+        self.frametime = frametime
+        self.grabber.frametime = frametime
+
+    def close(self):
+        self.grabber.stop()
+
+    def block(self):
+        self.grabber.continuousCollectionEvent.set()
+
+    def unblock(self):
+        self.grabber.continuousCollectionEvent.clear()
+
+    def continuous_collection(self, exposure=0.1, n=100, callback=None):
+        """Function to continuously collect data Blocks the videostream while
+        collecting data, and only shows collected images.
+
+        exposure: float
+            exposure time
+        n: int
+            number of frames to collect
+            if defined, returns a list of collected frames
+        callback: function
+            This function is called on every iteration with the image as first argument
+            Should return True or False if data collection is to continue
+        """
+        buffer = []
+
+        go_on = True
+        i = 0
+
+        self.block()
+        while go_on:
+            i += 1
+
+            img = self.getImage(exposure=exposure)
+
+            if callback:
+                go_on = callback(img)
+            else:
+                buffer.append(img)
+                go_on = i < n
+
+        self.unblock()
+
+        if not callback:
+            return buffer
+
+    def show_stream(self):
+        from instamatic.gui import videostream_frame
+        t = threading.Thread(target=videostream_frame.start_gui, args=(self, ), daemon=True)
+        t.start()
+
+
+if __name__ == '__main__':
+    stream = VideoStream(cam='timepix')
+    from IPython import embed
+    embed()
+    stream.stop()
```

### Comparing `instamatic-1.8.0/instamatic/config/__init__.py` & `instamatic-1.9.0/instamatic/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 import shutil
 import sys
 from collections.abc import Mapping
 from pathlib import Path
 
 import yaml
 
-from .config_updater import check_defaults_yaml
-from .config_updater import check_settings_yaml
-from .config_updater import convert_config
-from .config_updater import is_oldstyle
+from .config_updater import (
+    check_defaults_yaml,
+    check_settings_yaml,
+    convert_config,
+    is_oldstyle,
+)
+
 logger = logging.getLogger(__name__)
 
 
 _settings_yaml = 'settings.yaml'
 _defaults_yaml = 'defaults.yaml'
 _logs = 'logs'
 _config = 'config'
@@ -109,19 +112,19 @@
     def __getitem__(self, item):
         return self.mapping[item]
 
     @classmethod
     def from_file(cls, path: str):
         """Read configuration from yaml file, returns namespace."""
         name = Path(path).stem
-        return cls(yaml.load(open(path, 'r'), Loader=yaml.Loader), name=name, location=path)
+        return cls(yaml.load(open(path), Loader=yaml.Loader), name=name, location=path)
 
     def update_from_file(self, path: str) -> None:
         """Update configuration from yaml file."""
-        self.update(yaml.load(open(path, 'r'), Loader=yaml.Loader))
+        self.update(yaml.load(open(path), Loader=yaml.Loader))
         self.location = path
 
     def update(self, mapping: dict):
         for key, value in mapping.items():
             if isinstance(value, dict):
                 try:
                     nested_update(getattr(self, key), value)
@@ -201,25 +204,25 @@
 
 
 def load_defaults():
     global defaults
 
     check_defaults_yaml(config_drc, _defaults_yaml)
 
-    defaults = ConfigObject.from_file(Path(__file__).parent / _defaults_yaml)  # load defaults
-    defaults.update_from_file(config_drc / _defaults_yaml)             # update user parameters
+    defaults = ConfigObject.from_file(Path(__file__).parent / _defaults_yaml)
+    defaults.update_from_file(config_drc / _defaults_yaml)
 
 
 def load_settings():
     global settings
 
     check_settings_yaml(config_drc / 'global.yaml', config_drc / _settings_yaml)
 
-    settings = ConfigObject.from_file(Path(__file__).parent / _settings_yaml)  # load defaults
-    settings.update_from_file(config_drc / _settings_yaml)             # update user parameters
+    settings = ConfigObject.from_file(Path(__file__).parent / _settings_yaml)
+    settings.update_from_file(config_drc / _settings_yaml)
 
     settings.data_directory = Path(settings.data_directory)
 
     today = datetime.datetime.now().strftime('%Y-%m-%d')
     settings.work_directory = settings.data_directory / f'{today}'
 
 
@@ -265,17 +268,17 @@
 
 locations = {
     'base': base_drc,
     'config': config_drc,
     'logs': logs_drc,
     'scripts': scripts_drc,
     'camera': alignments_drc,
-    'microscope': calibration.location,
-    'calibration': microscope.location,
-    'alignments': camera.location,
+    'microscope': calibration.location.parent,
+    'calibration': microscope.location.parent,
+    'alignments': camera.location.parent,
     'data': settings.data_directory,
     'work': settings.work_directory,
     'microscope_config': calibration.location,
     'calibration_config': microscope.location,
     'alignments_config': camera.location,
     'settings': config_drc / _settings_yaml,
     'defaults': config_drc / _defaults_yaml,
```

### Comparing `instamatic-1.8.0/instamatic/config/autoconfig.py` & `instamatic-1.9.0/instamatic/config/autoconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from instamatic import config
 from instamatic.config.utils import yaml
 from instamatic.tools import relativistic_wavelength
 
 
 def get_tvips_calibs(ctrl, rng: list, mode: str, wavelength: float) -> dict:
     """Loop over magnification ranges and return calibrations from EMMENU."""
-
     if mode == 'diff':
         print('Warning: Pixelsize can be a factor 10 off in diff mode (bug in EMMENU)')
 
     calib_range = {}
 
     binning = ctrl.cam.getBinning()
 
@@ -49,15 +48,15 @@
     print()
 
     try:
         default_choice = choices.index(default)
         suffix = f' [{default}]'
     except ValueError:
         default_choice = 0
-        suffix = f''
+        suffix = ''
 
     for i, choice in enumerate(choices):
         print(f'{i+1: 2d}: {choice}')
 
     q = input(f'\n{question}{suffix} >> ')
     if not q:
         q = default_choice
@@ -106,16 +105,16 @@
 
     cam_config = choice_prompt(choices=choices,
                                default=None,
                                question='Which camera type do you want to use (select closest one and modify if needed)?')
 
     # Instantiate microscope / camera connection
 
-    from instamatic.TEMController.microscope import get_tem
     from instamatic.camera.camera import get_cam
+    from instamatic.TEMController.microscope import get_tem
     from instamatic.TEMController.TEMController import TEMController
 
     cam = get_cam(cam_name)() if cam_name else None
     tem = get_tem(tem_name)()
 
     ctrl = TEMController(tem=tem, cam=cam)
 
@@ -167,15 +166,15 @@
 
     microscope_drc = config.locations['microscope']
     camera_drc = config.locations['camera']
     calibration_drc = config.locations['calibration']
     settings_yaml = config.locations['settings']
 
     print()
-    print(f'Wrote files config files:')
+    print('Wrote files config files:')
     print(f'    Copy {tem_config_fn} -> `{microscope_drc / tem_config_fn}`')
     print(f'    Copy {calib_config_fn} -> `{calibration_drc / calib_config_fn}`')
     if cam_config:
         print(f'    Copy {cam_config_fn} -> `{camera_drc / cam_config_fn}`')
     print()
     print(f'In `{settings_yaml}`:')
     print(f'    microscope: {tem_name}_tem')
```

### Comparing `instamatic-1.8.0/instamatic/config/calibration/orius.yaml` & `instamatic-1.9.0/instamatic/config/calibration/orius.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/config/calibration/simulate.yaml` & `instamatic-1.9.0/instamatic/config/calibration/simulate.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/config/calibration/timepix.yaml` & `instamatic-1.9.0/instamatic/config/calibration/timepix.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/config/calibration/tvips-f416.yaml` & `instamatic-1.9.0/instamatic/config/calibration/tvips-f416.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/config/camera/serval.yaml` & `instamatic-1.9.0/instamatic/config/camera/serval.yaml`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-camera_rotation_vs_stage_xy: 0.0
-default_binsize: 1
-default_exposure: 0.02
-dimensions: [512, 512]
-dynamic_range: 11800
-interface: serval
-physical_pixelsize: 0.055
-possible_binsizes: [1]
-stretch_amplitude: 0.0
-stretch_azimuth: 0.0
-detector_config:
-  BiasVoltage: 100
-  BiasEnabled: True
-  TriggerMode: SOFTWARESTART_TIMERSTOP
-  ExposureTime: 1.0
-  TriggerPeriod: 1.001
-  nTriggers: 1000000000
-  GainMode: HGM
-bpc_file_path: '/home/asi/Desktop/Factory_settings/SPM-HGM/config.bpc'
-dacs_file_path: '/home/asi/Desktop/Factory_settings/SPM-HGM/config.dacs'
-url: 'http://localhost:8080'
+camera_rotation_vs_stage_xy: 0.0
+default_binsize: 1
+default_exposure: 0.02
+dimensions: [512, 512]
+dynamic_range: 11800
+interface: serval
+physical_pixelsize: 0.055
+possible_binsizes: [1]
+stretch_amplitude: 0.0
+stretch_azimuth: 0.0
+detector_config:
+  BiasVoltage: 100
+  BiasEnabled: True
+  TriggerMode: SOFTWARESTART_TIMERSTOP
+  ExposureTime: 1.0
+  TriggerPeriod: 1.001
+  nTriggers: 1000000000
+  GainMode: HGM
+bpc_file_path: '/home/asi/Desktop/Factory_settings/SPM-HGM/config.bpc'
+dacs_file_path: '/home/asi/Desktop/Factory_settings/SPM-HGM/config.dacs'
+url: 'http://localhost:8080'
```

### Comparing `instamatic-1.8.0/instamatic/config/config_updater.py` & `instamatic-1.9.0/instamatic/config/config_updater.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/config/microscope/fei_simu.yaml` & `instamatic-1.9.0/instamatic/config/microscope/fei_simu.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/config/microscope/fei_themisZ.yaml` & `instamatic-1.9.0/instamatic/config/microscope/fei_themisZ.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/config/microscope/jeol-1400.yaml` & `instamatic-1.9.0/instamatic/config/microscope/jeol-1400.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/config/microscope/jeol.yaml` & `instamatic-1.9.0/instamatic/config/microscope/jeol.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/config/microscope/simulate.yaml` & `instamatic-1.9.0/instamatic/config/microscope/simulate.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/config/scripts/readme.md` & `instamatic-1.9.0/instamatic/config/scripts/readme.md`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/config/settings.yaml` & `instamatic-1.9.0/instamatic/config/settings.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/config/utils.py` & `instamatic-1.9.0/instamatic/config/utils.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/exceptions.py` & `instamatic-1.9.0/instamatic/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,50 @@
-class TEMCommunicationError(ConnectionError):
-    pass
-
-
-class TEMValueError(ValueError):
-    pass
-
-
-class JEOLValueError(TEMValueError):
-    pass
-
-
-class FEIValueError(TEMValueError):
-    pass
-
-
-class TEMControllerError(Exception):
-    pass
-
-
-exception_list = {
-    'TEMValueError': TEMValueError,
-    'TEMCommunicationError': TEMCommunicationError,
-    'TEMValueError': TEMValueError,
-    'JEOLValueError': JEOLValueError,
-    'FEIValueError': FEIValueError,
-    'TEMControllerError   ': TEMControllerError,
-    'AttributeError': AttributeError,
-    'AssertionError': AssertionError,
-    'ConnectionError': ConnectionError,
-    'Exception': Exception,
-    'FileNotFoundError': FileNotFoundError,
-    'IndexError': IndexError,
-    'InterruptedError': InterruptedError,
-    'IOError': IOError,
-    'KeyError': KeyError,
-    'NameError': NameError,
-    'NotImplementedError': NotImplementedError,
-    'OSError': OSError,
-    'PermissionError': PermissionError,
-    'RuntimeError': RuntimeError,
-    'StopIteration': StopIteration,
-    'TypeError': TypeError,
-    'ValueError': ValueError,
-}
-
-try:
-    # avoid crash on linux instances
-    exception_list['WindowsError'] = WindowsError
-except NameError:
-    pass
+class TEMCommunicationError(ConnectionError):
+    pass
+
+
+class TEMValueError(ValueError):
+    pass
+
+
+class JEOLValueError(TEMValueError):
+    pass
+
+
+class FEIValueError(TEMValueError):
+    pass
+
+
+class TEMControllerError(Exception):
+    pass
+
+
+exception_list = {
+    'TEMValueError': TEMValueError,
+    'TEMCommunicationError': TEMCommunicationError,
+    'JEOLValueError': JEOLValueError,
+    'FEIValueError': FEIValueError,
+    'TEMControllerError   ': TEMControllerError,
+    'AttributeError': AttributeError,
+    'AssertionError': AssertionError,
+    'ConnectionError': ConnectionError,
+    'Exception': Exception,
+    'FileNotFoundError': FileNotFoundError,
+    'IndexError': IndexError,
+    'InterruptedError': InterruptedError,
+    'IOError': IOError,
+    'KeyError': KeyError,
+    'NameError': NameError,
+    'NotImplementedError': NotImplementedError,
+    'OSError': OSError,
+    'PermissionError': PermissionError,
+    'RuntimeError': RuntimeError,
+    'StopIteration': StopIteration,
+    'TypeError': TypeError,
+    'ValueError': ValueError,
+}
+
+try:
+    # avoid crash on linux instances
+    exception_list['WindowsError'] = WindowsError
+except NameError:
+    pass
```

### Comparing `instamatic-1.8.0/instamatic/experiments/autocred/experiment.py` & `instamatic-1.9.0/instamatic/experiments/autocred/experiment.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,1396 +1,1394 @@
-import datetime
-import json
-import os
-import pickle
-import shutil
-import socket
-import time
-import traceback
-from pathlib import Path
-
-import numpy as np
-from scipy import ndimage
-from skimage.registration import phase_cross_correlation
-from tqdm.auto import tqdm
-
-from instamatic import config
-from instamatic.calibrate import CalibBeamShift
-from instamatic.calibrate import CalibDirectBeam
-from instamatic.calibrate.calibrate_beamshift import calibrate_beamshift
-from instamatic.calibrate.calibrate_imageshift12 import Calibrate_Beamshift_D
-from instamatic.calibrate.calibrate_imageshift12 import Calibrate_Beamshift_D_Defoc
-from instamatic.calibrate.calibrate_imageshift12 import Calibrate_Imageshift
-from instamatic.calibrate.calibrate_imageshift12 import Calibrate_Imageshift2
-from instamatic.calibrate.calibrate_imageshift12 import Calibrate_Stage
-from instamatic.calibrate.center_z import center_z_height_HYMethod
-from instamatic.calibrate.filenames import *
-from instamatic.formats import write_tiff
-from instamatic.neural_network import predict
-from instamatic.neural_network import preprocess
-from instamatic.processing.find_crystals import find_crystals_timepix
-from instamatic.processing.ImgConversionTPX import ImgConversionTPX as ImgConversion
-from instamatic.tools import find_beam_center
-from instamatic.tools import find_defocused_image_center
-
-# SerialRED:
-#  Currently only working if live view can be read directly from camera via Python API
-#  Extensively tested on a JEOL 2100 LaB6 TEM with a Timepix camera.
-#  Imgvar can be compared with the first defocused image.
-#  If other particles move in, the variance will be at least 50% different
-
-# spread, offset: parameters for find_crystals_timepix
-# spread = 2  # sometimes crystals still are not so isolated using number 0.6 as suggested.
-# offset = 15  # The number needs to be smaller when the contrast of the crystals is low.
-# imgvar_threshold = 600
-
-date = datetime.datetime.now().strftime('%Y-%m-%d')
-log_rotaterange = config.locations['logs'] / f'Rotrange_stagepos_{date}.log'
-log_iscalibs = config.locations['logs'] / f'ImageShift_LOGS_{date}'
-log_iscalibs.mkdir(exist_ok=True)
-
-if not os.path.isfile(log_rotaterange):
-    with open(log_rotaterange, 'a') as f:
-        f.write('x\ty\tz\trotation range\n')
-
-use_dials = config.settings.use_indexing_server_exe
-use_vm = config.settings.use_VM_server_exe
-
-
-def load_IS_Calibrations(imageshift, ctrl, diff_defocus, logger, mode):
-    if mode == 'diff' or mode == 'mag1':
-        if imageshift == 'IS1' and diff_defocus != 0:
-            file = CALIB_IS1_DEFOC
-        elif imageshift == 'IS2' and diff_defocus != 0:
-            file = CALIB_IS2_DEFOC
-        elif imageshift == 'IS1' and diff_defocus == 0:
-            file = CALIB_IS1_FOC
-        elif imageshift == 'IS2' and diff_defocus == 0:
-            file = CALIB_IS2_FOC
-        elif imageshift == 'BS' and diff_defocus == 0:
-            file = CALIB_BEAMSHIFT_DP
-        elif imageshift == 'BS' and diff_defocus != 0:
-            file = CALIB_BEAMSHIFT_DP_DEFOC
-        elif imageshift == 'S':
-            file = CALIB_STAGE
-    else:
-        print('Wrong input. Mode can either be mag1 or diff for calibration!')
-        return 0
-
-    try:
-        if imageshift == 'S':
-            with open(config.locations['logs'] / file, 'rb') as f:
-                transform_imgshift, c = pickle.load(f)
-        else:
-            with open(log_iscalibs / file, 'rb') as f:
-                transform_imgshift, c = pickle.load(f)
-    except BaseException:
-        print(f'No {imageshift}, defocus = {diff_defocus} calibration found. Choose the desired defocus value.')
-        inp = input('Press ENTER when ready.')
-        if ctrl.mode != mode:
-            ctrl.mode.set(mode)
-        satisfied = 'x'
-        while satisfied == 'x':
-            if imageshift == 'IS1' and diff_defocus != 0:
-                mag_calib = ctrl.magnification.value
-                s_calib = int(200.0 / mag_calib * 1500)
-                transform_imgshift, c = Calibrate_Imageshift(ctrl, diff_defocus, stepsize=s_calib, logger=logger, key='IS1')
-            elif imageshift == 'IS1' and diff_defocus == 0:
-                mag_calib = ctrl.magnification.value
-                s_calib = int(200.0 / mag_calib * 1000)
-                transform_imgshift, c = Calibrate_Imageshift(ctrl, diff_defocus, stepsize=s_calib, logger=logger, key='IS1')
-            elif imageshift == 'IS2':
-                mag_calib = ctrl.magnification.value
-                s_calib = int(200.0 / mag_calib * 750)
-                transform_imgshift, c = Calibrate_Imageshift2(ctrl, diff_defocus, stepsize=s_calib, logger=logger)
-            elif imageshift == 'BS' and diff_defocus == 0:
-                mag_calib = ctrl.magnification.value
-                s_calib = int(250.0 / mag_calib * 100)
-                transform_imgshift, c = Calibrate_Beamshift_D(ctrl, stepsize=s_calib, logger=logger)
-            elif imageshift == 'BS' and diff_defocus != 0:
-                mag_calib = ctrl.magnification.value
-                s_calib = int(250.0 / mag_calib * 100)
-                transform_imgshift, c = Calibrate_Beamshift_D_Defoc(ctrl, diff_defocus, stepsize=s_calib, logger=logger)
-
-            elif imageshift == 'S':
-                mag_calib = ctrl.magnification.value
-                s_calib = int(2500.0 / mag_calib * 1000)
-                transform_imgshift, c = Calibrate_Stage(ctrl, stepsize=s_calib, logger=logger)
-            with open(log_iscalibs / file, 'wb') as f:
-                pickle.dump([transform_imgshift, c], f)
-            satisfied = input(f'{imageshift}, defocus = {diff_defocus} calibration done. \nPress Enter to continue. Press x to redo calibration.')
-
-    return transform_imgshift, c
-
-
-class Experiment:
-    def __init__(self, ctrl,
-                 exposure_time,
-                 exposure_time_image,
-                 stop_event,
-                 stop_event_experiment,
-                 enable_image_interval,
-                 enable_autotrack,
-                 enable_fullacred,
-                 enable_fullacred_crystalfinder,
-                 scan_area,
-                 zheight,
-                 autocenterDP,
-                 angle_activation,
-                 spread,
-                 offset,
-                 rotrange,
-                 backlash_killer,
-                 rotation_speed,
-                 unblank_beam=False,
-                 path=None,
-                 log=None,
-                 flatfield=None,
-                 image_interval=99999,
-                 diff_defocus=0):
-        super().__init__()
-        self.ctrl = ctrl
-        self.path = path
-        self.expt = exposure_time
-        self.unblank_beam = unblank_beam
-        self.logger = log
-        self.camtype = ctrl.cam.name
-        self.stopEvent = stop_event
-        self.stopEvent_rasterScan = stop_event_experiment
-        self.flatfield = flatfield
-        self.stagepos_idx = 0
-
-        self.diff_defocus = diff_defocus
-        self.image_interval = image_interval
-        self.nom_ii = self.image_interval
-        self.robust_ii = 2
-        self.exposure_time_image = exposure_time_image
-
-        self.scan_area = scan_area
-        self.auto_zheight = zheight
-        self.mode = 0
-
-        self.diff_brightness = self.ctrl.brightness.value
-        # self.autocenterDP = autocenterDP
-        self.angle_activation = angle_activation
-        self.spread = spread
-        self.offset = offset
-        self.rotrangelimit = rotrange
-        self.backlash_killer = backlash_killer
-        self.rotation_speed = rotation_speed
-
-        self.calibdir = self.path.parent / 'calib'
-
-        self.verbose = False
-        self.number_crystals_scanned = 0
-        self.number_exp_performed = 0
-
-        if not os.path.exists(self.calibdir):
-            os.makedirs(self.calibdir)
-
-        self.image_interval_enabled = enable_image_interval
-        if enable_image_interval:
-            self.image_interval = image_interval
-            msg = f'Image interval enabled: every {self.image_interval} frames an image with defocus {self.diff_defocus} will be displayed (t={self.exposure_time_image} s).'
-            if self.verbose:
-                print(msg)
-            self.logger.info(msg)
-        else:
-            self.image_interval = 99999
-
-        self.enable_autotrack = enable_autotrack
-        self.enable_fullacred = enable_fullacred
-        self.enable_fullacred_crystalfinder = enable_fullacred_crystalfinder
-
-        if enable_fullacred_crystalfinder:
-            self.diff_defocus = diff_defocus
-            self.image_interval = image_interval
-            msg = f'Full autocRED feature with auto crystal finder enabled: every {image_interval} frames an image with defocus value {diff_defocus} will be displayed.'
-            self.mode = 3
-
-        elif enable_fullacred:
-            self.diff_defocus = diff_defocus
-            self.image_interval = image_interval
-            msg = f'Full autocRED feature enabled: every {image_interval} frames an image with defocus value {diff_defocus} will be displayed.'
-            self.mode = 2
-
-        elif enable_autotrack:
-            self.diff_defocus = diff_defocus
-            self.image_interval = image_interval
-            msg = f'Image autotrack enabled: every {image_interval} frames an image with defocus value {diff_defocus} will be displayed.'
-            self.mode = 1
-
-        if self.verbose:
-            print(msg)
-
-        if use_dials:
-            self.s = socket.socket()
-            dials_host = config.settings.indexing_server_host
-            dials_port = config.settings.indexing_server_port
-            try:
-                self.s.connect((dials_host, dials_port))
-                print('DIALS server connected for autocRED.')
-                self.s_c = 1
-            except BaseException:
-                print('Is DIALS server running? Connection failed.')
-                self.s_c = 0
-
-        if use_vm:
-            self.s2 = socket.socket()
-            vm_host = config.settings.VM_server_host
-            vm_port = config.settings.VM_server_port
-            try:
-                self.s2.connect((vm_host, vm_port))
-                print('VirtualBox server connected for autocRED.')
-                self.s2_c = 1
-            except BaseException:
-                print('Is VM server running? Connection failed.')
-                self.s2_c = 0
-
-    def image_cropper(self, img, window_size=0):
-        crystal_pos, r = find_defocused_image_center(img)  # find_defocused_image_center crystal position (y,x)
-        crystal_pos = crystal_pos[::-1]
-
-        if window_size == 0:
-
-            if r[0] <= r[1]:
-                window_size = r[0] * 2
-            else:
-                window_size = r[1] * 2
-
-            window_size = int(window_size / 1.414)
-            if window_size % 2 == 1:
-                window_size = window_size + 1
-
-        a1 = int(crystal_pos[0] - window_size / 2)
-        b1 = int(crystal_pos[0] + window_size / 2)
-        a2 = int(crystal_pos[1] - window_size / 2)
-        b2 = int(crystal_pos[1] + window_size / 2)
-
-        img_cropped = img[a1:b1, a2:b2]
-        return crystal_pos, img_cropped, window_size
-
-    def hysteresis_check(self, n_cycle=4):
-        print('Relaxing beam...')
-        modes = ['mag1', 'samag', 'diff']
-        current_mode = self.ctrl.mode.get()
-        mode_index = modes.index(current_mode)
-
-        for i in range(n_cycle):
-            self.ctrl.mode.set(modes[(mode_index + 1) % 3])
-            time.sleep(0.5)
-            self.ctrl.mode.set(modes[(mode_index + 2) % 3])
-            time.sleep(0.5)
-            self.ctrl.mode.set(modes[mode_index])
-            time.sleep(0.5)
-
-        print('Beam relaxing done.')
-
-    def check_lens_close_to_limit_warning(self, lensname, lensvalue, MAX=65535, threshold=5000):
-        warn = 0
-        if MAX - lensvalue < threshold or lensvalue < threshold:
-            warn = 1
-            if self.verbose:
-                print(f'Warning: {lensname} close to limit!')
-        return warn
-
-    def img_var(self, img, apert_pos):
-        apert_pos = [int(apert_pos[0]), int(apert_pos[1])]
-        window_size = img.shape[0]
-        half_w = int(window_size / 2)
-        x_range = range(apert_pos[0] - half_w, apert_pos[0] + half_w)
-        y_range = range(apert_pos[1] - half_w, apert_pos[1] + half_w)
-
-        if not any(x in range(255, 261) for x in x_range) and not any(y in range(255, 261) for y in y_range):
-            return np.var(img)
-        else:
-            if any(x in range(255, 261) for x in x_range):
-                indx = []
-                for px in range(255, 261):
-                    try:
-                        indx.append(x_range.index(px))
-                    except BaseException:
-                        pass
-
-                img = np.delete(img, indx, 0)
-
-            if any(y in range(255, 261) for y in y_range):
-                indy = []
-                for px in range(255, 261):
-                    try:
-                        indy.append(y_range.index(px))
-                    except BaseException:
-                        pass
-
-                img = np.delete(img, indy, 1)
-
-            return np.var(img)
-
-    def check_img_outsidebeam_byscale(self, img1_scale, img2_scale):
-        """img1 is the original image for reference, img2 is the new image."""
-        if img2_scale / img1_scale < 0.5 or img2_scale / img1_scale > 2:
-            return 1
-        else:
-            return 0
-
-    def eliminate_backlash_in_tiltx(self):
-        a_i = self.ctrl.stage.a
-        if a_i < 0:
-            self.ctrl.stage.set(a=a_i + self.backlash_killer, wait=True)
-            # print("Rotation positive!")
-            return 0
-        else:
-            self.ctrl.stage.set(a=a_i - self.backlash_killer, wait=True)
-            # print("Rotation negative!")
-            return 1
-
-    def center_particle_ofinterest(self, pos_arr, transform_stagepos):
-        """Used to center the particle of interest in the view to minimize
-        usage of lens."""
-        transform_stagepos_ = np.linalg.inv(transform_stagepos)
-        if pos_arr[0] < 200 or pos_arr[0] > 316 or pos_arr[1] < 200 or pos_arr[1] > 316:
-
-            _x0 = self.ctrl.stage.x
-            _y0 = self.ctrl.stage.y
-
-            displacement = np.subtract((258, 258), pos_arr)
-            mag = self.ctrl.magnification.value
-
-            s = config.calibration['mag1']['pixelsize'][mag] / 1000  # nm -> um
-            # print("scaling facor: {} um per px".format(s))
-
-            mvmt = s * displacement
-            mvmt_x, mvmt_y = np.dot(1000 * mvmt, transform_stagepos_)
-
-            self.ctrl.stage.set(x=_x0 + mvmt_y, y=_y0 - mvmt_x)
-
-        else:
-            pass
-
-    def center_particle_from_crystalList(self, crystal_positions, transform_stagepos, magnification, beamsize):
-        n_crystals = len(crystal_positions)
-        if n_crystals == 0:
-            self.print_and_del('No crystal found on image!')
-            return (0, 0)
-
-        else:
-            beam_area = beamsize ** 2
-
-            for crystal in crystal_positions:
-                if crystal.isolated:
-                    self.center_particle_ofinterest((crystal.x, crystal.y), transform_stagepos)
-                    crystalsize = crystal.area_pixel
-                    # print("crystal size: {}".format(crystalsize))
-                    img, h = self.ctrl.get_image(exposure=self.expt, header_keys=None)
-
-                    crystal_positions_new = find_crystals_timepix(img, magnification=self.magnification, spread=self.spread, offset=self.offset)
-
-                    n_crystals_new = len(crystal_positions_new)
-                    # print(crystal_positions_new)
-                    if n_crystals_new == 0:
-                        self.print_and_del('No crystal found after centering...')
-                        return (0, 0)
-
-                    else:
-                        # print("Start looping.")
-                        for crystal in crystal_positions_new:
-                            if crystal.isolated and crystalsize * 0.9 <= crystal.area_pixel <= crystalsize * 1.1:
-                                self.print_and_del(f'Crystal that has been centered is found at {crystal.x}, {crystal.y}.')
-                                beamshift_coords = self.calib_beamshift.pixelcoord_to_beamshift((crystal.x, crystal.y))
-
-                                return (beamshift_coords, crystalsize)
-                            else:
-                                return (0, 0)
-
-                else:
-                    return (0, 0)
-
-    def isolated(self, c, crystalpositions, thresh=100):
-        distances = []
-        if len(crystalpositions) == 1:
-            return True
-        else:
-            for allcryst in crystalpositions:
-                distvec = np.subtract(allcryst, (c.x, c.y))
-                dist = np.linalg.norm(distvec)
-                if dist != 0:
-                    distances.append(dist)
-
-            if min(distances) > thresh:  # in pixels
-                return True
-            else:
-                return False
-
-    def find_crystal_center(self, img_c, window_size, gauss_window=4):
-        mn = np.min(img_c)
-        mx = np.max(img_c)
-
-        sel = (img_c > l + 0.1 * (mx - mn)) & (img_c < mx - 0.4 * (h - mn))
-        blurred = ndimage.filters.gaussian_filter(sel.astype(float), gauss_window)
-        x, y = np.unravel_index(np.argmax(blurred, axis=None), blurred.shape)
-        return (y, x)
-
-    def find_crystal_center_fromhist(self, img, bins=20, plot=False, gauss_window=5):
-        h, b = np.histogram(img, bins)
-        sel = (img > b[1]) & (img < b[8])
-
-        blurred = ndimage.filters.gaussian_filter(sel.astype(float), gauss_window)
-        x, y = np.unravel_index(np.argmax(blurred, axis=None), blurred.shape)
-        if plot:
-            plt.imshow(sel)
-            plt.scatter(y, x)
-            plt.show()
-        return (y, x)
-
-    def tracking_by_particlerecog(self, img, magnification=2500, spread=6, offset=18):
-        crystal_pos, r = find_defocused_image_center(img)  # find_defocused_image_center crystal position (y,x)
-        crystal_pos = crystal_pos[::-1]
-
-        window_size = 0
-
-        if window_size == 0:
-
-            if r[0] <= r[1]:
-                window_size = r[0] * 2
-            else:
-                window_size = r[1] * 2
-
-            # window_size = int(window_size/1.414)
-            if window_size % 2 == 1:
-                window_size = window_size + 1
-
-        a1 = int(crystal_pos[0] - window_size / 2)
-        b1 = int(crystal_pos[0] + window_size / 2)
-        a2 = int(crystal_pos[1] - window_size / 2)
-        b2 = int(crystal_pos[1] + window_size / 2)
-
-        img_cropped = img[a1:b1, a2:b2]
-
-        # crystalpositions = find_crystals_timepix(img_cropped, magnification = magnification, spread=spread, offset = offset)
-        # crystalposition = self.find_crystal_center(img_cropped, window_size)
-        crystalposition = self.find_crystal_center_fromhist(img_cropped)
-        center = (window_size / 2, window_size / 2)
-
-        # if len(crystalpositions) == 1:
-        # crystalxy = (crystalpositions[0].x, crystalpositions[0].y)
-        shift = np.subtract(center, crystalposition)
-        # elif len(crystalpositions) > 1:
-        #    areas = [crystal.area_pixel for crystal in crystalpositions]
-        #    idx = areas.index(max(areas))
-        #    crystalxy = (crystalpositions[idx].x, crystalpositions[idx].y)
-        #    shift = np.subtract(center, crystalxy)
-        # else:
-        #    print("Crystal lost.")
-        #    shift = np.array((512, 512))
-
-        return tuple(shift[::-1])
-
-    def setandupdate_bs(self, bs_x0, bs_y0, delta_beamshiftcoord1):
-        self.ctrl.beamshift.set(bs_x0 + delta_beamshiftcoord1[0], bs_y0 + delta_beamshiftcoord1[1])
-        bs_x0 = bs_x0 + delta_beamshiftcoord1[0]
-        bs_y0 = bs_y0 + delta_beamshiftcoord1[1]
-        return bs_x0, bs_y0
-
-    def defocus_and_image(self, difffocus, exp_t):
-        diff_focus_proper = self.ctrl.difffocus.value
-        diff_focus_defocused = diff_focus_proper + difffocus
-        self.ctrl.difffocus.value = diff_focus_defocused
-
-        img0, h = self.ctrl.get_image(exp_t, header_keys=None)
-        self.ctrl.difffocus.value = diff_focus_proper
-        return img0, h
-
-    def print_and_log(self, logger, msg):
-        print(msg)
-        logger.debug(msg)
-
-    def print_and_del(self, msg):
-        print('\033[k', msg, end='\r')
-
-    def imagevar_blank_estimator(self, brightness, cycle=3):
-        # previous_mode = self.ctrl.mode.get()
-        self.ctrl.mode.set('mag1')
-        self.ctrl.brightness.value = brightness
-
-        input('Please move your stage to a blank area for image variance calculation. Do not change brightness. Press ENTER when ready.')
-        img_var_est = []
-        beamsize_est = []
-        for i in range(0, cycle):
-            img, h = self.ctrl.get_image(self.exposure_time_image, header_keys=None)
-            crystal_pos, img0_cropped, window_size = self.image_cropper(img=img, window_size=0)
-            v = self.img_var(img0_cropped, crystal_pos)
-            print(f'blank image variance: {v}')
-            img_var_est.append(v)
-            beamsize_est.append(window_size)
-
-        image_var = np.average(img_var_est)
-        beamsize_avg = np.average(window_size)
-
-        self.ctrl.mode.set('samag')
-        self.ctrl.mode.set('diff')
-        return image_var, beamsize_avg
-
-    def auto_cred_collection(self, path, pathtiff, pathsmv, pathred, transform_imgshift, transform_imgshift2, transform_imgshift_foc, transform_imgshift2_foc, transform_beamshift_d, transform_beamshift_d_defoc, calib_beamshift):
-        """track method
-        p: particle recognition
-        c: cross correlation"""
-
-        trackmethod = 'p'
-
-        for paths in (path, pathtiff, pathsmv, pathred):
-            if not os.path.exists(paths):
-                os.makedirs(paths)
-
-        a = a0 = self.ctrl.stage.a
-        spotsize = self.ctrl.spotsize
-
-        if self.mode == 1:
-            self.logger.info('AutocRED experiment starting...')
-        elif self.mode == 2:
-            self.logger.info('Full AutocRED experiment starting...')
-        elif self.mode == 3:
-            self.logger.info('Full AutocRED with auto crystal finder experiment starting...')
-        self.logger.info('Data recording started at: {}'.format(datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')))
-        self.logger.info(f'Data saving path: {path}')
-        self.logger.info(f'Data collection exposure time: {self.expt} s')
-        self.logger.info(f'Data collection spot size: {spotsize}')
-        # TODO: Mostly above is setup, split off into own function
-
-        buffer = []
-        image_buffer = []
-
-        if self.mode > 0:
-
-            if self.verbose:
-                print('Auto tracking feature activated. Please remember to bring sample to proper Z height in order for autotracking to be effective.')
-
-            transform_imgshift_ = np.linalg.inv(transform_imgshift)
-            transform_imgshift2_ = np.linalg.inv(transform_imgshift2)
-            transform_imgshift_foc_ = np.linalg.inv(transform_imgshift_foc)
-            transform_imgshift2_foc_ = np.linalg.inv(transform_imgshift2_foc)
-
-            transform_beamshift_d_ = np.linalg.inv(transform_beamshift_d)
-
-            self.logger.debug(f'Transform_imgshift: {transform_imgshift}')
-            self.logger.debug(f'Transform_imgshift_foc: {transform_imgshift_foc}')
-            self.logger.debug(f'Transform_imgshift2: {transform_imgshift2}')
-            self.logger.debug(f'Transform_imgshift2_foc: {transform_imgshift2_foc}')
-
-            if self.ctrl.mode != 'diff':
-                self.ctrl.mode.set('samag')
-                self.ctrl.mode.set('diff')
-
-            bs_x0, bs_y0 = self.ctrl.beamshift.get()
-            is_x0, is_y0 = self.ctrl.imageshift1.get()
-            ds_x0, ds_y0 = self.ctrl.diffshift.get()
-            is2_x0, is2_y0 = self.ctrl.imageshift2.get()
-
-            is1_init = (is_x0, is_y0)
-            is2_init = (is2_x0, is2_y0)
-
-            self.logger.debug(f'Initial Beamshift: {bs_x0}, {bs_y0}')
-            self.logger.debug(f'Initial Imageshift1: {is_x0}, {is_y0}')
-            self.logger.debug(f'Initial Imageshift2: {is2_x0}, {is2_y0}')
-
-            diff_focus_proper = self.ctrl.difffocus.value
-            diff_focus_defocused = diff_focus_proper + self.diff_defocus
-
-            img0, h = self.defocus_and_image(difffocus=self.diff_defocus, exp_t=self.exposure_time_image)
-
-            """if trackmethod == "p":
-                shift = self.tracking_by_particlerecog(img0)
-                delta_beamshiftcoord = np.matmul(self.calib_beamshift.transform, shift)
-                self.logger.debug("Beam shift coordinates: {}".format(delta_beamshiftcoord))
-
-                bs_x0, bs_y0 = self.setandupdate_bs(bs_x0, bs_y0, delta_beamshiftcoord)
-
-                img0, h = self.defocus_and_image(difffocus = self.diff_defocus, exp_t = self.exposure_time_image)"""
-
-            img0_p = preprocess(img0.astype(float))
-            scorefromCNN = predict(img0_p)
-            # self.print_and_log(logger = self.logger, msg = "Score for the DP: {}".format(scorefromCNN))
-            self.logger.debug(f'Score for the DP: {scorefromCNN}')
-
-            crystal_pos, img0_cropped, window_size = self.image_cropper(img=img0, window_size=0)
-            img0var = self.img_var(img0_cropped, crystal_pos)
-            appos0 = crystal_pos
-
-            self.logger.debug(f'Tracking method: {trackmethod}. Initial crystal_pos: {crystal_pos} by find_defocused_image_center.')
-
-        if self.unblank_beam:
-            self.ctrl.beam.unblank()
-
-        if self.mode > 1:
-            a_i = self.ctrl.stage.a
-
-            rotation_range = self.rotrangelimit + abs(a_i)
-            rotation_t = rotation_range / self.rotation_speed
-
-            try:
-                if self.rotation_direction == 0:
-                    self.ctrl.stage.set(a=a_i + rotation_range, wait=False)
-                else:
-                    self.ctrl.stage.set(a=a_i - rotation_range, wait=False)
-            except BaseException:
-                if a_i < 0:
-                    self.ctrl.stage.set(a=a_i + rotation_range, wait=False)
-                else:
-                    self.ctrl.stage.set(a=a_i - rotation_range, wait=False)
-
-        if self.camtype == 'simulate':
-            self.startangle = a
-        else:
-            time.sleep(self.angle_activation)
-
-        i = 1
-
-        numb_robustTrack = 0
-        """Turn on and off for crystal movement guess here"""
-        self.guess_crystmove = False
-
-        """set acquisition time to be around 0.52 s in order to fix the image interval times."""
-        acquisition_time = self.expt + 0.02
-
-        self.ctrl.cam.block()
-        """To ensure lock got released in the block step."""
-        time.sleep(0.1)
-
-        t0 = time.perf_counter()
-        self.startangle = a
-
-        self.stopEvent.clear()
-
-        while not self.stopEvent.is_set():
-            try:
-                if i < self.nom_ii:
-                    self.image_interval = self.robust_ii
-                    numb_robustTrack += 1
-                else:
-                    self.image_interval = self.nom_ii
-
-                    """If variance changed over 20%, do a robust check to ensure crystal is back"""
-
-                    if imgvar / img0var < 0.5 or imgvar / img0var > 2 or imgscale / imgscale0 > 1.15 or imgscale / imgscale0 < 0.85:
-                        self.image_interval = self.robust_ii
-                        numb_robustTrack += 1
-                    else:
-                        self.image_interval = self.nom_ii
-                        numb_robustTrack = 0
-
-                if numb_robustTrack > 10:
-                    self.image_interval = self.nom_ii
-                    img0var = imgvar
-                    imgscale0 = imgscale
-                    numb_robustTrack = 0
-
-                if i % self.image_interval == 0:  # aim to make this more dynamically adapted...
-                    t_start = time.perf_counter()
-
-                    """Guessing the next particle position by simply apply the same beamshift change as previous"""
-                    if self.guess_crystmove and i >= self.nom_ii:
-                        bs_x0, bs_y0 = self.setandupdate_bs(bs_x0, bs_y0, delta_beamshiftcoord)
-
-                    self.ctrl.difffocus.value = diff_focus_defocused
-                    img, h = self.ctrl.get_image(self.exposure_time_image, header_keys=None)
-                    self.ctrl.difffocus.value = diff_focus_proper
-
-                    image_buffer.append((i, img, h))
-
-                    crystal_pos, img_cropped, _ = self.image_cropper(img=img, window_size=window_size)
-
-                    self.logger.debug(f'crystal_pos: {crystal_pos} by find_defocused_image_center.')
-
-                    imgvar = self.img_var(img_cropped, crystal_pos)
-
-                    self.logger.debug(f'Image variance: {imgvar}')
-
-                    """If variance changed over 50%, then the crystal is outside the beam and stop data collection"""
-                    if imgvar / img0var < 0.2 or imgvar / img0var > 5:
-                        self.print_and_del('Collection stopping because crystal out of the beam...')
-                        self.stopEvent.set()
-                    if imgvar < self.imgvar_threshold:
-                        self.print_and_del('Image variance smaller than blank image.')
-                        self.stopEvent.set()
-
-                    if trackmethod == 'c':
-
-                        cc, err, diffphase = phase_cross_correlation(img0_cropped, img_cropped)
-                        self.logger.debug(f'Cross correlation result: {cc}')
-
-                        if self.guess_crystmove and i >= self.nom_ii:
-                            delta_beamshiftcoord1 = np.matmul(self.calib_beamshift.transform, cc)
-                            # print("Beam shift coordinates: {}".format(delta_beamshiftcoord))
-                            self.logger.debug(f'Beam shift coordinates: {delta_beamshiftcoord1}')
-                            bs_x0, bs_y0 = self.setandupdate_bs(bs_x0, bs_y0, delta_beamshiftcoord1)
-
-                            delta_beamshiftcoord = delta_beamshiftcoord1 + delta_beamshiftcoord
-
-                        else:
-                            delta_beamshiftcoord = np.matmul(self.calib_beamshift.transform, cc)
-                            # print("Beam shift coordinates: {}".format(delta_beamshiftcoord))
-                            self.logger.debug(f'Beam shift coordinates: {delta_beamshiftcoord}')
-                            bs_x0, bs_y0 = self.setandupdate_bs(bs_x0, bs_y0, delta_beamshiftcoord)
-
-                    elif trackmethod == 'p':
-
-                        shift = self.tracking_by_particlerecog(img)
-                        delta_beamshiftcoord = np.matmul(shift, transform_beamshift_d_defoc)
-                        self.logger.debug(f'Beam shift coordinates: {delta_beamshiftcoord}')
-
-                        bs_x0, bs_y0 = self.setandupdate_bs(bs_x0, bs_y0, delta_beamshiftcoord)
-
-                        if shift[0] == 512:
-                            self.stopEvent.set()
-                            continue
-
-                    if self.check_lens_close_to_limit_warning(lensname='beamshift', lensvalue=bs_x0) or self.check_lens_close_to_limit_warning(lensname='beamshift', lensvalue=bs_y0):
-                        self.logger.debug(f'Beamshift close to limit warning: bs_x0 = {bs_x0}, bs_y0 = {bs_y0}')
-                        self.stopEvent.set()
-
-                    crystal_pos, r = find_defocused_image_center(img)
-                    crystal_pos = crystal_pos[::-1]
-                    crystal_pos_dif = crystal_pos - appos0
-                    apmv = -crystal_pos_dif
-                    dpmv = delta_beamshiftcoord @ transform_beamshift_d_
-                    R = -transform_imgshift2_foc_ @ transform_imgshift_foc @ transform_imgshift_ + transform_imgshift2_
-                    mv = apmv - dpmv @ transform_imgshift_foc @ transform_imgshift_
-                    delta_imageshift2coord = np.matmul(mv, np.linalg.inv(R))
-                    delta_imageshiftcoord = dpmv @ transform_imgshift_foc - delta_imageshift2coord @ transform_imgshift2_foc_ @ transform_imgshift_foc
-
-                    diff_shift = delta_imageshiftcoord @ transform_imgshift_foc_ + delta_imageshift2coord @ transform_imgshift2_foc_
-                    img_shift = delta_imageshiftcoord @ transform_imgshift_ + delta_imageshift2coord @ transform_imgshift2_
-
-                    self.logger.debug(f'delta imageshiftcoord: {delta_imageshiftcoord}, delta imageshift2coord: {delta_imageshift2coord}')
-
-                    self.ctrl.imageshift1.set(x=is_x0 - int(delta_imageshiftcoord[0]), y=is_y0 - int(delta_imageshiftcoord[1]))
-                    self.ctrl.imageshift2.set(x=is2_x0 - int(delta_imageshift2coord[0]), y=is2_y0 - int(delta_imageshift2coord[1]))
-
-                    is_x0 = is_x0 - int(delta_imageshiftcoord[0])
-                    is_y0 = is_y0 - int(delta_imageshiftcoord[1])
-                    is2_x0 = is2_x0 - int(delta_imageshift2coord[0])
-                    is2_y0 = is2_y0 - int(delta_imageshift2coord[1])
-
-                    if self.check_lens_close_to_limit_warning(lensname='imageshift1', lensvalue=is_x0) or self.check_lens_close_to_limit_warning(lensname='imageshift1', lensvalue=is_y0) or self.check_lens_close_to_limit_warning(lensname='imageshift2', lensvalue=is2_x0) or self.check_lens_close_to_limit_warning(lensname='imageshift2', lensvalue=is2_y0):
-                        self.logger.debug(f'Imageshift close to limit warning: is_x0 = {is_x0}, is_y0 = {is_y0}, is2_x0 = {is2_x0}, is2_y0 = {is2_y0}')
-                        self.stopEvent.set()
-
-                    self.logger.debug(f'Image Interval: {self.image_interval}, Imgvar/Img0var:{imgvar / img0var}')
-
-                    next_interval = t_start + acquisition_time
-
-                    while time.perf_counter() > next_interval:
-                        self.logger.debug('Skipping one image.')
-                        next_interval += acquisition_time
-                        i += 1
-
-                    diff = next_interval - time.perf_counter()
-                    time.sleep(diff)
-
-                else:
-                    t_start = time.perf_counter()
-                    img, h = self.ctrl.get_image(self.expt, header_keys=None)
-                    if buffer == []:
-                        imgscale0 = np.sum(img)
-                    else:
-                        imgscale = np.sum(img)
-                        self.logger.debug(f'Image scale variation: {imgscale / imgscale0}')
-
-                    buffer.append((i, img, h))
-
-                    next_interval = t_start + acquisition_time
-
-                    while time.perf_counter() > next_interval:
-                        next_interval += acquisition_time
-                        self.logger.debug('One image skipped because of too long acquisition or calculation time.')
-                        i += 1
-
-                    diff = next_interval - time.perf_counter()
-                    time.sleep(diff)
-
-                i += 1
-
-                if time.perf_counter() - t0 >= rotation_t:
-                    self.stopEvent.set()
-                    self.print_and_del('Goniometer close to limit!')
-
-            except Exception as e:
-                self.print_and_del(e)
-                self.stopEvent.set()
-
-        t1 = time.perf_counter()
-
-        self.ctrl.cam.unblock()
-        if self.mode > 1:
-            self.ctrl.stage.stop()
-
-        if self.camtype == 'simulate':
-            self.endangle = self.startangle + np.random.random() * 50
-            camera_length = 300
-        else:
-            self.endangle = self.ctrl.stage.a
-            camera_length = int(self.ctrl.magnification.get())
-
-        if self.unblank_beam:
-            # print("Blanking beam")
-            self.ctrl.beam.blank()
-
-        self.stopEvent.clear()
-
-        self.ctrl.imageshift1.set(x=is1_init[0], y=is1_init[1])
-        self.ctrl.imageshift2.set(x=is2_init[0], y=is2_init[1])
-
-        # stage_positions = tracer.stop()
-        stageposx, stageposy, stageposz, stageposa, stageposb = self.ctrl.stage.get()
-        rotrange = abs(self.endangle - self.startangle)
-
-        if self.verbose:
-            print(f'Rotated {abs(self.endangle - self.startangle):.2f} degrees from {self.startangle:.2f} to {self.endangle:.2f}')
-
-        self.logger.info(f'Rotated {abs(self.endangle - self.startangle):.2f} degrees from {self.startangle:.2f} to {self.endangle:.2f}')
-
-        nframes = i - 1  # i + 1 is not correct since i+=1 was executed before next image is taken???
-        osangle = abs(self.endangle - self.startangle) / nframes
-        acquisition_time = (t1 - t0) / nframes
-
-        self.logger.info(f'Data collection camera length: {camera_length} mm')
-        self.logger.info(f'Data collected from {self.startangle} degree to {self.endangle} degree.')
-        self.logger.info(f'Oscillation angle: {osangle}')
-        self.logger.info('Pixel size and actual camera length updated in SMV file headers for DIALS processing.')
-
-        rotation_angle = config.camera.camera_rotation_vs_stage_xy
-
-        self.pixelsize = config.calibration['diff']['pixelsize'][camera_length]  # px / Angstrom
-        self.physical_pixelsize = config.camera.physical_pixelsize  # mm
-        self.wavelength = config.microscope.wavelength  # angstrom
-        self.stretch_azimuth = config.camera.stretch_azimuth
-        self.stretch_amplitude = config.camera.stretch_amplitude
-
-        now = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-
-        with open(os.path.join(path, 'cRED_log.txt'), 'w') as f:
-            print(f'Data Collection Time: {now}', file=f)
-            print(f'Starting angle: {self.startangle}', file=f)
-            print(f'Ending angle: {self.endangle}', file=f)
-            print(f'Exposure Time: {self.expt} s', file=f)
-            print(f'Spot Size: {spotsize}', file=f)
-            print(f'Camera length: {camera_length} mm\n', file=f)
-            print(f'Pixelsize: {self.pixelsize} px/Angstrom', file=f)
-            print(f'Physical pixelsize: {self.physical_pixelsize} um', file=f)
-            print(f'Wavelength: {self.wavelength} Angstrom', file=f)
-            print(f'Stretch amplitude: {self.stretch_azimuth} %', file=f)
-            print(f'Stretch azimuth: {self.stretch_amplitude} degrees', file=f)
-            print(f'Rotation axis: {rotation_angle} radians', file=f)
-            print(f'Oscillation angle: {osangle} degrees', file=f)
-            print(f'Number of frames: {len(buffer)}', file=f)
-            print(f'Particle found at stage position: x: {stageposx}, y: {stageposy}, z: {stageposz}', file=f)
-
-        with open(log_rotaterange, 'a') as f:
-            f.write(f'{stageposx}\t{stageposy}\t{stageposz}\t{rotrange}\n')
-
-        img_conv = ImgConversion(buffer=buffer,
-                                 osc_angle=osangle,
-                                 start_angle=self.startangle,
-                                 end_angle=self.endangle,
-                                 rotation_axis=rotation_angle,
-                                 acquisition_time=acquisition_time,
-                                 flatfield=self.flatfield,
-                                 pixelsize=self.pixelsize,
-                                 physical_pixelsize=self.physical_pixelsize,
-                                 wavelength=self.wavelength,
-                                 stretch_amplitude=self.stretch_amplitude,
-                                 stretch_azimuth=self.stretch_azimuth,
-                                 )
-
-        img_conv.tiff_writer(pathtiff)
-        img_conv.smv_writer(pathsmv)
-        img_conv.mrc_writer(pathred)
-        img_conv.write_ed3d(pathred)
-        img_conv.write_xds_inp(pathsmv)
-
-        img_conv.to_dials(pathsmv)
-        pathsmv_str = str(pathsmv)
-        msg = {'path': pathsmv_str,
-               'rotrange': rotrange,
-               'nframes': nframes,
-               'osc': osangle}
-        msg_tosend = json.dumps(msg).encode('utf8')
-
-        if self.s_c:
-            self.s.send(msg_tosend)
-            self.print_and_del('SMVs sent to DIALS for processing.')
-
-        if self.s2_c:
-            self.s2.send(msg_tosend)
-            self.print_and_del('SMVs sent to XDS for processing.')
-
-        #self.logger.info("XDS INP file created.")
-
-        if image_buffer:
-            drc = os.path.join(path, 'tiff_image')
-            os.makedirs(drc)
-            while len(image_buffer) != 0:
-                i, img, h = image_buffer.pop(0)
-                fn = os.path.join(drc, f'{i:05d}.tiff')
-                write_tiff(fn, img, header=h)
-
-        self.ctrl.beam.unblank()
-        self.number_exp_performed += 1
-        if self.verbose:
-            print('Data Collection and Conversion Done.')
-
-    def write_BrightnessStates(self, n_cycles=2):
-        print('Go to your desired magnification and camera length. Now recording lens states...')
-        self.ctrl.mode.set('mag1')
-        input('Please choose the desired magnification, partially converge the beam in MAG1 to around 1 um in diameter, and center it using beamshift. Press ENTER when ready')
-
-        for i in range(0, n_cycles):
-            self.hysteresis_check()
-            input('Please recenter the beam with beamshift. Press ENTER when ready')
-
-        desired_mag = self.ctrl.magnification.get()
-        img_brightness = self.ctrl.brightness.value
-        bs = self.ctrl.beamshift.get()
-
-        self.ctrl.mode.set('samag')
-        self.ctrl.mode.set('diff')
-        input('Please go to diffraction mode, choose desired camera length, focus the diffraction spots, and center it using PLA. Press ENTER when ready')
-        for i in range(0, n_cycles):
-            self.hysteresis_check()
-            input('Please recenter the diffraction spot using PLA. Press ENTER when ready')
-
-        desired_cl = self.ctrl.magnification.get()
-        dp_focus = self.ctrl.difffocus.value
-        is1status = self.ctrl.imageshift1.get()
-        is2status = self.ctrl.imageshift2.get()
-        plastatus = self.ctrl.diffshift.get()
-        with open(self.calibdir / 'beam_brightness.pkl', 'wb') as f:
-            pickle.dump([img_brightness, bs, dp_focus, is1status, is2status, plastatus, desired_mag, desired_cl], f)
-
-        print('Brightness recorded.')
-        return [img_brightness, bs, dp_focus, is1status, is2status, plastatus, desired_mag, desired_cl]
-
-    def update_referencepoint_bs(self, bs, br):
-        exposure = 0.01
-        binsize = 1
-        scale = 1
-        self.ctrl.beamshift.set(*bs)
-        self.ctrl.brightness.value = br
-
-        img_cent = self.ctrl.get_raw_image(exposure=exposure, binsize=binsize)
-
-        if np.mean(img_cent) > 10:
-
-            pixel_cent = np.array(find_beam_center(img_cent)) * binsize / scale
-
-            # print(pixel_cent)
-
-            self.calib_beamshift.reference_shift = bs
-            self.calib_beamshift.reference_pixel = pixel_cent
-
-            return self.calib_beamshift.reference_pixel
-        else:
-            return self.calib_beamshift.reference_pixel
-
-    def raster_scan(self):
-        from instamatic.experiments.serialed.experiment import get_offsets_in_scan_area
-        pixelsize_mag1 = config.calibration['mag1']['pixelsize'][self.magnification] / 1000  # nm -> um
-        xdim, ydim = self.ctrl.getCameraDimensions()
-        box_x, box_y = self.pixelsize_mag1 * xdim, self.pixelsize_mag1 * ydim
-
-        # Make negative to reflect config change 2019-07-03 to make omega more in line with other software
-        rot_axis = -config.camera.camera_rotation_vs_stage_xy
-
-        offsets = get_offsets_in_scan_area(box_x, box_y, self.scan_area, angle=rot_axis)
-        self.offsets = offsets * 1000
-
-        center_x = self.ctrl.stage.x
-        center_y = self.ctrl.stage.y
-
-        x_zheight = 0
-        y_zheight = 0
-
-        t = tqdm(self.offsets, desc=f'Number of crystals scanned: {self.number_crystals_scanned}; Number of experiments performed: {self.number_exp_performed}')
-
-        for j, (x_offset, y_offset) in enumerate(t):
-            x = center_x + x_offset
-            y = center_y + y_offset
-
-            self.ctrl.stage.set(x=x, y=y)
-            # print("Stage position: x = {}, y = {}".format(x,y))
-            x_change = x - x_zheight
-            y_change = y - y_zheight
-            dist = np.linalg.norm((x_change, y_change))
-
-            if dist > 50000 or x_zheight * y_zheight == 0 or x_zheight == 999999:
-                try:
-                    img, h = self.ctrl.get_image(exposure=self.expt, header_keys=None)
-                    if img.mean() > 10:
-                        self.magnification = self.ctrl.magnification.value
-                        crystal_positions = find_crystals_timepix(img, self.magnification, spread=self.spread, offset=self.offset)
-                        crystal_coords = [(crystal.x, crystal.y) for crystal in crystal_positions]
-
-                        n_crystals = len(crystal_coords)
-                        if n_crystals > 0:
-                            self.print_and_del('centering z height...')
-                            x_zheight, y_zheight = center_z_height_HYMethod(self.ctrl, spread=self.spread, offset=self.offset)
-                            if x_zheight != 999999:
-                                xpoint, ypoint, zpoint, aaa, bbb = self.ctrl.stage.get()
-                                self.logger.info(f'Stage position: x = {xpoint}, y = {ypoint}. Z height adjusted to {zpoint}. Tilt angle x {aaa} deg, Tilt angle y {bbb} deg')
-                            else:
-                                self.print_and_del('Z height not found.')
-                except BaseException:
-                    self.print_and_del('Something went wrong, unable to adjust height')
-                    pass
-
-            self.start_collection_point()
-
-            t.set_description(f'Number of crystals scanned: {self.number_crystals_scanned}; Number of experiments performed: {self.number_exp_performed}')
-
-            if self.stopEvent_rasterScan.is_set():
-                print('\nRaster Scan stopped manually.')
-                break
-
-    def start_collection_point(self):
-
-        IS1_Neut = self.ctrl.imageshift1.get()
-        IS2_Neut = self.ctrl.imageshift2.get()
-
-        path = self.path
-
-        if self.scan_area != 0:
-            path = path / f'stagepos_{self.stagepos_idx:04d}'
-            self.stagepos_idx += 1
-            if not os.path.exists(path):
-                os.makedirs(path)
-
-        try:
-            with open(self.calibdir / 'beam_brightness.pkl', 'rb') as f:
-                [img_brightness, bs, dp_focus, is1status, is2status, plastatus, desired_mag, desired_cl] = pickle.load(f)
-        except OSError:
-            [img_brightness, bs, dp_focus, is1status, is2status, plastatus, desired_mag, desired_cl] = self.write_BrightnessStates()
-
-        try:
-            self.calib_beamshift = CalibBeamShift.from_file(fn=self.calibdir / CALIB_BEAMSHIFT)
-            self.ctrl.beamshift.set(x=self.calib_beamshift.reference_shift[0], y=self.calib_beamshift.reference_shift[1])
-
-        except OSError:
-            print('No beam shift calibration result found. Running instamatic.calibrate_beamshift first...\n')
-            print('Going to MAG1, desired magnification, and desired brightness. DO NOT change brightness!')
-            if self.ctrl.mode != 'mag1':
-                self.ctrl.mode.set('mag1')
-                self.ctrl.magnification.value = desired_mag
-                self.ctrl.brightness.value = img_brightness
-
-            calib_file = 'x'
-            while calib_file == 'x':
-                print('Find a clear area, toggle the beam to the desired defocus value.')
-                self.calib_beamshift = calibrate_beamshift(ctrl=self.ctrl, outdir=self.calibdir)
-                print('Beam shift calibration done.')
-                calib_file = input('Press ENTER when ready to continue. Press x to REDO the calibration.')
-
-        self.logger.debug(f'Transform_beamshift: {self.calib_beamshift.transform}')
-
-        try:
-            self.calib_directbeam = CalibDirectBeam.from_file(fn=self.calibdir / CALIB_DIRECTBEAM)
-            with open(self.calibdir / 'diff_par.pkl', 'rb') as f:
-                self.diff_brightness, self.diff_difffocus = pickle.load(f)
-        except OSError:
-            if not self.ctrl.mode == 'diff':
-                self.ctrl.mode.set('samag')
-                self.ctrl.imageshift1.set(x=is1status[0], y=is1status[1])
-                self.ctrl.imageshift2.set(x=is2status[0], y=is2status[1])
-                self.ctrl.mode.set('diff')
-            self.ctrl.difffocus.value = dp_focus
-
-            self.calib_directbeam = CalibDirectBeam.live(self.ctrl, outdir=self.calibdir)
-            self.diff_brightness = self.ctrl.brightness.value
-            self.diff_difffocus = self.ctrl.difffocus.value
-            with open(self.calibdir / 'diff_par.pkl', 'wb') as f:
-                pickle.dump([self.diff_brightness, self.diff_difffocus], f)
-
-        try:
-            with open(self.calibdir / 'imgvariance.pkl', 'rb') as f:
-                self.imgvar_threshold, self.beam_size_avg = pickle.load(f)
-        except OSError:
-            self.imgvar_threshold, self.beam_size_avg = self.imagevar_blank_estimator(brightness=img_brightness)
-            with open(self.calibdir / 'imgvariance.pkl', 'wb') as f:
-                pickle.dump([self.imgvar_threshold, self.beam_size_avg], f)
-
-        self.neutral_beamshift = bs
-        # print("Neutral beamshift: from beam_brightness.pkl {}".format(bs))
-        self.neutral_diffshift = plastatus
-
-        self.calib_beamshift.reference_pixel = self.update_referencepoint_bs(bs, img_brightness)
-
-        # print("Calib_beamshift_referenceshift: {}".format(self.calib_beamshift.reference_shift))
-
-        transform_imgshift, c = load_IS_Calibrations(imageshift='IS1', ctrl=self.ctrl, diff_defocus=self.diff_defocus, logger=self.logger, mode='diff')
-        transform_imgshift2, c = load_IS_Calibrations(imageshift='IS2', ctrl=self.ctrl, diff_defocus=self.diff_defocus, logger=self.logger, mode='diff')
-        transform_imgshift_foc, c = load_IS_Calibrations(imageshift='IS1', ctrl=self.ctrl, diff_defocus=0, logger=self.logger, mode='diff')
-        transform_imgshift2_foc, c = load_IS_Calibrations(imageshift='IS2', ctrl=self.ctrl, diff_defocus=0, logger=self.logger, mode='diff')
-
-        transform_beamshift_d, c = load_IS_Calibrations(imageshift='BS', ctrl=self.ctrl, diff_defocus=0, logger=self.logger, mode='diff')
-        transform_beamshift_d_defoc, c = load_IS_Calibrations(imageshift='BS', ctrl=self.ctrl, diff_defocus=self.diff_defocus, logger=self.logger, mode='diff')
-        # transform_beamshift_d = self.calib_beamshift.transform
-
-        transform_stagepos, c = load_IS_Calibrations(imageshift='S', ctrl=self.ctrl, diff_defocus=0, logger=self.logger, mode='mag1')
-
-        if self.mode == 3:
-            # ready = input("Please make sure that you are in the super user mode and the rotation speed is set via GONIOTOOL! Press ENTER to continue.")
-
-            if self.ctrl.mode != 'mag1':
-                self.ctrl.mode.set('mag1')
-
-            self.ctrl.magnification.value = desired_mag
-            self.ctrl.brightness.value = 65535
-
-            header_keys = None
-
-            if self.verbose:
-                print(f'Beamshift reference: {self.calib_beamshift.reference_shift}')
-
-            self.ctrl.beamshift.set(x=self.calib_beamshift.reference_shift[0], y=self.calib_beamshift.reference_shift[1])
-
-            self.magnification = self.ctrl.magnification.value
-
-            self.rotation_direction = self.eliminate_backlash_in_tiltx()
-            img, h = self.ctrl.get_image(exposure=self.expt, header_keys=header_keys)
-            # img, h = Experiment.apply_corrections(img, h)
-
-            threshold = 10  # ignore black images
-
-            if img.mean() > threshold:
-
-                h['exp_magnification'] = self.ctrl.magnification.get()
-
-                write_tiff(path / 'Overall_view', img, h)
-
-                crystal_positions = find_crystals_timepix(img, self.magnification, spread=self.spread, offset=self.offset)
-                crystal_coords = [(crystal.x, crystal.y) for crystal in crystal_positions]
-
-                n_crystals = len(crystal_coords)
-
-                if n_crystals == 0:
-                    self.print_and_del('No crystals found in the image. Find another area!')
-                    return 0
-
-                (beamshiftcoord_0, size_crystal_targeted) = self.center_particle_from_crystalList(crystal_positions, transform_stagepos, self.magnification, self.beam_size_avg)
-
-                img, h = self.ctrl.get_image(exposure=self.expt, header_keys=header_keys)
-                h['exp_magnification'] = self.ctrl.magnification.get()
-                write_tiff(path / 'Overall_view', img, h)
-
-                crystal_positions = find_crystals_timepix(img, self.magnification, spread=self.spread, offset=self.offset)
-                crystal_coords = [(crystal.x, crystal.y) for crystal in crystal_positions]
-                crystal_sizes = [crystal.area_pixel for crystal in crystal_positions]
-                n_crystals = len(crystal_coords)
-
-                if n_crystals == 0:
-                    self.print_and_del('No crystals found in the image. Find another area!')
-                    return 0
-
-                if size_crystal_targeted != 0:
-                    try:
-                        ind_target = crystal_sizes.index(size_crystal_targeted)
-                        crystal_coords[0], crystal_coords[ind_target] = crystal_coords[ind_target], crystal_coords[0]
-                        self.print_and_del('Targeted isolated crystal centered is swapped to the first of the list.')
-                    except ValueError:
-                        self.print_and_del('Lost targeted isolated crystal.')
-                        return 0
-
-                self.logger.info(f'{datetime.datetime.now()} {n_crystals} crystals found.')
-
-                k = 0
-
-                while not self.stopEvent_rasterScan.is_set():
-
-                    try:
-                        self.ctrl.brightness.value = img_brightness
-
-                        if self.verbose:
-                            print(f'Collecting on crystal {k + 1}/{n_crystals}. Beamshift coordinates: {self.ctrl.beamshift.get()}')
-
-                        outfile = path / f'crystal_{k:04d}'
-                        comment = f'crystal {k}'
-
-                        beamshift_coords = np.array(bs) - np.dot(crystal_coords[k] - self.calib_beamshift.reference_pixel, self.calib_beamshift.transform)
-                        self.ctrl.beamshift.set(*beamshift_coords.astype(int))
-
-                        img, h = self.ctrl.get_image(exposure=0.001, comment=comment, header_keys=header_keys)
-                        h['exp_magnification'] = self.ctrl.magnification.get()
-                        write_tiff(path / f'crystal_{k:04d}', img, h)
-
-                        self.number_crystals_scanned += 1
-
-                        if self.isolated(crystal_positions[k], crystal_coords) and crystal_positions[k].isolated and not any(t < 100 for t in crystal_coords[k]) and not any(t > 416 for t in crystal_coords[k]):
-
-                            self.ctrl.mode.set('samag')
-                            self.ctrl.mode.set('diff')
-                            self.ctrl.imageshift1.set(x=is1status[0], y=is1status[1])
-                            self.ctrl.imageshift2.set(x=is2status[0], y=is2status[1])
-                            self.ctrl.diffshift.set(x=plastatus[0], y=plastatus[1])
-
-                            # compensate beamshift
-                            beamshift_offset = beamshift_coords - self.neutral_beamshift
-                            pixelshift = self.calib_directbeam.beamshift2pixelshift(beamshift_offset)
-
-                            diffshift_offset = self.calib_directbeam.pixelshift2diffshift(pixelshift)
-                            diffshift = self.neutral_diffshift - diffshift_offset
-
-                            self.ctrl.diffshift.set(*diffshift.astype(int))
-
-                            pathtiff = outfile / 'tiff'
-                            pathsmv = outfile / 'SMV'
-                            pathred = outfile / 'RED'
-
-                            self.auto_cred_collection(outfile, pathtiff, pathsmv, pathred, transform_imgshift, transform_imgshift2, transform_imgshift_foc, transform_imgshift2_foc, transform_beamshift_d, transform_beamshift_d_defoc, self.calib_beamshift)
-
-                            self.ctrl.beamshift.set(x=self.calib_beamshift.reference_shift[0], y=self.calib_beamshift.reference_shift[1])
-                            self.ctrl.mode.set('mag1')
-                            self.ctrl.brightness.value = 65535
-                            time.sleep(0.5)
-
-                            self.rotation_direction = self.eliminate_backlash_in_tiltx()
-                            img, h = self.ctrl.get_image(exposure=self.expt, header_keys=header_keys)
-                            h['exp_magnification'] = self.ctrl.magnification.get()
-                            write_tiff(path / f'Overall_view_{k:04d}', img, h)
-
-                            crystal_positions = find_crystals_timepix(img, self.magnification, spread=self.spread, offset=self.offset)
-                            crystal_coords = [(crystal.x, crystal.y) for crystal in crystal_positions]
-                            # self.ctrl.brightness.value = img_brightness
-
-                            if n_crystals == 0:
-                                self.print_and_del('No crystals found in the image. exitting loop...')
-                                break
-
-                            (beamshiftcoord_0, size_crystal_targeted) = self.center_particle_from_crystalList(crystal_positions, transform_stagepos, self.magnification, self.beam_size_avg)
-
-                            img, h = self.ctrl.get_image(exposure=self.expt, header_keys=header_keys)
-                            h['exp_magnification'] = self.ctrl.magnification.get()
-                            write_tiff(path / f'Overall_view_{k:04d}', img, h)
-
-                            crystal_positions = find_crystals_timepix(img, self.magnification, spread=self.spread, offset=self.offset)
-                            crystal_coords = [(crystal.x, crystal.y) for crystal in crystal_positions]
-                            crystal_sizes = [crystal.area_pixel for crystal in crystal_positions]
-                            n_crystals = len(crystal_coords)
-
-                            if n_crystals == 0:
-                                self.print_and_del('No crystals found in the image. Find another area!')
-                                break
-
-                            if size_crystal_targeted != 0:
-                                try:
-                                    ind_target = crystal_sizes.index(size_crystal_targeted)
-                                    crystal_coords[k + 1], crystal_coords[ind_target] = crystal_coords[ind_target], crystal_coords[k + 1]
-                                    self.print_and_del('Targeted isolated crystal centered is swapped to the next.')
-                                except ValueError:
-                                    self.print_and_del('Lost targeted isolated crystal.')
-                                    break
-
-                        else:
-                            if self.verbose:
-                                print(f'Crystal {k + 1} not isolated: not suitable for cred collection')
-
-                        k = k + 1
-                        if k >= n_crystals:
-                            break
-                    except BaseException:
-                        traceback.print_exc()
-                        self.ctrl.beam.unblank()
-                        self.print_and_del('Exitting loop...')
-                        break
-
-                self.ctrl.mode.set('mag1')
-                self.ctrl.brightness.value = 65535
-
-                self.ctrl.imageshift1.set(x=IS1_Neut[0], y=IS1_Neut[1])
-                self.ctrl.imageshift2.set(x=IS2_Neut[0], y=IS2_Neut[1])
-
-                self.ctrl.beamshift.set(x=self.calib_beamshift.reference_shift[0], y=self.calib_beamshift.reference_shift[1])
-
-                if self.verbose:
-                    print('AutocRED with crystal_finder data collection done. Find another area for particles.')
-
-            if os.listdir(path) == ['Overall_view.tiff']:
-                shutil.rmtree(path)
-                # print("Path {} removed since no crystal rotation data was collected.".format(path))
-
-            try:
-                if len(os.listdir(path)) == 0:
-                    os.rmdir(path)
-                    # print("Path {} removed since it is empty.".format(path))
-            except BaseException:
-                # print("Deletion error. Path might have already been deleted.")
-                pass
-
-        elif self.mode == 1 or self.mode == 2:
-            self.pathtiff = Path(self.path) / 'tiff'
-            self.pathsmv = Path(self.path) / 'SMV'
-            self.pathred = Path(self.path) / 'RED'
-
-            for path in (self.path, self.pathtiff, self.pathsmv, self.pathred):
-                if not os.path.exists(path):
-                    os.makedirs(path)
-            self.auto_cred_collection(self.path, self.pathtiff, self.pathsmv, self.pathred, transform_imgshift, transform_imgshift2, transform_imgshift_foc, transform_imgshift2_foc, transform_beamshift_d, transform_beamshift_d_defoc, self.calib_beamshift)
-
-        else:
-            print('Choose cRED tab for data collection with manual/blind tracking.')
-            return 0
-
-    def start_collection(self):
-        ready = input('Please make sure that you have adjusted Goniotool if you are using full autocRED!')
-        if self.stopEvent_rasterScan.is_set():
-            # print("Raster scan stopper clearing..")
-            self.stopEvent_rasterScan.clear()
-
-        if not self.auto_zheight:
-            try:
-                with open(self.calibdir / 'z-height-adjustment-time.pkl', 'rb') as f:
-                    t = pickle.load(f)
-                    if t - time.perf_counter() > 14400:
-                        self.print_and_del('Z-height needs to be updated every session. Readjusting z-height...')
-                        x_zheight, y_zheight = center_z_height_HYMethod(self.ctrl, spread=self.spread, offset=self.offset)
-                        xpoint, ypoint, zpoint, aaa, bbb = self.ctrl.stage.get()
-                        self.logger.info(f'Stage position: x = {xpoint}, y = {ypoint}. Z height adjusted to {zpoint}. Tilt angle x {aaa} deg, Tilt angle y {bbb} deg')
-                        t = time.perf_counter()
-                        with open(self.calibdir / 'z-height-adjustment-time.pkl', 'wb') as f:
-                            pickle.dump(t, f)
-
-            except BaseException:
-                input('No z-height adjustment found. Please find an area with particles! Press Enter to continue auto adjustment of z height>>>')
-                x_zheight, y_zheight = center_z_height_HYMethod(self.ctrl, spread=self.spread, offset=self.offset)
-                xpoint, ypoint, zpoint, aaa, bbb = self.ctrl.stage.get()
-                self.logger.info(f'Stage position: x = {xpoint}, y = {ypoint}. Z height adjusted to {zpoint}. Tilt angle x {aaa} deg, Tilt angle y {bbb} deg')
-                t = time.perf_counter()
-                with open(self.calibdir / 'z-height-adjustment-time.pkl', 'wb') as f:
-                    pickle.dump(t, f)
-        else:
-            self.print_and_del('Z height adjusting...')
-            x_zheight, y_zheight = center_z_height_HYMethod(self.ctrl, spread=self.spread, offset=self.offset)
-            xpoint, ypoint, zpoint, aaa, bbb = self.ctrl.stage.get()
-            self.logger.info(f'Stage position: x = {xpoint}, y = {ypoint}. Z height adjusted to {zpoint}. Tilt angle x {aaa} deg, Tilt angle y {bbb} deg')
-            t = time.perf_counter()
-            with open(self.calibdir / 'z-height-adjustment-time.pkl', 'wb') as f:
-                pickle.dump(t, f)
-
-        lensPar = self.ctrl.to_dict()
-        with open(self.calibdir / 'LensPar.pkl', 'wb') as f:
-            pickle.dump(lensPar, f)
-
-        # Check DIALS server connection status here
-
-        if self.scan_area == 0:
-            self.start_collection_point()
-        else:
-            self.raster_scan()
-
-        self.stopEvent_rasterScan.clear()
-
-        with open(self.calibdir / 'LensPar.pkl', 'rb') as f:
-            lensPar_i = pickle.load(f)
-
-        self.ctrl.from_dict(lensPar_i)
-        self.ctrl.beam.blank()
-
-        print('AutocRED collection done.')
-        self.number_crystals_scanned = 0
-        self.number_exp_performed = 0
+import datetime
+import json
+import os
+import pickle
+import shutil
+import socket
+import time
+import traceback
+from pathlib import Path
+
+import numpy as np
+from scipy import ndimage
+from skimage.registration import phase_cross_correlation
+from tqdm.auto import tqdm
+
+from instamatic import config
+from instamatic.calibrate import CalibBeamShift, CalibDirectBeam
+from instamatic.calibrate.calibrate_beamshift import calibrate_beamshift
+from instamatic.calibrate.calibrate_imageshift12 import (
+    Calibrate_Beamshift_D,
+    Calibrate_Beamshift_D_Defoc,
+    Calibrate_Imageshift,
+    Calibrate_Imageshift2,
+    Calibrate_Stage,
+)
+from instamatic.calibrate.center_z import center_z_height_HYMethod
+from instamatic.calibrate.filenames import *
+from instamatic.formats import write_tiff
+from instamatic.neural_network import predict, preprocess
+from instamatic.processing.find_crystals import find_crystals_timepix
+from instamatic.processing.ImgConversionTPX import ImgConversionTPX as ImgConversion
+from instamatic.tools import find_beam_center, find_defocused_image_center
+
+# SerialRED:
+#  Currently only working if live view can be read directly from camera via Python API
+#  Extensively tested on a JEOL 2100 LaB6 TEM with a Timepix camera.
+#  Imgvar can be compared with the first defocused image.
+#  If other particles move in, the variance will be at least 50% different
+
+# spread, offset: parameters for find_crystals_timepix
+# spread = 2  # sometimes crystals still are not so isolated using number 0.6 as suggested.
+# offset = 15  # The number needs to be smaller when the contrast of the crystals is low.
+# imgvar_threshold = 600
+
+date = datetime.datetime.now().strftime('%Y-%m-%d')
+log_rotaterange = config.locations['logs'] / f'Rotrange_stagepos_{date}.log'
+log_iscalibs = config.locations['logs'] / f'ImageShift_LOGS_{date}'
+log_iscalibs.mkdir(exist_ok=True)
+
+if not os.path.isfile(log_rotaterange):
+    with open(log_rotaterange, 'a') as f:
+        f.write('x\ty\tz\trotation range\n')
+
+use_dials = config.settings.use_indexing_server_exe
+use_vm = config.settings.use_VM_server_exe
+
+
+def load_IS_Calibrations(imageshift, ctrl, diff_defocus, logger, mode):
+    if mode == 'diff' or mode == 'mag1':
+        if imageshift == 'IS1' and diff_defocus != 0:
+            file = CALIB_IS1_DEFOC
+        elif imageshift == 'IS2' and diff_defocus != 0:
+            file = CALIB_IS2_DEFOC
+        elif imageshift == 'IS1' and diff_defocus == 0:
+            file = CALIB_IS1_FOC
+        elif imageshift == 'IS2' and diff_defocus == 0:
+            file = CALIB_IS2_FOC
+        elif imageshift == 'BS' and diff_defocus == 0:
+            file = CALIB_BEAMSHIFT_DP
+        elif imageshift == 'BS' and diff_defocus != 0:
+            file = CALIB_BEAMSHIFT_DP_DEFOC
+        elif imageshift == 'S':
+            file = CALIB_STAGE
+    else:
+        print('Wrong input. Mode can either be mag1 or diff for calibration!')
+        return 0
+
+    try:
+        if imageshift == 'S':
+            with open(config.locations['logs'] / file, 'rb') as f:
+                transform_imgshift, c = pickle.load(f)
+        else:
+            with open(log_iscalibs / file, 'rb') as f:
+                transform_imgshift, c = pickle.load(f)
+    except BaseException:
+        print(f'No {imageshift}, defocus = {diff_defocus} calibration found. Choose the desired defocus value.')
+        inp = input('Press ENTER when ready.')
+        if ctrl.mode != mode:
+            ctrl.mode.set(mode)
+        satisfied = 'x'
+        while satisfied == 'x':
+            if imageshift == 'IS1' and diff_defocus != 0:
+                mag_calib = ctrl.magnification.value
+                s_calib = int(200.0 / mag_calib * 1500)
+                transform_imgshift, c = Calibrate_Imageshift(ctrl, diff_defocus, stepsize=s_calib, logger=logger, key='IS1')
+            elif imageshift == 'IS1' and diff_defocus == 0:
+                mag_calib = ctrl.magnification.value
+                s_calib = int(200.0 / mag_calib * 1000)
+                transform_imgshift, c = Calibrate_Imageshift(ctrl, diff_defocus, stepsize=s_calib, logger=logger, key='IS1')
+            elif imageshift == 'IS2':
+                mag_calib = ctrl.magnification.value
+                s_calib = int(200.0 / mag_calib * 750)
+                transform_imgshift, c = Calibrate_Imageshift2(ctrl, diff_defocus, stepsize=s_calib, logger=logger)
+            elif imageshift == 'BS' and diff_defocus == 0:
+                mag_calib = ctrl.magnification.value
+                s_calib = int(250.0 / mag_calib * 100)
+                transform_imgshift, c = Calibrate_Beamshift_D(ctrl, stepsize=s_calib, logger=logger)
+            elif imageshift == 'BS' and diff_defocus != 0:
+                mag_calib = ctrl.magnification.value
+                s_calib = int(250.0 / mag_calib * 100)
+                transform_imgshift, c = Calibrate_Beamshift_D_Defoc(ctrl, diff_defocus, stepsize=s_calib, logger=logger)
+
+            elif imageshift == 'S':
+                mag_calib = ctrl.magnification.value
+                s_calib = int(2500.0 / mag_calib * 1000)
+                transform_imgshift, c = Calibrate_Stage(ctrl, stepsize=s_calib, logger=logger)
+            with open(log_iscalibs / file, 'wb') as f:
+                pickle.dump([transform_imgshift, c], f)
+            satisfied = input(f'{imageshift}, defocus = {diff_defocus} calibration done. \nPress Enter to continue. Press x to redo calibration.')
+
+    return transform_imgshift, c
+
+
+class Experiment:
+    def __init__(self, ctrl,
+                 exposure_time,
+                 exposure_time_image,
+                 stop_event,
+                 stop_event_experiment,
+                 enable_image_interval,
+                 enable_autotrack,
+                 enable_fullacred,
+                 enable_fullacred_crystalfinder,
+                 scan_area,
+                 zheight,
+                 autocenterDP,
+                 angle_activation,
+                 spread,
+                 offset,
+                 rotrange,
+                 backlash_killer,
+                 rotation_speed,
+                 unblank_beam=False,
+                 path=None,
+                 log=None,
+                 flatfield=None,
+                 image_interval=99999,
+                 diff_defocus=0):
+        super().__init__()
+        self.ctrl = ctrl
+        self.path = path
+        self.expt = exposure_time
+        self.unblank_beam = unblank_beam
+        self.logger = log
+        self.camtype = ctrl.cam.name
+        self.stopEvent = stop_event
+        self.stopEvent_rasterScan = stop_event_experiment
+        self.flatfield = flatfield
+        self.stagepos_idx = 0
+
+        self.diff_defocus = diff_defocus
+        self.image_interval = image_interval
+        self.nom_ii = self.image_interval
+        self.robust_ii = 2
+        self.exposure_time_image = exposure_time_image
+
+        self.scan_area = scan_area
+        self.auto_zheight = zheight
+        self.mode = 0
+
+        self.diff_brightness = self.ctrl.brightness.value
+        # self.autocenterDP = autocenterDP
+        self.angle_activation = angle_activation
+        self.spread = spread
+        self.offset = offset
+        self.rotrangelimit = rotrange
+        self.backlash_killer = backlash_killer
+        self.rotation_speed = rotation_speed
+
+        self.calibdir = self.path.parent / 'calib'
+
+        self.verbose = False
+        self.number_crystals_scanned = 0
+        self.number_exp_performed = 0
+
+        if not os.path.exists(self.calibdir):
+            os.makedirs(self.calibdir)
+
+        self.image_interval_enabled = enable_image_interval
+        if enable_image_interval:
+            self.image_interval = image_interval
+            msg = f'Image interval enabled: every {self.image_interval} frames an image with defocus {self.diff_defocus} will be displayed (t={self.exposure_time_image} s).'
+            if self.verbose:
+                print(msg)
+            self.logger.info(msg)
+        else:
+            self.image_interval = 99999
+
+        self.enable_autotrack = enable_autotrack
+        self.enable_fullacred = enable_fullacred
+        self.enable_fullacred_crystalfinder = enable_fullacred_crystalfinder
+
+        if enable_fullacred_crystalfinder:
+            self.diff_defocus = diff_defocus
+            self.image_interval = image_interval
+            msg = f'Full autocRED feature with auto crystal finder enabled: every {image_interval} frames an image with defocus value {diff_defocus} will be displayed.'
+            self.mode = 3
+
+        elif enable_fullacred:
+            self.diff_defocus = diff_defocus
+            self.image_interval = image_interval
+            msg = f'Full autocRED feature enabled: every {image_interval} frames an image with defocus value {diff_defocus} will be displayed.'
+            self.mode = 2
+
+        elif enable_autotrack:
+            self.diff_defocus = diff_defocus
+            self.image_interval = image_interval
+            msg = f'Image autotrack enabled: every {image_interval} frames an image with defocus value {diff_defocus} will be displayed.'
+            self.mode = 1
+
+        if self.verbose:
+            print(msg)
+
+        if use_dials:
+            self.s = socket.socket()
+            dials_host = config.settings.indexing_server_host
+            dials_port = config.settings.indexing_server_port
+            try:
+                self.s.connect((dials_host, dials_port))
+                print('DIALS server connected for autocRED.')
+                self.s_c = 1
+            except BaseException:
+                print('Is DIALS server running? Connection failed.')
+                self.s_c = 0
+
+        if use_vm:
+            self.s2 = socket.socket()
+            vm_host = config.settings.VM_server_host
+            vm_port = config.settings.VM_server_port
+            try:
+                self.s2.connect((vm_host, vm_port))
+                print('VirtualBox server connected for autocRED.')
+                self.s2_c = 1
+            except BaseException:
+                print('Is VM server running? Connection failed.')
+                self.s2_c = 0
+
+    def image_cropper(self, img, window_size=0):
+        crystal_pos, r = find_defocused_image_center(img)  # find_defocused_image_center crystal position (y,x)
+        crystal_pos = crystal_pos[::-1]
+
+        if window_size == 0:
+
+            if r[0] <= r[1]:
+                window_size = r[0] * 2
+            else:
+                window_size = r[1] * 2
+
+            window_size = int(window_size / 1.414)
+            if window_size % 2 == 1:
+                window_size = window_size + 1
+
+        a1 = int(crystal_pos[0] - window_size / 2)
+        b1 = int(crystal_pos[0] + window_size / 2)
+        a2 = int(crystal_pos[1] - window_size / 2)
+        b2 = int(crystal_pos[1] + window_size / 2)
+
+        img_cropped = img[a1:b1, a2:b2]
+        return crystal_pos, img_cropped, window_size
+
+    def hysteresis_check(self, n_cycle=4):
+        print('Relaxing beam...')
+        modes = ['mag1', 'samag', 'diff']
+        current_mode = self.ctrl.mode.get()
+        mode_index = modes.index(current_mode)
+
+        for i in range(n_cycle):
+            self.ctrl.mode.set(modes[(mode_index + 1) % 3])
+            time.sleep(0.5)
+            self.ctrl.mode.set(modes[(mode_index + 2) % 3])
+            time.sleep(0.5)
+            self.ctrl.mode.set(modes[mode_index])
+            time.sleep(0.5)
+
+        print('Beam relaxing done.')
+
+    def check_lens_close_to_limit_warning(self, lensname, lensvalue, MAX=65535, threshold=5000):
+        warn = 0
+        if MAX - lensvalue < threshold or lensvalue < threshold:
+            warn = 1
+            if self.verbose:
+                print(f'Warning: {lensname} close to limit!')
+        return warn
+
+    def img_var(self, img, apert_pos):
+        apert_pos = [int(apert_pos[0]), int(apert_pos[1])]
+        window_size = img.shape[0]
+        half_w = int(window_size / 2)
+        x_range = range(apert_pos[0] - half_w, apert_pos[0] + half_w)
+        y_range = range(apert_pos[1] - half_w, apert_pos[1] + half_w)
+
+        if not any(x in range(255, 261) for x in x_range) and not any(y in range(255, 261) for y in y_range):
+            return np.var(img)
+        else:
+            if any(x in range(255, 261) for x in x_range):
+                indx = []
+                for px in range(255, 261):
+                    try:
+                        indx.append(x_range.index(px))
+                    except BaseException:
+                        pass
+
+                img = np.delete(img, indx, 0)
+
+            if any(y in range(255, 261) for y in y_range):
+                indy = []
+                for px in range(255, 261):
+                    try:
+                        indy.append(y_range.index(px))
+                    except BaseException:
+                        pass
+
+                img = np.delete(img, indy, 1)
+
+            return np.var(img)
+
+    def check_img_outsidebeam_byscale(self, img1_scale, img2_scale):
+        """img1 is the original image for reference, img2 is the new image."""
+        if img2_scale / img1_scale < 0.5 or img2_scale / img1_scale > 2:
+            return 1
+        else:
+            return 0
+
+    def eliminate_backlash_in_tiltx(self):
+        a_i = self.ctrl.stage.a
+        if a_i < 0:
+            self.ctrl.stage.set(a=a_i + self.backlash_killer, wait=True)
+            # print("Rotation positive!")
+            return 0
+        else:
+            self.ctrl.stage.set(a=a_i - self.backlash_killer, wait=True)
+            # print("Rotation negative!")
+            return 1
+
+    def center_particle_ofinterest(self, pos_arr, transform_stagepos):
+        """Used to center the particle of interest in the view to minimize
+        usage of lens."""
+        transform_stagepos_ = np.linalg.inv(transform_stagepos)
+        if pos_arr[0] < 200 or pos_arr[0] > 316 or pos_arr[1] < 200 or pos_arr[1] > 316:
+
+            _x0 = self.ctrl.stage.x
+            _y0 = self.ctrl.stage.y
+
+            displacement = np.subtract((258, 258), pos_arr)
+            mag = self.ctrl.magnification.value
+
+            s = config.calibration['mag1']['pixelsize'][mag] / 1000  # nm -> um
+            # print("scaling facor: {} um per px".format(s))
+
+            mvmt = s * displacement
+            mvmt_x, mvmt_y = np.dot(1000 * mvmt, transform_stagepos_)
+
+            self.ctrl.stage.set(x=_x0 + mvmt_y, y=_y0 - mvmt_x)
+
+        else:
+            pass
+
+    def center_particle_from_crystalList(self, crystal_positions, transform_stagepos, magnification, beamsize):
+        n_crystals = len(crystal_positions)
+        if n_crystals == 0:
+            self.print_and_del('No crystal found on image!')
+            return (0, 0)
+
+        else:
+            beam_area = beamsize ** 2
+
+            for crystal in crystal_positions:
+                if crystal.isolated:
+                    self.center_particle_ofinterest((crystal.x, crystal.y), transform_stagepos)
+                    crystalsize = crystal.area_pixel
+                    # print("crystal size: {}".format(crystalsize))
+                    img, h = self.ctrl.get_image(exposure=self.expt, header_keys=None)
+
+                    crystal_positions_new = find_crystals_timepix(img, magnification=self.magnification, spread=self.spread, offset=self.offset)
+
+                    n_crystals_new = len(crystal_positions_new)
+                    # print(crystal_positions_new)
+                    if n_crystals_new == 0:
+                        self.print_and_del('No crystal found after centering...')
+                        return (0, 0)
+
+                    else:
+                        # print("Start looping.")
+                        for crystal in crystal_positions_new:
+                            if crystal.isolated and crystalsize * 0.9 <= crystal.area_pixel <= crystalsize * 1.1:
+                                self.print_and_del(f'Crystal that has been centered is found at {crystal.x}, {crystal.y}.')
+                                beamshift_coords = self.calib_beamshift.pixelcoord_to_beamshift((crystal.x, crystal.y))
+
+                                return (beamshift_coords, crystalsize)
+                            else:
+                                return (0, 0)
+
+                else:
+                    return (0, 0)
+
+    def isolated(self, c, crystalpositions, thresh=100):
+        distances = []
+        if len(crystalpositions) == 1:
+            return True
+        else:
+            for allcryst in crystalpositions:
+                distvec = np.subtract(allcryst, (c.x, c.y))
+                dist = np.linalg.norm(distvec)
+                if dist != 0:
+                    distances.append(dist)
+
+            if min(distances) > thresh:  # in pixels
+                return True
+            else:
+                return False
+
+    def find_crystal_center(self, img_c, window_size, gauss_window=4):
+        mn = np.min(img_c)
+        mx = np.max(img_c)
+
+        sel = (img_c > l + 0.1 * (mx - mn)) & (img_c < mx - 0.4 * (h - mn))
+        blurred = ndimage.filters.gaussian_filter(sel.astype(float), gauss_window)
+        x, y = np.unravel_index(np.argmax(blurred, axis=None), blurred.shape)
+        return (y, x)
+
+    def find_crystal_center_fromhist(self, img, bins=20, plot=False, gauss_window=5):
+        h, b = np.histogram(img, bins)
+        sel = (img > b[1]) & (img < b[8])
+
+        blurred = ndimage.filters.gaussian_filter(sel.astype(float), gauss_window)
+        x, y = np.unravel_index(np.argmax(blurred, axis=None), blurred.shape)
+        if plot:
+            plt.imshow(sel)
+            plt.scatter(y, x)
+            plt.show()
+        return (y, x)
+
+    def tracking_by_particlerecog(self, img, magnification=2500, spread=6, offset=18):
+        crystal_pos, r = find_defocused_image_center(img)  # find_defocused_image_center crystal position (y,x)
+        crystal_pos = crystal_pos[::-1]
+
+        window_size = 0
+
+        if window_size == 0:
+
+            if r[0] <= r[1]:
+                window_size = r[0] * 2
+            else:
+                window_size = r[1] * 2
+
+            # window_size = int(window_size/1.414)
+            if window_size % 2 == 1:
+                window_size = window_size + 1
+
+        a1 = int(crystal_pos[0] - window_size / 2)
+        b1 = int(crystal_pos[0] + window_size / 2)
+        a2 = int(crystal_pos[1] - window_size / 2)
+        b2 = int(crystal_pos[1] + window_size / 2)
+
+        img_cropped = img[a1:b1, a2:b2]
+
+        # crystalpositions = find_crystals_timepix(img_cropped, magnification = magnification, spread=spread, offset = offset)
+        # crystalposition = self.find_crystal_center(img_cropped, window_size)
+        crystalposition = self.find_crystal_center_fromhist(img_cropped)
+        center = (window_size / 2, window_size / 2)
+
+        # if len(crystalpositions) == 1:
+        # crystalxy = (crystalpositions[0].x, crystalpositions[0].y)
+        shift = np.subtract(center, crystalposition)
+        # elif len(crystalpositions) > 1:
+        #    areas = [crystal.area_pixel for crystal in crystalpositions]
+        #    idx = areas.index(max(areas))
+        #    crystalxy = (crystalpositions[idx].x, crystalpositions[idx].y)
+        #    shift = np.subtract(center, crystalxy)
+        # else:
+        #    print("Crystal lost.")
+        #    shift = np.array((512, 512))
+
+        return tuple(shift[::-1])
+
+    def setandupdate_bs(self, bs_x0, bs_y0, delta_beamshiftcoord1):
+        self.ctrl.beamshift.set(bs_x0 + delta_beamshiftcoord1[0], bs_y0 + delta_beamshiftcoord1[1])
+        bs_x0 = bs_x0 + delta_beamshiftcoord1[0]
+        bs_y0 = bs_y0 + delta_beamshiftcoord1[1]
+        return bs_x0, bs_y0
+
+    def defocus_and_image(self, difffocus, exp_t):
+        diff_focus_proper = self.ctrl.difffocus.value
+        diff_focus_defocused = diff_focus_proper + difffocus
+        self.ctrl.difffocus.value = diff_focus_defocused
+
+        img0, h = self.ctrl.get_image(exp_t, header_keys=None)
+        self.ctrl.difffocus.value = diff_focus_proper
+        return img0, h
+
+    def print_and_log(self, logger, msg):
+        print(msg)
+        logger.debug(msg)
+
+    def print_and_del(self, msg):
+        print('\033[k', msg, end='\r')
+
+    def imagevar_blank_estimator(self, brightness, cycle=3):
+        # previous_mode = self.ctrl.mode.get()
+        self.ctrl.mode.set('mag1')
+        self.ctrl.brightness.value = brightness
+
+        input('Please move your stage to a blank area for image variance calculation. Do not change brightness. Press ENTER when ready.')
+        img_var_est = []
+        beamsize_est = []
+        for i in range(0, cycle):
+            img, h = self.ctrl.get_image(self.exposure_time_image, header_keys=None)
+            crystal_pos, img0_cropped, window_size = self.image_cropper(img=img, window_size=0)
+            v = self.img_var(img0_cropped, crystal_pos)
+            print(f'blank image variance: {v}')
+            img_var_est.append(v)
+            beamsize_est.append(window_size)
+
+        image_var = np.average(img_var_est)
+        beamsize_avg = np.average(window_size)
+
+        self.ctrl.mode.set('samag')
+        self.ctrl.mode.set('diff')
+        return image_var, beamsize_avg
+
+    def auto_cred_collection(self, path, pathtiff, pathsmv, pathred, transform_imgshift, transform_imgshift2, transform_imgshift_foc, transform_imgshift2_foc, transform_beamshift_d, transform_beamshift_d_defoc, calib_beamshift):
+        """track method
+        p: particle recognition
+        c: cross correlation"""
+
+        trackmethod = 'p'
+
+        for paths in (path, pathtiff, pathsmv, pathred):
+            if not os.path.exists(paths):
+                os.makedirs(paths)
+
+        a = a0 = self.ctrl.stage.a
+        spotsize = self.ctrl.spotsize
+
+        if self.mode == 1:
+            self.logger.info('AutocRED experiment starting...')
+        elif self.mode == 2:
+            self.logger.info('Full AutocRED experiment starting...')
+        elif self.mode == 3:
+            self.logger.info('Full AutocRED with auto crystal finder experiment starting...')
+        self.logger.info('Data recording started at: {}'.format(datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')))
+        self.logger.info(f'Data saving path: {path}')
+        self.logger.info(f'Data collection exposure time: {self.expt} s')
+        self.logger.info(f'Data collection spot size: {spotsize}')
+        # TODO: Mostly above is setup, split off into own function
+
+        buffer = []
+        image_buffer = []
+
+        if self.mode > 0:
+
+            if self.verbose:
+                print('Auto tracking feature activated. Please remember to bring sample to proper Z height in order for autotracking to be effective.')
+
+            transform_imgshift_ = np.linalg.inv(transform_imgshift)
+            transform_imgshift2_ = np.linalg.inv(transform_imgshift2)
+            transform_imgshift_foc_ = np.linalg.inv(transform_imgshift_foc)
+            transform_imgshift2_foc_ = np.linalg.inv(transform_imgshift2_foc)
+
+            transform_beamshift_d_ = np.linalg.inv(transform_beamshift_d)
+
+            self.logger.debug(f'Transform_imgshift: {transform_imgshift}')
+            self.logger.debug(f'Transform_imgshift_foc: {transform_imgshift_foc}')
+            self.logger.debug(f'Transform_imgshift2: {transform_imgshift2}')
+            self.logger.debug(f'Transform_imgshift2_foc: {transform_imgshift2_foc}')
+
+            if self.ctrl.mode != 'diff':
+                self.ctrl.mode.set('samag')
+                self.ctrl.mode.set('diff')
+
+            bs_x0, bs_y0 = self.ctrl.beamshift.get()
+            is_x0, is_y0 = self.ctrl.imageshift1.get()
+            ds_x0, ds_y0 = self.ctrl.diffshift.get()
+            is2_x0, is2_y0 = self.ctrl.imageshift2.get()
+
+            is1_init = (is_x0, is_y0)
+            is2_init = (is2_x0, is2_y0)
+
+            self.logger.debug(f'Initial Beamshift: {bs_x0}, {bs_y0}')
+            self.logger.debug(f'Initial Imageshift1: {is_x0}, {is_y0}')
+            self.logger.debug(f'Initial Imageshift2: {is2_x0}, {is2_y0}')
+
+            diff_focus_proper = self.ctrl.difffocus.value
+            diff_focus_defocused = diff_focus_proper + self.diff_defocus
+
+            img0, h = self.defocus_and_image(difffocus=self.diff_defocus, exp_t=self.exposure_time_image)
+
+            """if trackmethod == "p":
+                shift = self.tracking_by_particlerecog(img0)
+                delta_beamshiftcoord = np.matmul(self.calib_beamshift.transform, shift)
+                self.logger.debug("Beam shift coordinates: {}".format(delta_beamshiftcoord))
+
+                bs_x0, bs_y0 = self.setandupdate_bs(bs_x0, bs_y0, delta_beamshiftcoord)
+
+                img0, h = self.defocus_and_image(difffocus = self.diff_defocus, exp_t = self.exposure_time_image)"""
+
+            img0_p = preprocess(img0.astype(float))
+            scorefromCNN = predict(img0_p)
+            # self.print_and_log(logger = self.logger, msg = "Score for the DP: {}".format(scorefromCNN))
+            self.logger.debug(f'Score for the DP: {scorefromCNN}')
+
+            crystal_pos, img0_cropped, window_size = self.image_cropper(img=img0, window_size=0)
+            img0var = self.img_var(img0_cropped, crystal_pos)
+            appos0 = crystal_pos
+
+            self.logger.debug(f'Tracking method: {trackmethod}. Initial crystal_pos: {crystal_pos} by find_defocused_image_center.')
+
+        if self.unblank_beam:
+            self.ctrl.beam.unblank()
+
+        if self.mode > 1:
+            a_i = self.ctrl.stage.a
+
+            rotation_range = self.rotrangelimit + abs(a_i)
+            rotation_t = rotation_range / self.rotation_speed
+
+            try:
+                if self.rotation_direction == 0:
+                    self.ctrl.stage.set(a=a_i + rotation_range, wait=False)
+                else:
+                    self.ctrl.stage.set(a=a_i - rotation_range, wait=False)
+            except BaseException:
+                if a_i < 0:
+                    self.ctrl.stage.set(a=a_i + rotation_range, wait=False)
+                else:
+                    self.ctrl.stage.set(a=a_i - rotation_range, wait=False)
+
+        if self.camtype == 'simulate':
+            self.startangle = a
+        else:
+            time.sleep(self.angle_activation)
+
+        i = 1
+
+        numb_robustTrack = 0
+        """Turn on and off for crystal movement guess here."""
+        self.guess_crystmove = False
+
+        """set acquisition time to be around 0.52 s in order to fix the image interval times."""
+        acquisition_time = self.expt + 0.02
+
+        self.ctrl.cam.block()
+        """To ensure lock got released in the block step."""
+        time.sleep(0.1)
+
+        t0 = time.perf_counter()
+        self.startangle = a
+
+        self.stopEvent.clear()
+
+        while not self.stopEvent.is_set():
+            try:
+                if i < self.nom_ii:
+                    self.image_interval = self.robust_ii
+                    numb_robustTrack += 1
+                else:
+                    self.image_interval = self.nom_ii
+
+                    """If variance changed over 20%, do a robust check to ensure crystal is back"""
+
+                    if imgvar / img0var < 0.5 or imgvar / img0var > 2 or imgscale / imgscale0 > 1.15 or imgscale / imgscale0 < 0.85:
+                        self.image_interval = self.robust_ii
+                        numb_robustTrack += 1
+                    else:
+                        self.image_interval = self.nom_ii
+                        numb_robustTrack = 0
+
+                if numb_robustTrack > 10:
+                    self.image_interval = self.nom_ii
+                    img0var = imgvar
+                    imgscale0 = imgscale
+                    numb_robustTrack = 0
+
+                if i % self.image_interval == 0:  # aim to make this more dynamically adapted...
+                    t_start = time.perf_counter()
+
+                    """Guessing the next particle position by simply apply the same beamshift change as previous"""
+                    if self.guess_crystmove and i >= self.nom_ii:
+                        bs_x0, bs_y0 = self.setandupdate_bs(bs_x0, bs_y0, delta_beamshiftcoord)
+
+                    self.ctrl.difffocus.value = diff_focus_defocused
+                    img, h = self.ctrl.get_image(self.exposure_time_image, header_keys=None)
+                    self.ctrl.difffocus.value = diff_focus_proper
+
+                    image_buffer.append((i, img, h))
+
+                    crystal_pos, img_cropped, _ = self.image_cropper(img=img, window_size=window_size)
+
+                    self.logger.debug(f'crystal_pos: {crystal_pos} by find_defocused_image_center.')
+
+                    imgvar = self.img_var(img_cropped, crystal_pos)
+
+                    self.logger.debug(f'Image variance: {imgvar}')
+
+                    """If variance changed over 50%, then the crystal is outside the beam and stop data collection"""
+                    if imgvar / img0var < 0.2 or imgvar / img0var > 5:
+                        self.print_and_del('Collection stopping because crystal out of the beam...')
+                        self.stopEvent.set()
+                    if imgvar < self.imgvar_threshold:
+                        self.print_and_del('Image variance smaller than blank image.')
+                        self.stopEvent.set()
+
+                    if trackmethod == 'c':
+
+                        cc, err, diffphase = phase_cross_correlation(img0_cropped, img_cropped)
+                        self.logger.debug(f'Cross correlation result: {cc}')
+
+                        if self.guess_crystmove and i >= self.nom_ii:
+                            delta_beamshiftcoord1 = np.matmul(self.calib_beamshift.transform, cc)
+                            # print("Beam shift coordinates: {}".format(delta_beamshiftcoord))
+                            self.logger.debug(f'Beam shift coordinates: {delta_beamshiftcoord1}')
+                            bs_x0, bs_y0 = self.setandupdate_bs(bs_x0, bs_y0, delta_beamshiftcoord1)
+
+                            delta_beamshiftcoord = delta_beamshiftcoord1 + delta_beamshiftcoord
+
+                        else:
+                            delta_beamshiftcoord = np.matmul(self.calib_beamshift.transform, cc)
+                            # print("Beam shift coordinates: {}".format(delta_beamshiftcoord))
+                            self.logger.debug(f'Beam shift coordinates: {delta_beamshiftcoord}')
+                            bs_x0, bs_y0 = self.setandupdate_bs(bs_x0, bs_y0, delta_beamshiftcoord)
+
+                    elif trackmethod == 'p':
+
+                        shift = self.tracking_by_particlerecog(img)
+                        delta_beamshiftcoord = np.matmul(shift, transform_beamshift_d_defoc)
+                        self.logger.debug(f'Beam shift coordinates: {delta_beamshiftcoord}')
+
+                        bs_x0, bs_y0 = self.setandupdate_bs(bs_x0, bs_y0, delta_beamshiftcoord)
+
+                        if shift[0] == 512:
+                            self.stopEvent.set()
+                            continue
+
+                    if self.check_lens_close_to_limit_warning(lensname='beamshift', lensvalue=bs_x0) or self.check_lens_close_to_limit_warning(lensname='beamshift', lensvalue=bs_y0):
+                        self.logger.debug(f'Beamshift close to limit warning: bs_x0 = {bs_x0}, bs_y0 = {bs_y0}')
+                        self.stopEvent.set()
+
+                    crystal_pos, r = find_defocused_image_center(img)
+                    crystal_pos = crystal_pos[::-1]
+                    crystal_pos_dif = crystal_pos - appos0
+                    apmv = -crystal_pos_dif
+                    dpmv = delta_beamshiftcoord @ transform_beamshift_d_
+                    R = -transform_imgshift2_foc_ @ transform_imgshift_foc @ transform_imgshift_ + transform_imgshift2_
+                    mv = apmv - dpmv @ transform_imgshift_foc @ transform_imgshift_
+                    delta_imageshift2coord = np.matmul(mv, np.linalg.inv(R))
+                    delta_imageshiftcoord = dpmv @ transform_imgshift_foc - delta_imageshift2coord @ transform_imgshift2_foc_ @ transform_imgshift_foc
+
+                    diff_shift = delta_imageshiftcoord @ transform_imgshift_foc_ + delta_imageshift2coord @ transform_imgshift2_foc_
+                    img_shift = delta_imageshiftcoord @ transform_imgshift_ + delta_imageshift2coord @ transform_imgshift2_
+
+                    self.logger.debug(f'delta imageshiftcoord: {delta_imageshiftcoord}, delta imageshift2coord: {delta_imageshift2coord}')
+
+                    self.ctrl.imageshift1.set(x=is_x0 - int(delta_imageshiftcoord[0]), y=is_y0 - int(delta_imageshiftcoord[1]))
+                    self.ctrl.imageshift2.set(x=is2_x0 - int(delta_imageshift2coord[0]), y=is2_y0 - int(delta_imageshift2coord[1]))
+
+                    is_x0 = is_x0 - int(delta_imageshiftcoord[0])
+                    is_y0 = is_y0 - int(delta_imageshiftcoord[1])
+                    is2_x0 = is2_x0 - int(delta_imageshift2coord[0])
+                    is2_y0 = is2_y0 - int(delta_imageshift2coord[1])
+
+                    if self.check_lens_close_to_limit_warning(lensname='imageshift1', lensvalue=is_x0) or self.check_lens_close_to_limit_warning(lensname='imageshift1', lensvalue=is_y0) or self.check_lens_close_to_limit_warning(lensname='imageshift2', lensvalue=is2_x0) or self.check_lens_close_to_limit_warning(lensname='imageshift2', lensvalue=is2_y0):
+                        self.logger.debug(f'Imageshift close to limit warning: is_x0 = {is_x0}, is_y0 = {is_y0}, is2_x0 = {is2_x0}, is2_y0 = {is2_y0}')
+                        self.stopEvent.set()
+
+                    self.logger.debug(f'Image Interval: {self.image_interval}, Imgvar/Img0var:{imgvar / img0var}')
+
+                    next_interval = t_start + acquisition_time
+
+                    while time.perf_counter() > next_interval:
+                        self.logger.debug('Skipping one image.')
+                        next_interval += acquisition_time
+                        i += 1
+
+                    diff = next_interval - time.perf_counter()
+                    time.sleep(diff)
+
+                else:
+                    t_start = time.perf_counter()
+                    img, h = self.ctrl.get_image(self.expt, header_keys=None)
+                    if buffer == []:
+                        imgscale0 = np.sum(img)
+                    else:
+                        imgscale = np.sum(img)
+                        self.logger.debug(f'Image scale variation: {imgscale / imgscale0}')
+
+                    buffer.append((i, img, h))
+
+                    next_interval = t_start + acquisition_time
+
+                    while time.perf_counter() > next_interval:
+                        next_interval += acquisition_time
+                        self.logger.debug('One image skipped because of too long acquisition or calculation time.')
+                        i += 1
+
+                    diff = next_interval - time.perf_counter()
+                    time.sleep(diff)
+
+                i += 1
+
+                if time.perf_counter() - t0 >= rotation_t:
+                    self.stopEvent.set()
+                    self.print_and_del('Goniometer close to limit!')
+
+            except Exception as e:
+                self.print_and_del(e)
+                self.stopEvent.set()
+
+        t1 = time.perf_counter()
+
+        self.ctrl.cam.unblock()
+        if self.mode > 1:
+            self.ctrl.stage.stop()
+
+        if self.camtype == 'simulate':
+            self.endangle = self.startangle + np.random.random() * 50
+            camera_length = 300
+        else:
+            self.endangle = self.ctrl.stage.a
+            camera_length = int(self.ctrl.magnification.get())
+
+        if self.unblank_beam:
+            # print("Blanking beam")
+            self.ctrl.beam.blank()
+
+        self.stopEvent.clear()
+
+        self.ctrl.imageshift1.set(x=is1_init[0], y=is1_init[1])
+        self.ctrl.imageshift2.set(x=is2_init[0], y=is2_init[1])
+
+        # stage_positions = tracer.stop()
+        stageposx, stageposy, stageposz, stageposa, stageposb = self.ctrl.stage.get()
+        rotrange = abs(self.endangle - self.startangle)
+
+        if self.verbose:
+            print(f'Rotated {abs(self.endangle - self.startangle):.2f} degrees from {self.startangle:.2f} to {self.endangle:.2f}')
+
+        self.logger.info(f'Rotated {abs(self.endangle - self.startangle):.2f} degrees from {self.startangle:.2f} to {self.endangle:.2f}')
+
+        nframes = i - 1  # i + 1 is not correct since i+=1 was executed before next image is taken???
+        osangle = abs(self.endangle - self.startangle) / nframes
+        acquisition_time = (t1 - t0) / nframes
+
+        self.logger.info(f'Data collection camera length: {camera_length} mm')
+        self.logger.info(f'Data collected from {self.startangle} degree to {self.endangle} degree.')
+        self.logger.info(f'Oscillation angle: {osangle}')
+        self.logger.info('Pixel size and actual camera length updated in SMV file headers for DIALS processing.')
+
+        rotation_angle = config.camera.camera_rotation_vs_stage_xy
+
+        self.pixelsize = config.calibration['diff']['pixelsize'][camera_length]  # px / Angstrom
+        self.physical_pixelsize = config.camera.physical_pixelsize  # mm
+        self.wavelength = config.microscope.wavelength  # angstrom
+        self.stretch_azimuth = config.camera.stretch_azimuth
+        self.stretch_amplitude = config.camera.stretch_amplitude
+
+        now = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+
+        with open(os.path.join(path, 'cRED_log.txt'), 'w') as f:
+            print(f'Data Collection Time: {now}', file=f)
+            print(f'Starting angle: {self.startangle}', file=f)
+            print(f'Ending angle: {self.endangle}', file=f)
+            print(f'Exposure Time: {self.expt} s', file=f)
+            print(f'Spot Size: {spotsize}', file=f)
+            print(f'Camera length: {camera_length} mm\n', file=f)
+            print(f'Pixelsize: {self.pixelsize} px/Angstrom', file=f)
+            print(f'Physical pixelsize: {self.physical_pixelsize} um', file=f)
+            print(f'Wavelength: {self.wavelength} Angstrom', file=f)
+            print(f'Stretch amplitude: {self.stretch_azimuth} %', file=f)
+            print(f'Stretch azimuth: {self.stretch_amplitude} degrees', file=f)
+            print(f'Rotation axis: {rotation_angle} radians', file=f)
+            print(f'Oscillation angle: {osangle} degrees', file=f)
+            print(f'Number of frames: {len(buffer)}', file=f)
+            print(f'Particle found at stage position: x: {stageposx}, y: {stageposy}, z: {stageposz}', file=f)
+
+        with open(log_rotaterange, 'a') as f:
+            f.write(f'{stageposx}\t{stageposy}\t{stageposz}\t{rotrange}\n')
+
+        img_conv = ImgConversion(buffer=buffer,
+                                 osc_angle=osangle,
+                                 start_angle=self.startangle,
+                                 end_angle=self.endangle,
+                                 rotation_axis=rotation_angle,
+                                 acquisition_time=acquisition_time,
+                                 flatfield=self.flatfield,
+                                 pixelsize=self.pixelsize,
+                                 physical_pixelsize=self.physical_pixelsize,
+                                 wavelength=self.wavelength,
+                                 stretch_amplitude=self.stretch_amplitude,
+                                 stretch_azimuth=self.stretch_azimuth,
+                                 )
+
+        img_conv.tiff_writer(pathtiff)
+        img_conv.smv_writer(pathsmv)
+        img_conv.mrc_writer(pathred)
+        img_conv.write_ed3d(pathred)
+        img_conv.write_xds_inp(pathsmv)
+
+        img_conv.to_dials(pathsmv)
+        pathsmv_str = str(pathsmv)
+        msg = {'path': pathsmv_str,
+               'rotrange': rotrange,
+               'nframes': nframes,
+               'osc': osangle}
+        msg_tosend = json.dumps(msg).encode('utf8')
+
+        if self.s_c:
+            self.s.send(msg_tosend)
+            self.print_and_del('SMVs sent to DIALS for processing.')
+
+        if self.s2_c:
+            self.s2.send(msg_tosend)
+            self.print_and_del('SMVs sent to XDS for processing.')
+
+        # self.logger.info("XDS INP file created.")
+
+        if image_buffer:
+            drc = os.path.join(path, 'tiff_image')
+            os.makedirs(drc)
+            while len(image_buffer) != 0:
+                i, img, h = image_buffer.pop(0)
+                fn = os.path.join(drc, f'{i:05d}.tiff')
+                write_tiff(fn, img, header=h)
+
+        self.ctrl.beam.unblank()
+        self.number_exp_performed += 1
+        if self.verbose:
+            print('Data Collection and Conversion Done.')
+
+    def write_BrightnessStates(self, n_cycles=2):
+        print('Go to your desired magnification and camera length. Now recording lens states...')
+        self.ctrl.mode.set('mag1')
+        input('Please choose the desired magnification, partially converge the beam in MAG1 to around 1 um in diameter, and center it using beamshift. Press ENTER when ready')
+
+        for i in range(0, n_cycles):
+            self.hysteresis_check()
+            input('Please recenter the beam with beamshift. Press ENTER when ready')
+
+        desired_mag = self.ctrl.magnification.get()
+        img_brightness = self.ctrl.brightness.value
+        bs = self.ctrl.beamshift.get()
+
+        self.ctrl.mode.set('samag')
+        self.ctrl.mode.set('diff')
+        input('Please go to diffraction mode, choose desired camera length, focus the diffraction spots, and center it using PLA. Press ENTER when ready')
+        for i in range(0, n_cycles):
+            self.hysteresis_check()
+            input('Please recenter the diffraction spot using PLA. Press ENTER when ready')
+
+        desired_cl = self.ctrl.magnification.get()
+        dp_focus = self.ctrl.difffocus.value
+        is1status = self.ctrl.imageshift1.get()
+        is2status = self.ctrl.imageshift2.get()
+        plastatus = self.ctrl.diffshift.get()
+        with open(self.calibdir / 'beam_brightness.pkl', 'wb') as f:
+            pickle.dump([img_brightness, bs, dp_focus, is1status, is2status, plastatus, desired_mag, desired_cl], f)
+
+        print('Brightness recorded.')
+        return [img_brightness, bs, dp_focus, is1status, is2status, plastatus, desired_mag, desired_cl]
+
+    def update_referencepoint_bs(self, bs, br):
+        exposure = 0.01
+        binsize = 1
+        scale = 1
+        self.ctrl.beamshift.set(*bs)
+        self.ctrl.brightness.value = br
+
+        img_cent = self.ctrl.get_raw_image(exposure=exposure, binsize=binsize)
+
+        if np.mean(img_cent) > 10:
+
+            pixel_cent = np.array(find_beam_center(img_cent)) * binsize / scale
+
+            # print(pixel_cent)
+
+            self.calib_beamshift.reference_shift = bs
+            self.calib_beamshift.reference_pixel = pixel_cent
+
+            return self.calib_beamshift.reference_pixel
+        else:
+            return self.calib_beamshift.reference_pixel
+
+    def raster_scan(self):
+        from instamatic.experiments.serialed.experiment import get_offsets_in_scan_area
+        pixelsize_mag1 = config.calibration['mag1']['pixelsize'][self.magnification] / 1000  # nm -> um
+        xdim, ydim = self.ctrl.getCameraDimensions()
+        box_x, box_y = self.pixelsize_mag1 * xdim, self.pixelsize_mag1 * ydim
+
+        # Make negative to reflect config change 2019-07-03 to make omega more in line with other software
+        rot_axis = -config.camera.camera_rotation_vs_stage_xy
+
+        offsets = get_offsets_in_scan_area(box_x, box_y, self.scan_area, angle=rot_axis)
+        self.offsets = offsets * 1000
+
+        center_x = self.ctrl.stage.x
+        center_y = self.ctrl.stage.y
+
+        x_zheight = 0
+        y_zheight = 0
+
+        t = tqdm(self.offsets, desc=f'Number of crystals scanned: {self.number_crystals_scanned}; Number of experiments performed: {self.number_exp_performed}')
+
+        for j, (x_offset, y_offset) in enumerate(t):
+            x = center_x + x_offset
+            y = center_y + y_offset
+
+            self.ctrl.stage.set(x=x, y=y)
+            # print("Stage position: x = {}, y = {}".format(x,y))
+            x_change = x - x_zheight
+            y_change = y - y_zheight
+            dist = np.linalg.norm((x_change, y_change))
+
+            if dist > 50000 or x_zheight * y_zheight == 0 or x_zheight == 999999:
+                try:
+                    img, h = self.ctrl.get_image(exposure=self.expt, header_keys=None)
+                    if img.mean() > 10:
+                        self.magnification = self.ctrl.magnification.value
+                        crystal_positions = find_crystals_timepix(img, self.magnification, spread=self.spread, offset=self.offset)
+                        crystal_coords = [(crystal.x, crystal.y) for crystal in crystal_positions]
+
+                        n_crystals = len(crystal_coords)
+                        if n_crystals > 0:
+                            self.print_and_del('centering z height...')
+                            x_zheight, y_zheight = center_z_height_HYMethod(self.ctrl, spread=self.spread, offset=self.offset)
+                            if x_zheight != 999999:
+                                xpoint, ypoint, zpoint, aaa, bbb = self.ctrl.stage.get()
+                                self.logger.info(f'Stage position: x = {xpoint}, y = {ypoint}. Z height adjusted to {zpoint}. Tilt angle x {aaa} deg, Tilt angle y {bbb} deg')
+                            else:
+                                self.print_and_del('Z height not found.')
+                except BaseException:
+                    self.print_and_del('Something went wrong, unable to adjust height')
+                    pass
+
+            self.start_collection_point()
+
+            t.set_description(f'Number of crystals scanned: {self.number_crystals_scanned}; Number of experiments performed: {self.number_exp_performed}')
+
+            if self.stopEvent_rasterScan.is_set():
+                print('\nRaster Scan stopped manually.')
+                break
+
+    def start_collection_point(self):
+        IS1_Neut = self.ctrl.imageshift1.get()
+        IS2_Neut = self.ctrl.imageshift2.get()
+
+        path = self.path
+
+        if self.scan_area != 0:
+            path = path / f'stagepos_{self.stagepos_idx:04d}'
+            self.stagepos_idx += 1
+            if not os.path.exists(path):
+                os.makedirs(path)
+
+        try:
+            with open(self.calibdir / 'beam_brightness.pkl', 'rb') as f:
+                [img_brightness, bs, dp_focus, is1status, is2status, plastatus, desired_mag, desired_cl] = pickle.load(f)
+        except OSError:
+            [img_brightness, bs, dp_focus, is1status, is2status, plastatus, desired_mag, desired_cl] = self.write_BrightnessStates()
+
+        try:
+            self.calib_beamshift = CalibBeamShift.from_file(fn=self.calibdir / CALIB_BEAMSHIFT)
+            self.ctrl.beamshift.set(x=self.calib_beamshift.reference_shift[0], y=self.calib_beamshift.reference_shift[1])
+
+        except OSError:
+            print('No beam shift calibration result found. Running instamatic.calibrate_beamshift first...\n')
+            print('Going to MAG1, desired magnification, and desired brightness. DO NOT change brightness!')
+            if self.ctrl.mode != 'mag1':
+                self.ctrl.mode.set('mag1')
+                self.ctrl.magnification.value = desired_mag
+                self.ctrl.brightness.value = img_brightness
+
+            calib_file = 'x'
+            while calib_file == 'x':
+                print('Find a clear area, toggle the beam to the desired defocus value.')
+                self.calib_beamshift = calibrate_beamshift(ctrl=self.ctrl, outdir=self.calibdir)
+                print('Beam shift calibration done.')
+                calib_file = input('Press ENTER when ready to continue. Press x to REDO the calibration.')
+
+        self.logger.debug(f'Transform_beamshift: {self.calib_beamshift.transform}')
+
+        try:
+            self.calib_directbeam = CalibDirectBeam.from_file(fn=self.calibdir / CALIB_DIRECTBEAM)
+            with open(self.calibdir / 'diff_par.pkl', 'rb') as f:
+                self.diff_brightness, self.diff_difffocus = pickle.load(f)
+        except OSError:
+            if not self.ctrl.mode == 'diff':
+                self.ctrl.mode.set('samag')
+                self.ctrl.imageshift1.set(x=is1status[0], y=is1status[1])
+                self.ctrl.imageshift2.set(x=is2status[0], y=is2status[1])
+                self.ctrl.mode.set('diff')
+            self.ctrl.difffocus.value = dp_focus
+
+            self.calib_directbeam = CalibDirectBeam.live(self.ctrl, outdir=self.calibdir)
+            self.diff_brightness = self.ctrl.brightness.value
+            self.diff_difffocus = self.ctrl.difffocus.value
+            with open(self.calibdir / 'diff_par.pkl', 'wb') as f:
+                pickle.dump([self.diff_brightness, self.diff_difffocus], f)
+
+        try:
+            with open(self.calibdir / 'imgvariance.pkl', 'rb') as f:
+                self.imgvar_threshold, self.beam_size_avg = pickle.load(f)
+        except OSError:
+            self.imgvar_threshold, self.beam_size_avg = self.imagevar_blank_estimator(brightness=img_brightness)
+            with open(self.calibdir / 'imgvariance.pkl', 'wb') as f:
+                pickle.dump([self.imgvar_threshold, self.beam_size_avg], f)
+
+        self.neutral_beamshift = bs
+        # print("Neutral beamshift: from beam_brightness.pkl {}".format(bs))
+        self.neutral_diffshift = plastatus
+
+        self.calib_beamshift.reference_pixel = self.update_referencepoint_bs(bs, img_brightness)
+
+        # print("Calib_beamshift_referenceshift: {}".format(self.calib_beamshift.reference_shift))
+
+        transform_imgshift, c = load_IS_Calibrations(imageshift='IS1', ctrl=self.ctrl, diff_defocus=self.diff_defocus, logger=self.logger, mode='diff')
+        transform_imgshift2, c = load_IS_Calibrations(imageshift='IS2', ctrl=self.ctrl, diff_defocus=self.diff_defocus, logger=self.logger, mode='diff')
+        transform_imgshift_foc, c = load_IS_Calibrations(imageshift='IS1', ctrl=self.ctrl, diff_defocus=0, logger=self.logger, mode='diff')
+        transform_imgshift2_foc, c = load_IS_Calibrations(imageshift='IS2', ctrl=self.ctrl, diff_defocus=0, logger=self.logger, mode='diff')
+
+        transform_beamshift_d, c = load_IS_Calibrations(imageshift='BS', ctrl=self.ctrl, diff_defocus=0, logger=self.logger, mode='diff')
+        transform_beamshift_d_defoc, c = load_IS_Calibrations(imageshift='BS', ctrl=self.ctrl, diff_defocus=self.diff_defocus, logger=self.logger, mode='diff')
+        # transform_beamshift_d = self.calib_beamshift.transform
+
+        transform_stagepos, c = load_IS_Calibrations(imageshift='S', ctrl=self.ctrl, diff_defocus=0, logger=self.logger, mode='mag1')
+
+        if self.mode == 3:
+            # ready = input("Please make sure that you are in the super user mode and the rotation speed is set via GONIOTOOL! Press ENTER to continue.")
+
+            if self.ctrl.mode != 'mag1':
+                self.ctrl.mode.set('mag1')
+
+            self.ctrl.magnification.value = desired_mag
+            self.ctrl.brightness.value = 65535
+
+            header_keys = None
+
+            if self.verbose:
+                print(f'Beamshift reference: {self.calib_beamshift.reference_shift}')
+
+            self.ctrl.beamshift.set(x=self.calib_beamshift.reference_shift[0], y=self.calib_beamshift.reference_shift[1])
+
+            self.magnification = self.ctrl.magnification.value
+
+            self.rotation_direction = self.eliminate_backlash_in_tiltx()
+            img, h = self.ctrl.get_image(exposure=self.expt, header_keys=header_keys)
+            # img, h = Experiment.apply_corrections(img, h)
+
+            threshold = 10  # ignore black images
+
+            if img.mean() > threshold:
+
+                h['exp_magnification'] = self.ctrl.magnification.get()
+
+                write_tiff(path / 'Overall_view', img, h)
+
+                crystal_positions = find_crystals_timepix(img, self.magnification, spread=self.spread, offset=self.offset)
+                crystal_coords = [(crystal.x, crystal.y) for crystal in crystal_positions]
+
+                n_crystals = len(crystal_coords)
+
+                if n_crystals == 0:
+                    self.print_and_del('No crystals found in the image. Find another area!')
+                    return 0
+
+                (beamshiftcoord_0, size_crystal_targeted) = self.center_particle_from_crystalList(crystal_positions, transform_stagepos, self.magnification, self.beam_size_avg)
+
+                img, h = self.ctrl.get_image(exposure=self.expt, header_keys=header_keys)
+                h['exp_magnification'] = self.ctrl.magnification.get()
+                write_tiff(path / 'Overall_view', img, h)
+
+                crystal_positions = find_crystals_timepix(img, self.magnification, spread=self.spread, offset=self.offset)
+                crystal_coords = [(crystal.x, crystal.y) for crystal in crystal_positions]
+                crystal_sizes = [crystal.area_pixel for crystal in crystal_positions]
+                n_crystals = len(crystal_coords)
+
+                if n_crystals == 0:
+                    self.print_and_del('No crystals found in the image. Find another area!')
+                    return 0
+
+                if size_crystal_targeted != 0:
+                    try:
+                        ind_target = crystal_sizes.index(size_crystal_targeted)
+                        crystal_coords[0], crystal_coords[ind_target] = crystal_coords[ind_target], crystal_coords[0]
+                        self.print_and_del('Targeted isolated crystal centered is swapped to the first of the list.')
+                    except ValueError:
+                        self.print_and_del('Lost targeted isolated crystal.')
+                        return 0
+
+                self.logger.info(f'{datetime.datetime.now()} {n_crystals} crystals found.')
+
+                k = 0
+
+                while not self.stopEvent_rasterScan.is_set():
+
+                    try:
+                        self.ctrl.brightness.value = img_brightness
+
+                        if self.verbose:
+                            print(f'Collecting on crystal {k + 1}/{n_crystals}. Beamshift coordinates: {self.ctrl.beamshift.get()}')
+
+                        outfile = path / f'crystal_{k:04d}'
+                        comment = f'crystal {k}'
+
+                        beamshift_coords = np.array(bs) - np.dot(crystal_coords[k] - self.calib_beamshift.reference_pixel, self.calib_beamshift.transform)
+                        self.ctrl.beamshift.set(*beamshift_coords.astype(int))
+
+                        img, h = self.ctrl.get_image(exposure=0.001, comment=comment, header_keys=header_keys)
+                        h['exp_magnification'] = self.ctrl.magnification.get()
+                        write_tiff(path / f'crystal_{k:04d}', img, h)
+
+                        self.number_crystals_scanned += 1
+
+                        if self.isolated(crystal_positions[k], crystal_coords) and crystal_positions[k].isolated and not any(t < 100 for t in crystal_coords[k]) and not any(t > 416 for t in crystal_coords[k]):
+
+                            self.ctrl.mode.set('samag')
+                            self.ctrl.mode.set('diff')
+                            self.ctrl.imageshift1.set(x=is1status[0], y=is1status[1])
+                            self.ctrl.imageshift2.set(x=is2status[0], y=is2status[1])
+                            self.ctrl.diffshift.set(x=plastatus[0], y=plastatus[1])
+
+                            # compensate beamshift
+                            beamshift_offset = beamshift_coords - self.neutral_beamshift
+                            pixelshift = self.calib_directbeam.beamshift2pixelshift(beamshift_offset)
+
+                            diffshift_offset = self.calib_directbeam.pixelshift2diffshift(pixelshift)
+                            diffshift = self.neutral_diffshift - diffshift_offset
+
+                            self.ctrl.diffshift.set(*diffshift.astype(int))
+
+                            pathtiff = outfile / 'tiff'
+                            pathsmv = outfile / 'SMV'
+                            pathred = outfile / 'RED'
+
+                            self.auto_cred_collection(outfile, pathtiff, pathsmv, pathred, transform_imgshift, transform_imgshift2, transform_imgshift_foc, transform_imgshift2_foc, transform_beamshift_d, transform_beamshift_d_defoc, self.calib_beamshift)
+
+                            self.ctrl.beamshift.set(x=self.calib_beamshift.reference_shift[0], y=self.calib_beamshift.reference_shift[1])
+                            self.ctrl.mode.set('mag1')
+                            self.ctrl.brightness.value = 65535
+                            time.sleep(0.5)
+
+                            self.rotation_direction = self.eliminate_backlash_in_tiltx()
+                            img, h = self.ctrl.get_image(exposure=self.expt, header_keys=header_keys)
+                            h['exp_magnification'] = self.ctrl.magnification.get()
+                            write_tiff(path / f'Overall_view_{k:04d}', img, h)
+
+                            crystal_positions = find_crystals_timepix(img, self.magnification, spread=self.spread, offset=self.offset)
+                            crystal_coords = [(crystal.x, crystal.y) for crystal in crystal_positions]
+                            # self.ctrl.brightness.value = img_brightness
+
+                            if n_crystals == 0:
+                                self.print_and_del('No crystals found in the image. exitting loop...')
+                                break
+
+                            (beamshiftcoord_0, size_crystal_targeted) = self.center_particle_from_crystalList(crystal_positions, transform_stagepos, self.magnification, self.beam_size_avg)
+
+                            img, h = self.ctrl.get_image(exposure=self.expt, header_keys=header_keys)
+                            h['exp_magnification'] = self.ctrl.magnification.get()
+                            write_tiff(path / f'Overall_view_{k:04d}', img, h)
+
+                            crystal_positions = find_crystals_timepix(img, self.magnification, spread=self.spread, offset=self.offset)
+                            crystal_coords = [(crystal.x, crystal.y) for crystal in crystal_positions]
+                            crystal_sizes = [crystal.area_pixel for crystal in crystal_positions]
+                            n_crystals = len(crystal_coords)
+
+                            if n_crystals == 0:
+                                self.print_and_del('No crystals found in the image. Find another area!')
+                                break
+
+                            if size_crystal_targeted != 0:
+                                try:
+                                    ind_target = crystal_sizes.index(size_crystal_targeted)
+                                    crystal_coords[k + 1], crystal_coords[ind_target] = crystal_coords[ind_target], crystal_coords[k + 1]
+                                    self.print_and_del('Targeted isolated crystal centered is swapped to the next.')
+                                except ValueError:
+                                    self.print_and_del('Lost targeted isolated crystal.')
+                                    break
+
+                        else:
+                            if self.verbose:
+                                print(f'Crystal {k + 1} not isolated: not suitable for cred collection')
+
+                        k = k + 1
+                        if k >= n_crystals:
+                            break
+                    except BaseException:
+                        traceback.print_exc()
+                        self.ctrl.beam.unblank()
+                        self.print_and_del('Exitting loop...')
+                        break
+
+                self.ctrl.mode.set('mag1')
+                self.ctrl.brightness.value = 65535
+
+                self.ctrl.imageshift1.set(x=IS1_Neut[0], y=IS1_Neut[1])
+                self.ctrl.imageshift2.set(x=IS2_Neut[0], y=IS2_Neut[1])
+
+                self.ctrl.beamshift.set(x=self.calib_beamshift.reference_shift[0], y=self.calib_beamshift.reference_shift[1])
+
+                if self.verbose:
+                    print('AutocRED with crystal_finder data collection done. Find another area for particles.')
+
+            if os.listdir(path) == ['Overall_view.tiff']:
+                shutil.rmtree(path)
+                # print("Path {} removed since no crystal rotation data was collected.".format(path))
+
+            try:
+                if len(os.listdir(path)) == 0:
+                    os.rmdir(path)
+                    # print("Path {} removed since it is empty.".format(path))
+            except BaseException:
+                # print("Deletion error. Path might have already been deleted.")
+                pass
+
+        elif self.mode == 1 or self.mode == 2:
+            self.pathtiff = Path(self.path) / 'tiff'
+            self.pathsmv = Path(self.path) / 'SMV'
+            self.pathred = Path(self.path) / 'RED'
+
+            for path in (self.path, self.pathtiff, self.pathsmv, self.pathred):
+                if not os.path.exists(path):
+                    os.makedirs(path)
+            self.auto_cred_collection(self.path, self.pathtiff, self.pathsmv, self.pathred, transform_imgshift, transform_imgshift2, transform_imgshift_foc, transform_imgshift2_foc, transform_beamshift_d, transform_beamshift_d_defoc, self.calib_beamshift)
+
+        else:
+            print('Choose cRED tab for data collection with manual/blind tracking.')
+            return 0
+
+    def start_collection(self):
+        ready = input('Please make sure that you have adjusted Goniotool if you are using full autocRED!')
+        if self.stopEvent_rasterScan.is_set():
+            # print("Raster scan stopper clearing..")
+            self.stopEvent_rasterScan.clear()
+
+        if not self.auto_zheight:
+            try:
+                with open(self.calibdir / 'z-height-adjustment-time.pkl', 'rb') as f:
+                    t = pickle.load(f)
+                    if t - time.perf_counter() > 14400:
+                        self.print_and_del('Z-height needs to be updated every session. Readjusting z-height...')
+                        x_zheight, y_zheight = center_z_height_HYMethod(self.ctrl, spread=self.spread, offset=self.offset)
+                        xpoint, ypoint, zpoint, aaa, bbb = self.ctrl.stage.get()
+                        self.logger.info(f'Stage position: x = {xpoint}, y = {ypoint}. Z height adjusted to {zpoint}. Tilt angle x {aaa} deg, Tilt angle y {bbb} deg')
+                        t = time.perf_counter()
+                        with open(self.calibdir / 'z-height-adjustment-time.pkl', 'wb') as f:
+                            pickle.dump(t, f)
+
+            except BaseException:
+                input('No z-height adjustment found. Please find an area with particles! Press Enter to continue auto adjustment of z height>>>')
+                x_zheight, y_zheight = center_z_height_HYMethod(self.ctrl, spread=self.spread, offset=self.offset)
+                xpoint, ypoint, zpoint, aaa, bbb = self.ctrl.stage.get()
+                self.logger.info(f'Stage position: x = {xpoint}, y = {ypoint}. Z height adjusted to {zpoint}. Tilt angle x {aaa} deg, Tilt angle y {bbb} deg')
+                t = time.perf_counter()
+                with open(self.calibdir / 'z-height-adjustment-time.pkl', 'wb') as f:
+                    pickle.dump(t, f)
+        else:
+            self.print_and_del('Z height adjusting...')
+            x_zheight, y_zheight = center_z_height_HYMethod(self.ctrl, spread=self.spread, offset=self.offset)
+            xpoint, ypoint, zpoint, aaa, bbb = self.ctrl.stage.get()
+            self.logger.info(f'Stage position: x = {xpoint}, y = {ypoint}. Z height adjusted to {zpoint}. Tilt angle x {aaa} deg, Tilt angle y {bbb} deg')
+            t = time.perf_counter()
+            with open(self.calibdir / 'z-height-adjustment-time.pkl', 'wb') as f:
+                pickle.dump(t, f)
+
+        lensPar = self.ctrl.to_dict()
+        with open(self.calibdir / 'LensPar.pkl', 'wb') as f:
+            pickle.dump(lensPar, f)
+
+        # Check DIALS server connection status here
+
+        if self.scan_area == 0:
+            self.start_collection_point()
+        else:
+            self.raster_scan()
+
+        self.stopEvent_rasterScan.clear()
+
+        with open(self.calibdir / 'LensPar.pkl', 'rb') as f:
+            lensPar_i = pickle.load(f)
+
+        self.ctrl.from_dict(lensPar_i)
+        self.ctrl.beam.blank()
+
+        print('AutocRED collection done.')
+        self.number_crystals_scanned = 0
+        self.number_exp_performed = 0
```

### Comparing `instamatic-1.8.0/instamatic/experiments/cred/experiment.py` & `instamatic-1.9.0/instamatic/experiments/cred/experiment.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,430 +1,432 @@
-import datetime
-import json
-import socket
-import time
-from pathlib import Path
-
-import numpy as np
-
-import instamatic
-from instamatic import config
-from instamatic.formats import write_tiff
-from instamatic.processing.ImgConversionTPX import ImgConversionTPX as ImgConversion
-
-# degrees to rotate before activating data collection procedure
-ACTIVATION_THRESHOLD = 0.2
-
-use_vm = config.settings.use_VM_server_exe
-
-
-def print_and_log(msg, logger=None):
-    print(msg)
-    if logger:
-        logger.info(msg)
-
-
-class Experiment:
-    """Initialize continuous rotation electron diffraction experiment.
-
-    ctrl:
-        Instance of instamatic.TEMController.TEMController
-    path:
-        `str` or `pathlib.Path` object giving the path to save data at
-    log:
-        Instance of `logging.Logger`
-    flatfield:
-        Path to flatfield correction image
-    unblank_beam:
-        Whether beam should be automatically unblanked before experiment
-    mode:
-        Which mode the experiment is running in, choices: 'simulate', 'footfree', None (default)
-    footfree_rotate_to:
-        In 'footfree' mode, rotate to this angle
-    enable_image_interval:
-        Gives the interval with which to defocs the pattern slightly for tracking purposes,
-        default is set to 99999 so it never occurs.
-    diff_defocus:
-        Image interval only - Defocus value to apply when defocused images are used for tracking
-    exposure_time_image:
-        Image interval only - Exposure time for defocused images
-    write_tiff, write_xds, write_dials, write_red:
-        Specify which data types/input files should be written
-    stop_event:
-        Instance of `threading.Event()` that signals the experiment to be terminated.
-    """
-
-    def __init__(self, ctrl,
-                 path: str = None,
-                 log=None,
-                 flatfield: str = None,
-                 exposure_time: float = 0.5,
-                 unblank_beam: bool = False,
-                 mode: str = None,
-                 footfree_rotate_to: float = 60.0,
-                 enable_image_interval: bool = False,
-                 image_interval: int = 99999,
-                 diff_defocus: int = 0,
-                 exposure_time_image: float = 0.01,
-                 write_tiff: bool = True,
-                 write_xds: bool = True,
-                 write_dials: bool = True,
-                 write_red: bool = True,
-                 stop_event=None,
-                 ):
-        super().__init__()
-        self.ctrl = ctrl
-        self.path = Path(path)
-        self.exposure = exposure_time
-        self.unblank_beam = unblank_beam
-        self.logger = log
-        self.mode = mode
-        if ctrl.cam.name == 'simulate':
-            self.mode = 'simulate'
-        self.stopEvent = stop_event
-        self.flatfield = flatfield
-
-        self.footfree_rotate_to = footfree_rotate_to
-
-        self.diff_defocus = diff_defocus
-        self.exposure_image = exposure_time_image
-
-        self.write_tiff = write_tiff
-        self.write_xds = write_xds
-        self.write_dials = write_dials
-        self.write_red = write_red
-        self.write_pets = write_tiff  # TODO
-
-        self.image_interval_enabled = enable_image_interval
-        if enable_image_interval:
-            self.image_interval = image_interval
-            print_and_log(f'Image interval enabled: every {self.image_interval} frames an image with defocus {self.diff_defocus} will be displayed (t={self.exposure_image} s).', logger=self.logger)
-        else:
-            self.image_interval = 99999
-
-        self.relax_beam_before_experiment = self.image_interval_enabled and config.settings.cred_relax_beam_before_experiment
-
-        self.track_stage_position = config.settings.cred_track_stage_positions
-        self.stage_positions = []
-
-        if use_vm:
-            self.s2 = socket.socket()
-            vm_host = config.settings.VM_server_host
-            vm_port = config.settings.VM_server_port
-        try:
-            self.s2.connect((vm_host, vm_port))
-            print('VirtualBox server connected for autocRED.')
-            self.s2_c = 1
-        except BaseException:
-            print('Is VM server running? Connection failed.')
-            self.s2_c = 0
-
-    def log_start_status(self):
-        """Log the starting parameters."""
-        self.now = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-        self.logger.info(f'Data recording started at: {self.now}')
-        self.logger.info(f'Data collection exposure time: {self.exposure} s')
-        self.logger.info(f'Data saving path: {self.path}')
-
-    def log_end_status(self):
-        """Log the experimental values, write file `cRED_log.txt`"""
-        start_xy = np.array(self.start_position[0:2])
-        end_xy = np.array(self.end_position[0:2])
-
-        print_and_log(f'Rotated {self.total_angle:.2f} degrees from {self.start_angle:.2f} to {self.end_angle:.2f} in {self.nframes} frames (step: {self.osc_angle:.4f})', logger=self.logger)
-
-        def fmt(arr):
-            return f'[{arr[0]:.0f} {arr[1]:.0f}]'
-        print_and_log(f'Stage moved from {fmt(start_xy)} to {fmt(end_xy)}, drift: {fmt(start_xy - end_xy)}', logger=self.logger)
-        self.logger.info(f'Start stage position: {self.start_position}')
-        self.logger.info(f'End stage position: {self.end_position}')
-        self.logger.info(f'Data collection camera length: {self.camera_length} mm')
-        self.logger.info(f'Data collection spot size: {self.spotsize}')
-
-        self.logger.info(self.stage_positions)
-
-        with open(self.path / 'cRED_log.txt', 'w') as f:
-            print(f'Program: {instamatic.__long_title__}', file=f)
-            print(f'Data Collection Time: {self.now}', file=f)
-            print(f'Time Period Start: {self.t_start}', file=f)
-            print(f'Time Period End: {self.t_end}', file=f)
-            print(f'Starting angle: {self.start_angle:.2f} degrees', file=f)
-            print(f'Ending angle: {self.end_angle:.2f} degrees', file=f)
-            print(f'Rotation range: {self.end_angle-self.start_angle:.2f} degrees', file=f)
-            print(f'Exposure Time: {self.exposure:.3f} s', file=f)
-            print(f'Acquisition time: {self.acquisition_time:.3f} s', file=f)
-            print(f'Total time: {self.total_time:.3f} s', file=f)
-            print(f'Spot Size: {self.spotsize}', file=f)
-            print(f'Camera length: {self.camera_length} mm', file=f)
-            print(f'Pixelsize: {self.pixelsize} px/Angstrom', file=f)
-            print(f'Physical pixelsize: {self.physical_pixelsize} um', file=f)
-            print(f'Wavelength: {self.wavelength} Angstrom', file=f)
-            print(f'Stretch amplitude: {self.stretch_azimuth} %', file=f)
-            print(f'Stretch azimuth: {self.stretch_amplitude} degrees', file=f)
-            print(f'Rotation axis: {self.rotation_axis} radians', file=f)
-            print(f'Oscillation angle: {self.osc_angle:.4f} degrees', file=f)
-            print(f'Number of frames: {self.nframes_diff}', file=f)
-            print('Stage start: X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:5.2f} | B {:5.2f}'.format(*self.start_position), file=f)
-            print('Stage end:   X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:5.2f} | B {:5.2f}'.format(*self.end_position), file=f)
-
-            if self.image_interval_enabled:
-                print(f'Image interval: every {self.image_interval} frames an image with defocus {self.diff_focus_defocused} (t={self.exposure_image} s).', file=f)
-                print(f'Number of images: {self.nframes_image}', file=f)
-
-            print('', file=f)
-            print('References:', file=f)
-            print(' -', instamatic.__citation__, file=f)
-            print(' -', instamatic.__citation_cred__, file=f)
-
-    def setup_paths(self):
-        """Set up the paths for saving the data to."""
-        print(f'\nOutput directory: {self.path}')
-        self.tiff_path = self.path / 'tiff' if self.write_tiff else None
-        self.smv_path = self.path / 'SMV' if (self.write_xds or self.write_dials) else None
-        self.mrc_path = self.path / 'RED' if self.write_red else None
-
-    def start_rotation(self) -> float:
-        """Controls the starting of the rotation of the experiment.
-
-        In the default mode, wait for rotation to start (i.e. controlled via the pedals)
-        In `footfree` mode, initialize rotation from current angle to target angle.
-        In `simulate` mode, simulate the start condition.
-
-        Returns the starting value for the rotation.
-        """
-        self.start_position = self.ctrl.stage.get()
-        self.stage_positions.append((0, self.start_position))
-        a = self.start_position[3]
-
-        if self.mode == 'simulate':
-            start_angle = a
-            print('Data Recording started.')
-
-        elif self.mode == 'footfree':
-            rotate_to = self.footfree_rotate_to
-
-            start_angle = self.ctrl.stage.a
-            self.ctrl.stage.set(a=rotate_to, wait=False)
-
-        else:
-            print('Waiting for rotation to start...', end=' ')
-            a0 = a
-            while abs(a - a0) < ACTIVATION_THRESHOLD:
-                if self.stopEvent.is_set():
-                    break
-
-                a = self.ctrl.stage.a
-
-            print('Data Recording started.')
-            start_angle = a
-
-        if self.unblank_beam:
-            print('Unblanking beam')
-            self.ctrl.beam.unblank()
-
-        return start_angle
-
-    def relax_beam(self, n_cycles: int = 5):
-        """Relax the beam prior to the experiment by toggling between the
-        defocused/focused states."""
-        print(f'Relaxing beam ({n_cycles} cycles)', end='')
-
-        for i in range(n_cycles):
-            self.ctrl.difffocus.set(self.diff_focus_defocused)
-            time.sleep(0.5)
-            print(f'.', end='')
-            self.ctrl.difffocus.set(self.diff_focus_proper)
-            time.sleep(0.5)
-            print(f'.', end='')
-
-        print('Done.')
-
-    def start_collection(self) -> bool:
-        """Main experimental function, returns True if experiment runs
-        normally, False if it is interrupted for whatever reason."""
-        self.setup_paths()
-        self.log_start_status()
-
-        buffer = []
-        image_buffer = []
-
-        if self.ctrl.mode != 'diff':
-            self.ctrl.mode.set('diff')
-
-        self.diff_focus_proper = self.ctrl.difffocus.value
-        self.diff_focus_defocused = self.diff_defocus + self.diff_focus_proper
-        exposure_image = self.exposure_image
-
-        if self.relax_beam_before_experiment:
-            self.relax_beam()
-
-        self.start_angle = self.start_rotation()
-        self.ctrl.cam.block()
-
-        i = 1
-
-        t0 = time.perf_counter()
-
-        while not self.stopEvent.is_set():
-            if i % self.image_interval == 0:
-                t_start = time.perf_counter()
-                acquisition_time = (t_start - t0) / (i - 1)
-
-                self.ctrl.difffocus.set(self.diff_focus_defocused, confirm_mode=False)
-                img, h = self.ctrl.get_image(exposure_image, header_keys=None)
-                self.ctrl.difffocus.set(self.diff_focus_proper, confirm_mode=False)
-
-                image_buffer.append((i, img, h))
-
-                next_interval = t_start + acquisition_time
-                # print(f"{i} BLOOP! {next_interval-t_start:.3f} {acquisition_time:.3f} {t_start-t0:.3f}")
-
-                while time.perf_counter() > next_interval:
-                    next_interval += acquisition_time
-                    i += 1
-                    # print(f"{i} "SKIP!  {next_interval-t_start:.3f} {acquisition_time:.3f}")
-
-                diff = next_interval - time.perf_counter()  # seconds
-
-                if self.track_stage_position and diff > 0.1:
-                    self.stage_positions.append((i, self.ctrl.stage.get()))
-
-                time.sleep(diff)
-
-            else:
-                img, h = self.ctrl.get_image(self.exposure, header_keys=None)
-                # print(f"{i} Image!")
-                buffer.append((i, img, h))
-
-            i += 1
-
-        t1 = time.perf_counter()
-
-        if self.mode == 'footfree':
-            self.ctrl.stage.stop()
-
-        self.stopEvent.clear()
-
-        self.ctrl.cam.unblock()
-
-        if self.mode == 'simulate':
-            # simulate somewhat realistic end numbers
-            self.ctrl.stage.x += np.random.randint(-5000, 5000)
-            self.ctrl.stage.y += np.random.randint(-5000, 5000)
-            self.ctrl.stage.a += np.random.randint(-100, 100)
-            self.ctrl.magnification.set(300)
-
-        self.end_position = self.ctrl.stage.get()
-        self.end_angle = self.end_position[3]
-        self.camera_length = int(self.ctrl.magnification.get())
-        self.stage_positions.append((99999, self.end_position))
-
-        is_moving = bool(self.ctrl.stage.is_moving())
-        self.logger.info(f'Experiment finished, stage is moving: {is_moving}')
-
-        if self.unblank_beam:
-            print('Blanking beam')
-            self.ctrl.beam.blank()
-
-        # in case something went wrong starting data collection, return gracefully
-        if i == 1:
-            print_and_log(f'Data collection interrupted', logger=self.logger)
-            return False
-
-        self.spotsize = self.ctrl.spotsize
-        self.nframes = i - 1  # len(buffer) can lie in case of frame skipping
-        self.osc_angle = abs(self.end_angle - self.start_angle) / self.nframes
-        self.t_start = t0
-        self.t_end = t1
-        self.total_time = t1 - t0
-        self.acquisition_time = self.total_time / self.nframes
-        self.total_angle = abs(self.end_angle - self.start_angle)
-        self.rotation_axis = config.camera.camera_rotation_vs_stage_xy
-
-        self.pixelsize = config.calibration['diff']['pixelsize'][self.camera_length]  # px / Angstrom
-        self.physical_pixelsize = config.camera.physical_pixelsize  # mm
-        self.wavelength = config.microscope.wavelength  # angstrom
-        self.stretch_azimuth = config.camera.stretch_azimuth  # deg
-        self.stretch_amplitude = config.camera.stretch_amplitude  # %
-
-        self.nframes_diff = len(buffer)
-        self.nframes_image = len(image_buffer)
-
-        self.log_end_status()
-
-        if self.nframes <= 3:
-            print_and_log(f'Not enough frames collected. Data will not be written (nframes={self.nframes})', logger=self.logger)
-            return False
-
-        self.write_data(buffer)
-        self.write_image_data(image_buffer)
-
-        print('Data Collection and Conversion Done.')
-
-        pathsmv_str = str(self.smv_path)
-        msg = {'path': pathsmv_str,
-               'rotrange': self.total_angle,
-               'nframes': self.nframes,
-               'osc': self.osc_angle}
-        msg_tosend = json.dumps(msg).encode('utf8')
-
-        if self.s2_c:
-            self.s2.send(msg_tosend)
-            print('SMVs sent to XDS for processing.')
-
-        return True
-
-    def write_data(self, buffer: list):
-        """Write diffraction data in the buffer.
-
-        The image buffer is passed as a list of tuples, where each tuple contains the
-        index (int), image data (2D numpy array), metadata/header (dict).
-
-        The buffer index must start at 1.
-        """
-
-        img_conv = ImgConversion(buffer=buffer,
-                                 osc_angle=self.osc_angle,
-                                 start_angle=self.start_angle,
-                                 end_angle=self.end_angle,
-                                 rotation_axis=self.rotation_axis,
-                                 acquisition_time=self.acquisition_time,
-                                 flatfield=self.flatfield,
-                                 pixelsize=self.pixelsize,
-                                 physical_pixelsize=self.physical_pixelsize,
-                                 wavelength=self.wavelength,
-                                 stretch_amplitude=self.stretch_amplitude,
-                                 stretch_azimuth=self.stretch_azimuth,
-                                 )
-
-        print('Writing data files...')
-        img_conv.threadpoolwriter(tiff_path=self.tiff_path,
-                                  mrc_path=self.mrc_path,
-                                  smv_path=self.smv_path,
-                                  workers=8)
-
-        print('Writing input files...')
-        if self.write_dials:
-            img_conv.to_dials(self.smv_path)
-        if self.write_red:
-            img_conv.write_ed3d(self.mrc_path)
-        if self.write_xds or self.write_dials:
-            img_conv.write_xds_inp(self.smv_path)
-        if self.write_pets:
-            img_conv.write_pets_inp(self.path)
-
-        img_conv.write_beam_centers(self.path)
-
-    def write_image_data(self, buffer: list):
-        """Write image data in the buffer.
-
-        The image buffer is passed as a list of tuples, where each tuple
-        contains the index (int), image data (2D numpy array),
-        metadata/header (dict).
-        """
-        if buffer:
-            drc = self.path / 'tiff_image'
-            drc.mkdir(exist_ok=True)
-            while len(buffer) != 0:
-                i, img, h = buffer.pop(0)
-                fn = drc / f'{i:05d}.tiff'
-                write_tiff(fn, img, header=h)
+import datetime
+import json
+import socket
+import time
+from pathlib import Path
+
+import numpy as np
+
+import instamatic
+from instamatic import config
+from instamatic.formats import write_tiff
+from instamatic.processing.ImgConversionTPX import ImgConversionTPX as ImgConversion
+
+# degrees to rotate before activating data collection procedure
+ACTIVATION_THRESHOLD = 0.2
+
+use_vm = config.settings.use_VM_server_exe
+
+
+def print_and_log(msg, logger=None):
+    print(msg)
+    if logger:
+        logger.info(msg)
+
+
+class Experiment:
+    """Initialize continuous rotation electron diffraction experiment.
+
+    ctrl:
+        Instance of instamatic.TEMController.TEMController
+    path:
+        `str` or `pathlib.Path` object giving the path to save data at
+    log:
+        Instance of `logging.Logger`
+    flatfield:
+        Path to flatfield correction image
+    unblank_beam:
+        Whether beam should be automatically unblanked before experiment
+    mode:
+        Which mode the experiment is running in, choices: 'simulate', 'footfree', None (default)
+    footfree_rotate_to:
+        In 'footfree' mode, rotate to this angle
+    enable_image_interval:
+        Gives the interval with which to defocs the pattern slightly for tracking purposes,
+        default is set to 99999 so it never occurs.
+    diff_defocus:
+        Image interval only - Defocus value to apply when defocused images are used for tracking
+    exposure_time_image:
+        Image interval only - Exposure time for defocused images
+    write_tiff, write_xds, write_dials, write_red:
+        Specify which data types/input files should be written
+    stop_event:
+        Instance of `threading.Event()` that signals the experiment to be terminated.
+    """
+
+    def __init__(self, ctrl,
+                 path: str = None,
+                 log=None,
+                 flatfield: str = None,
+                 exposure_time: float = 0.5,
+                 unblank_beam: bool = False,
+                 mode: str = None,
+                 footfree_rotate_to: float = 60.0,
+                 enable_image_interval: bool = False,
+                 image_interval: int = 99999,
+                 diff_defocus: int = 0,
+                 exposure_time_image: float = 0.01,
+                 write_tiff: bool = True,
+                 write_xds: bool = True,
+                 write_dials: bool = True,
+                 write_red: bool = True,
+                 stop_event=None,
+                 ):
+        super().__init__()
+        self.ctrl = ctrl
+        self.path = Path(path)
+        self.exposure = exposure_time
+        self.unblank_beam = unblank_beam
+        self.logger = log
+        self.mode = mode
+        if ctrl.cam.name == 'simulate':
+            self.mode = 'simulate'
+        self.stopEvent = stop_event
+        self.flatfield = flatfield
+
+        self.footfree_rotate_to = footfree_rotate_to
+
+        self.diff_defocus = diff_defocus
+        self.exposure_image = exposure_time_image
+
+        self.write_tiff = write_tiff
+        self.write_xds = write_xds
+        self.write_dials = write_dials
+        self.write_red = write_red
+        self.write_pets = write_tiff  # TODO
+
+        self.image_interval_enabled = enable_image_interval
+        if enable_image_interval:
+            self.image_interval = image_interval
+            print_and_log(f'Image interval enabled: every {self.image_interval} frames an image with defocus {self.diff_defocus} will be displayed (t={self.exposure_image} s).', logger=self.logger)
+        else:
+            self.image_interval = 99999
+
+        self.relax_beam_before_experiment = self.image_interval_enabled and config.settings.cred_relax_beam_before_experiment
+
+        self.track_stage_position = config.settings.cred_track_stage_positions
+        self.stage_positions = []
+
+        if use_vm:
+            self.s2 = socket.socket()
+            vm_host = config.settings.VM_server_host
+            vm_port = config.settings.VM_server_port
+        try:
+            self.s2.connect((vm_host, vm_port))
+            print('VirtualBox server connected for autocRED.')
+            self.s2_c = 1
+        except BaseException:
+            print('Is VM server running? Connection failed.')
+            self.s2_c = 0
+
+    def log_start_status(self):
+        """Log the starting parameters."""
+        self.now = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+        self.logger.info(f'Data recording started at: {self.now}')
+        self.logger.info(f'Data collection exposure time: {self.exposure} s')
+        self.logger.info(f'Data saving path: {self.path}')
+
+    def log_end_status(self):
+        """Log the experimental values, write file `cRED_log.txt`"""
+        start_xy = np.array(self.start_position[0:2])
+        end_xy = np.array(self.end_position[0:2])
+
+        print_and_log(f'Rotated {self.total_angle:.2f} degrees from {self.start_angle:.2f} to {self.end_angle:.2f} in {self.nframes} frames (step: {self.osc_angle:.4f})', logger=self.logger)
+
+        def fmt(arr):
+            return f'[{arr[0]:.0f} {arr[1]:.0f}]'
+        print_and_log(f'Stage moved from {fmt(start_xy)} to {fmt(end_xy)}, drift: {fmt(start_xy - end_xy)}', logger=self.logger)
+        self.logger.info(f'Start stage position: {self.start_position}')
+        self.logger.info(f'End stage position: {self.end_position}')
+        self.logger.info(f'Data collection camera length: {self.camera_length} mm')
+        self.logger.info(f'Data collection spot size: {self.spotsize}')
+
+        self.logger.info(self.stage_positions)
+
+        with open(self.path / 'cRED_log.txt', 'w') as f:
+            print(f'Program: {instamatic.__long_title__}', file=f)
+            print(f'Data Collection Time: {self.now}', file=f)
+            print(f'Time Period Start: {self.t_start}', file=f)
+            print(f'Time Period End: {self.t_end}', file=f)
+            print(f'Starting angle: {self.start_angle:.2f} degrees', file=f)
+            print(f'Ending angle: {self.end_angle:.2f} degrees', file=f)
+            print(f'Rotation range: {self.end_angle-self.start_angle:.2f} degrees', file=f)
+            print(f'Exposure Time: {self.exposure:.3f} s', file=f)
+            print(f'Acquisition time: {self.acquisition_time:.3f} s', file=f)
+            print(f'Total time: {self.total_time:.3f} s', file=f)
+            print(f'Spot Size: {self.spotsize}', file=f)
+            print(f'Camera length: {self.camera_length} mm', file=f)
+            print(f'Pixelsize: {self.pixelsize} px/Angstrom', file=f)
+            print(f'Physical pixelsize: {self.physical_pixelsize} um', file=f)
+            print(f'Wavelength: {self.wavelength} Angstrom', file=f)
+            print(f'Stretch amplitude: {self.stretch_azimuth} %', file=f)
+            print(f'Stretch azimuth: {self.stretch_amplitude} degrees', file=f)
+            print(f'Rotation axis: {self.rotation_axis} radians', file=f)
+            print(f'Oscillation angle: {self.osc_angle:.4f} degrees', file=f)
+            print(f'Number of frames: {self.nframes_diff}', file=f)
+            print('Stage start: X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:5.2f} | B {:5.2f}'.format(*self.start_position), file=f)
+            print('Stage end:   X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:5.2f} | B {:5.2f}'.format(*self.end_position), file=f)
+
+            if self.image_interval_enabled:
+                print(f'Image interval: every {self.image_interval} frames an image with defocus {self.diff_focus_defocused} (t={self.exposure_image} s).', file=f)
+                print(f'Number of images: {self.nframes_image}', file=f)
+
+            print('', file=f)
+            print('References:', file=f)
+            print(' -', instamatic.__citation__, file=f)
+            print(' -', instamatic.__citation_cred__, file=f)
+
+    def setup_paths(self):
+        """Set up the paths for saving the data to."""
+        print(f'\nOutput directory: {self.path}')
+        self.tiff_path = self.path / 'tiff' if self.write_tiff else None
+        self.smv_path = self.path / 'SMV' if (self.write_xds or self.write_dials) else None
+        self.mrc_path = self.path / 'RED' if self.write_red else None
+
+    def start_rotation(self) -> float:
+        """Controls the starting of the rotation of the experiment.
+
+        In the default mode, wait for rotation to start (i.e. controlled
+        via the pedals) In `footfree` mode, initialize rotation from
+        current angle to target angle. In `simulate` mode, simulate the
+        start condition.
+
+        Returns the starting value for the rotation.
+        """
+        self.start_position = self.ctrl.stage.get()
+        self.stage_positions.append((0, self.start_position))
+        a = self.start_position[3]
+
+        if self.mode == 'simulate':
+            start_angle = a
+            print('Data Recording started.')
+
+        elif self.mode == 'footfree':
+            rotate_to = self.footfree_rotate_to
+
+            start_angle = self.ctrl.stage.a
+            self.ctrl.stage.set(a=rotate_to, wait=False)
+
+        else:
+            print('Waiting for rotation to start...', end=' ')
+            a0 = a
+            while abs(a - a0) < ACTIVATION_THRESHOLD:
+                if self.stopEvent.is_set():
+                    break
+
+                a = self.ctrl.stage.a
+
+            print('Data Recording started.')
+            start_angle = a
+
+        if self.unblank_beam:
+            print('Unblanking beam')
+            self.ctrl.beam.unblank()
+
+        return start_angle
+
+    def relax_beam(self, n_cycles: int = 5):
+        """Relax the beam prior to the experiment by toggling between the
+        defocused/focused states."""
+        print(f'Relaxing beam ({n_cycles} cycles)', end='')
+
+        for i in range(n_cycles):
+            self.ctrl.difffocus.set(self.diff_focus_defocused)
+            time.sleep(0.5)
+            print('.', end='')
+            self.ctrl.difffocus.set(self.diff_focus_proper)
+            time.sleep(0.5)
+            print('.', end='')
+
+        print('Done.')
+
+    def start_collection(self) -> bool:
+        """Main experimental function, returns True if experiment runs
+        normally, False if it is interrupted for whatever reason."""
+        self.setup_paths()
+        self.log_start_status()
+
+        buffer = []
+        image_buffer = []
+
+        if self.ctrl.mode != 'diff':
+            self.ctrl.mode.set('diff')
+
+        self.diff_focus_proper = self.ctrl.difffocus.value
+        self.diff_focus_defocused = self.diff_defocus + self.diff_focus_proper
+        exposure_image = self.exposure_image
+
+        if self.relax_beam_before_experiment:
+            self.relax_beam()
+
+        self.start_angle = self.start_rotation()
+        self.ctrl.cam.block()
+
+        i = 1
+
+        t0 = time.perf_counter()
+
+        while not self.stopEvent.is_set():
+            if i % self.image_interval == 0:
+                t_start = time.perf_counter()
+                acquisition_time = (t_start - t0) / (i - 1)
+
+                self.ctrl.difffocus.set(self.diff_focus_defocused, confirm_mode=False)
+                img, h = self.ctrl.get_image(exposure_image, header_keys=None)
+                self.ctrl.difffocus.set(self.diff_focus_proper, confirm_mode=False)
+
+                image_buffer.append((i, img, h))
+
+                next_interval = t_start + acquisition_time
+                # print(f"{i} BLOOP! {next_interval-t_start:.3f} {acquisition_time:.3f} {t_start-t0:.3f}")
+
+                while time.perf_counter() > next_interval:
+                    next_interval += acquisition_time
+                    i += 1
+                    # print(f"{i} "SKIP!  {next_interval-t_start:.3f} {acquisition_time:.3f}")
+
+                diff = next_interval - time.perf_counter()  # seconds
+
+                if self.track_stage_position and diff > 0.1:
+                    self.stage_positions.append((i, self.ctrl.stage.get()))
+
+                time.sleep(diff)
+
+            else:
+                img, h = self.ctrl.get_image(self.exposure, header_keys=None)
+                # print(f"{i} Image!")
+                buffer.append((i, img, h))
+
+            i += 1
+
+        t1 = time.perf_counter()
+
+        if self.mode == 'footfree':
+            self.ctrl.stage.stop()
+
+        self.stopEvent.clear()
+
+        self.ctrl.cam.unblock()
+
+        if self.mode == 'simulate':
+            # simulate somewhat realistic end numbers
+            self.ctrl.stage.x += np.random.randint(-5000, 5000)
+            self.ctrl.stage.y += np.random.randint(-5000, 5000)
+            self.ctrl.stage.a += np.random.randint(-100, 100)
+            self.ctrl.magnification.set(300)
+
+        self.end_position = self.ctrl.stage.get()
+        self.end_angle = self.end_position[3]
+        self.camera_length = int(self.ctrl.magnification.get())
+        self.stage_positions.append((99999, self.end_position))
+
+        is_moving = bool(self.ctrl.stage.is_moving())
+        self.logger.info(f'Experiment finished, stage is moving: {is_moving}')
+
+        if self.unblank_beam:
+            print('Blanking beam')
+            self.ctrl.beam.blank()
+
+        # in case something went wrong starting data collection, return gracefully
+        if i == 1:
+            print_and_log('Data collection interrupted', logger=self.logger)
+            return False
+
+        self.spotsize = self.ctrl.spotsize
+        self.nframes = i - 1  # len(buffer) can lie in case of frame skipping
+        self.osc_angle = abs(self.end_angle - self.start_angle) / self.nframes
+        self.t_start = t0
+        self.t_end = t1
+        self.total_time = t1 - t0
+        self.acquisition_time = self.total_time / self.nframes
+        self.total_angle = abs(self.end_angle - self.start_angle)
+        self.rotation_axis = config.camera.camera_rotation_vs_stage_xy
+
+        self.pixelsize = config.calibration['diff']['pixelsize'][self.camera_length]  # px / Angstrom
+        self.physical_pixelsize = config.camera.physical_pixelsize  # mm
+        self.wavelength = config.microscope.wavelength  # angstrom
+        self.stretch_azimuth = config.camera.stretch_azimuth  # deg
+        self.stretch_amplitude = config.camera.stretch_amplitude  # %
+
+        self.nframes_diff = len(buffer)
+        self.nframes_image = len(image_buffer)
+
+        self.log_end_status()
+
+        if self.nframes <= 3:
+            print_and_log(f'Not enough frames collected. Data will not be written (nframes={self.nframes})', logger=self.logger)
+            return False
+
+        self.write_data(buffer)
+        self.write_image_data(image_buffer)
+
+        print('Data Collection and Conversion Done.')
+
+        pathsmv_str = str(self.smv_path)
+        msg = {'path': pathsmv_str,
+               'rotrange': self.total_angle,
+               'nframes': self.nframes,
+               'osc': self.osc_angle}
+        msg_tosend = json.dumps(msg).encode('utf8')
+
+        if self.s2_c:
+            self.s2.send(msg_tosend)
+            print('SMVs sent to XDS for processing.')
+
+        return True
+
+    def write_data(self, buffer: list):
+        """Write diffraction data in the buffer.
+
+        The image buffer is passed as a list of tuples, where each tuple
+        contains the index (int), image data (2D numpy array),
+        metadata/header (dict).
+
+        The buffer index must start at 1.
+        """
+
+        img_conv = ImgConversion(buffer=buffer,
+                                 osc_angle=self.osc_angle,
+                                 start_angle=self.start_angle,
+                                 end_angle=self.end_angle,
+                                 rotation_axis=self.rotation_axis,
+                                 acquisition_time=self.acquisition_time,
+                                 flatfield=self.flatfield,
+                                 pixelsize=self.pixelsize,
+                                 physical_pixelsize=self.physical_pixelsize,
+                                 wavelength=self.wavelength,
+                                 stretch_amplitude=self.stretch_amplitude,
+                                 stretch_azimuth=self.stretch_azimuth,
+                                 )
+
+        print('Writing data files...')
+        img_conv.threadpoolwriter(tiff_path=self.tiff_path,
+                                  mrc_path=self.mrc_path,
+                                  smv_path=self.smv_path,
+                                  workers=8)
+
+        print('Writing input files...')
+        if self.write_dials:
+            img_conv.to_dials(self.smv_path)
+        if self.write_red:
+            img_conv.write_ed3d(self.mrc_path)
+        if self.write_xds or self.write_dials:
+            img_conv.write_xds_inp(self.smv_path)
+        if self.write_pets:
+            img_conv.write_pets_inp(self.path)
+
+        img_conv.write_beam_centers(self.path)
+
+    def write_image_data(self, buffer: list):
+        """Write image data in the buffer.
+
+        The image buffer is passed as a list of tuples, where each tuple
+        contains the index (int), image data (2D numpy array),
+        metadata/header (dict).
+        """
+        if buffer:
+            drc = self.path / 'tiff_image'
+            drc.mkdir(exist_ok=True)
+            while len(buffer) != 0:
+                i, img, h = buffer.pop(0)
+                fn = drc / f'{i:05d}.tiff'
+                write_tiff(fn, img, header=h)
```

### Comparing `instamatic-1.8.0/instamatic/experiments/cred_gatan/experiment.py` & `instamatic-1.9.0/instamatic/experiments/cred_gatan/experiment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,433 +1,433 @@
-import datetime
-import msvcrt
-import pickle
-import time
-from pathlib import Path
-
-import numpy as np
-from scipy.interpolate import interp1d
-
-import instamatic
-from instamatic import config
-from instamatic.formats import write_tiff
-
-
-class Experiment:
-    """Class to control data collection through DM to collect continuous
-    rotation electron diffraction data.
-
-    ctrl: `TEMController`
-        Instance of instamatic.TEMController.TEMController
-    path: str
-        `str` or `pathlib.Path` object giving the path to save data at
-    log: `logging.Logger`
-        Instance of `logging.Logger`
-    exposure: float
-        Exposure time in ms
-    mode: str
-    """
-
-    def __init__(self, ctrl,
-                 path: str = None,
-                 log=None,
-                 track: str = None,
-                 exposure: float = 400,
-                 mode: str = 'diff',
-                 rotation_speed: int = None):
-        super().__init__()
-
-        self.ctrl = ctrl
-        self.cam = ctrl.cam
-        self.path = Path(path)
-
-        self.exposure = exposure
-        self.defocus_offset = 1500
-
-        self.logger = log
-        self.mode = mode
-
-        self.rotation_speed = rotation_speed
-
-        if track:
-            self.load_tracking_file(track)
-            self.track = True
-        else:
-            self.track = False
-
-    def load_tracking_file(self, trackfile):
-        trackfile = Path(trackfile)
-        if trackfile.suffix == '.pickle':
-            print(f'(autotracking) Loading tracking file: {trackfile}')
-            dct = pickle.load(open(trackfile, 'rb'))
-
-            self.track_func = dct['y_offset']
-            self.x_offset = dct['x_offset']
-            self.start_x = dct['x_center']
-            self.start_y = dct['y_center']
-            self.start_z = dct['z_pos']
-
-            self.min_angle = dct['angle_min']
-            self.max_angle = dct['angle_max']
-
-            self.crystal_number = dct['i']
-
-            self.trackfile = trackfile
-
-            self.track_interval = 2
-            self.track_relative = False
-
-        else:
-            raise OSError("I don't know how to read file `{trackfile}`")
-
-    def prepare_tracking(self):
-        if self.track:
-            current_angle = self.ctrl.stage.a
-
-            min_angle = self.min_angle
-            max_angle = self.max_angle
-
-            # find start angle closest to current angle
-            if abs(min_angle - current_angle) > abs(max_angle - current_angle):
-                start_angle, target_angle = max_angle, min_angle
-            else:
-                start_angle, target_angle = min_angle, max_angle
-
-            print(f'(autotracking) Overriding angle range: {start_angle:.0f} -> {target_angle:.0f}')
-
-            y_offset = int(self.track_func(start_angle))
-            x_offset = self.x_offset
-
-            print(f'(autotracking) setting a={start_angle:.0f}, x={self.start_x+x_offset:.0f}, y={self.start_y+y_offset:.0f}, z={self.start_z:.0f}')
-            self.ctrl.stage.set_xy_with_backlash_correction(x=self.start_x + x_offset, y=self.start_y + y_offset, step=10000)
-            self.ctrl.stage.set(a=start_angle, z=self.start_z)
-
-            return start_angle, target_angle
-
-    def track_crystal(self, n, angle):
-        # tracking routine
-        if (n % self.track_interval == 0):
-            target_y = self.start_y + int(self.track_func(angle))
-            self.ctrl.stage.set(y=target_y, wait=False)
-            print(f'(autotracking) set y={target_y:.0f}')
-
-    def get_ready(self):
-        # self.cam.set_exposure(self.exposure)
-
-        if not self.ctrl.beam.is_blanked:
-            self.ctrl.beam.blank()
-
-        self.ctrl.screen.up()
-
-        if self.ctrl.mode != self.mode:
-            print(f'Switching to {self.mode} mode')
-            self.ctrl.mode.set(self.mode)
-
-        if self.mode == 'diff':
-            self.ctrl.difffocus.refocus()
-
-        spotsize = self.ctrl.spotsize
-
-        self.cam.set_tag('exp_directory', str(self.path))
-        self.cam.get_ready_for_record()
-        print('Ready...')
-
-    def manual_activation(self) -> float:
-        ACTIVATION_THRESHOLD = 0.2
-
-        print('Waiting for rotation to start...', end=' ')
-        a0 = a = self.ctrl.stage.a
-        while abs(a - a0) < ACTIVATION_THRESHOLD:
-            a = self.ctrl.stage.a
-
-        print('Rotation started...')
-
-        return a
-
-    def start_collection(self, target_angle: float, start_angle: float = None, manual_control: bool = False):
-        """
-        manual_control : bool
-            Control the rotation using the buttons or pedals
-        """
-        angle_tolerance = 0.5  # degrees
-
-        self.now = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-
-        self.stage_positions = []
-        interval = 0.7  # interval at which it check for rotation to end / does tracking
-
-        if self.track:
-            start_angle, target_angle = self.prepare_tracking()
-
-        if start_angle:
-            print(f'Going to starting angle: {start_angle:.1f}')
-            self.ctrl.stage.a = start_angle
-
-        self.start_position = self.ctrl.stage.get()
-        start_angle = self.start_position.a
-
-        if self.track:
-            # Center crystal position
-            if self.mode == 'diff':
-                self.ctrl.difffocus.defocus(self.defocus_offset)
-            self.ctrl.beam.unblank()
-
-            input('Move SAED aperture to crystal and press <ENTER> to measure! ')
-
-            # cannot do this while lieview is running
-            # img1 = self.ctrl.get_raw_image()
-            # write_tiff(self.path / "image_before.tiff", img1)
-
-            self.ctrl.beam.blank()
-            if self.mode == 'diff':
-                self.ctrl.difffocus.refocus()
-            time.sleep(3)
-
-        self.ctrl.beam.unblank()(delay=0.2)  # give the beamblank some time to dissappear to avoid weak first frame
-
-        if manual_control:
-            start_angle = self.manual_activation()
-            last_angle = 999
-        elif self.rotation_speed:
-            self.ctrl.stage.set_a_with_speed(a=target_angle, speed=self.rotation_speed, wait=False)
-        else:
-            self.ctrl.stage.set(a=target_angle, wait=False)
-
-        self.cam.start_record()  # start recording
-
-        t0 = time.perf_counter()
-        t_delta = t0
-
-        n = 0
-
-        print('Acquiring data...')
-
-        while True:
-            t = time.perf_counter()
-
-            if not manual_control:
-                if abs(self.ctrl.stage.a - target_angle) < angle_tolerance:
-                    print('Target angle reached!')
-                    break
-
-            if t - t_delta > interval:
-
-                n += 1
-                x, y, z, a, _ = pos = self.ctrl.stage.get()
-                self.stage_positions.append((t, pos))
-                t_delta = t
-                # print(t, pos)
-
-                if manual_control:
-                    current_angle = a
-                    if last_angle == current_angle:
-                        print(f'Manual rotation was interrupted (current: {current_angle:.2f} | last {last_angle:.2f})')
-                        break
-                    last_angle = current_angle
-
-                    print(f' >> Current angle: {a:.2f}', end='      \r')
-
-                if self.track:
-                    self.track_crystal(n=n, angle=a)
-
-            # Stop/interrupt and go to next crystal
-            if msvcrt.kbhit():
-                key = msvcrt.getch().decode()
-                if key == ' ':
-                    print('Stopping the stage!')
-                    self.ctrl.stage.stop()
-                    break
-                if key == 'q':
-                    self.ctrl.stage.stop()
-                    raise InterruptedError('Data collection was interrupted!')
-
-        t1 = time.perf_counter()
-        self.cam.stop_record()
-
-        if self.ctrl.beam.is_blanked:
-            self.ctrl.beam.blank()
-
-        self.end_position = self.ctrl.stage.get()
-        end_angle = self.end_position.a
-
-        self.t_start = t0
-        self.t_end = t1
-        self.total_time = t1 - t0
-
-        print('Waiting for DM to finish...')
-        while not self.cam.get_tag('finish_acquire'):
-            time.sleep(0.2)
-
-        self.gatan_readout = self.cam.readout()
-
-        self.nframes = nframes = self.gatan_readout['nframes']
-        if nframes < 1:
-            print('No frames measured??')
-            return
-
-        self.osc_angle = abs(end_angle - start_angle) / nframes
-
-        # acquisition_time = total_time / nframes
-        self.total_angle = abs(end_angle - start_angle)
-        self.rotation_axis = config.camera.camera_rotation_vs_stage_xy
-        self.camera_length = int(self.ctrl.magnification.get())
-        self.spotsize = self.ctrl.spotsize
-        self.rotation_speed = (end_angle - start_angle) / self.total_time
-        # self.exposure_time = self.cam.get_exposure()
-        self.start_angle, self.end_angle = start_angle, end_angle
-
-        self.log_end_status()
-        self.log_stage_positions()
-
-        print('Writing data files...')
-        path_data = self.path / 'tiff'
-        path_data.mkdir(exist_ok=True, parents=True)
-
-        if self.track:
-            # Center crystal position
-            if self.mode == 'diff':
-                self.ctrl.difffocus.defocus(self.defocus_offset)
-            self.ctrl.beam.unblank()
-
-            img2 = self.ctrl.get_rotated_image()
-            write_tiff(self.path / 'image_after.tiff', img2)
-
-            self.ctrl.beam.blank()
-            if self.mode == 'diff':
-                self.ctrl.difffocus.refocus()
-
-        print(f'Wrote {nframes} images to {path_data}')
-
-        if self.track:
-            print(f'Done with this crystal (number #{self.crystal_number})!')
-        else:
-            print('Done with this crystal!')
-
-    def log_end_status(self):
-        wavelength = config.microscope.wavelength
-
-        try:
-            pixelsize = config.calibration['diff']['pixelsize'][self.camera_length]  # px / Angstrom
-        except KeyError:
-            print(f'Warning: No such camera length: {self.camera_length} in diff calibration, defaulting to 1.0')
-            pixelsize = 1.0
-
-        physical_pixelsize = config.camera.physical_pixelsize  # mm
-
-        d = self.gatan_readout
-
-        bin_x, bin_y = d['bin_x'], d['bin_y']
-        image_dimensions_x, image_dimensions_y = d['image_res_x'], d['image_res_y']
-        camera_dimensions_x, camera_dimensions_y = d['cam_res_x'], d['cam_res_y']
-        assert bin_x == bin_y, 'Binnings differ in X and Y direction! (X: {bin_x} | Y: {bin_y})'
-        binning = bin_x
-
-        pixelsize *= binning
-        physical_pixelsize *= binning
-
-        print(f'\nRotated {self.total_angle:.2f} degrees from {self.start_angle:.2f} to {self.end_angle:.2f}')
-        print('Start stage position:  X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:6.1f} | B {:6.1f}'.format(*self.start_position))
-        print('End stage position:    X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:6.1f} | B {:6.1f}'.format(*self.end_position))
-        print(f'Data collection camera length: {self.camera_length} cm')
-        print(f'Data collection spot size: {self.spotsize}')
-        print(f'Rotation speed: {self.rotation_speed:.3f} degrees/s')
-
-        with open(self.path / 'cRED_log.txt', 'w') as f:
-            print(f'Program: {instamatic.__long_title__} + GMS {self.cam.getDMVersion()}', file=f)
-            print(f'Camera: {config.camera.name}', file=f)
-            print(f'Microscope: {config.microscope.name}', file=f)
-            # print(f"Camera type: {self.cam.getCameraType()}", file=f)
-            print(f'Mode: {self.mode}', file=f)
-            print(f'Data Collection Time: {self.now}', file=f)
-            print(f'Time Period Start: {self.t_start}', file=f)
-            print(f'Time Period End: {self.t_end}', file=f)
-            print(f'Number of frames: {self.nframes}', file=f)
-            print(f'Starting angle: {self.start_angle:.2f} degrees', file=f)
-            print(f'Ending angle: {self.end_angle:.2f} degrees', file=f)
-            print(f'Rotation range: {self.end_angle-self.start_angle:.2f} degrees', file=f)
-            print(f'Rotation speed: {self.rotation_speed:.3f} degrees/s', file=f)
-            # print(f"Exposure Time: {self.timings.exposure_time:.3f} s", file=f)
-            # print(f"Acquisition time: {self.timings.acquisition_time:.3f} s", file=f)
-            # print(f"Overhead time: {self.timings.overhead:.3f} s", file=f)
-            print(f'Total time: {self.total_time:.3f} s', file=f)
-            print(f'Wavelength: {wavelength} Angstrom', file=f)
-            print(f'Spot Size: {self.spotsize}', file=f)
-            print(f'Camera length: {self.camera_length} cm', file=f)
-            print(f'Pixelsize: {pixelsize} px/Angstrom', file=f)
-            print(f'Physical pixelsize: {physical_pixelsize} um', file=f)
-            print(f'Binning: {binning}', file=f)
-            print(f'Image dimensions: {image_dimensions_x} {image_dimensions_y}', file=f)
-            print(f'Camera dimensions: {camera_dimensions_x} {camera_dimensions_y}', file=f)
-            print(f'Stretch amplitude: {config.camera.stretch_azimuth} %', file=f)
-            print(f'Stretch azimuth: {config.camera.stretch_amplitude} degrees', file=f)
-            print(f'Rotation axis: {self.rotation_axis} radians', file=f)
-            print(f'Oscillation angle: {self.osc_angle:.4f} degrees', file=f)
-            print('Stage start: X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:8.2f} | B {:8.2f}'.format(*self.start_position), file=f)
-            print('Stage end: X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:8.2f} | B {:8.2f}'.format(*self.end_position), file=f)
-            # print("Beam stopper: yes", file=f)
-
-            if self.track:
-                print()
-                print(f'Crystal number: {self.crystal_number}', file=f)
-                print(f'Tracking data: {self.trackfile}', file=f)
-                print(f'Tracking between {self.min_angle} and {self.max_angle}', file=f)
-
-            print('', file=f)
-
-        print(f'Wrote file {f.name}')
-
-    def log_stage_positions(self):
-        fn = 'stage_positions(tracked).txt' if self.track else 'stage_positions.txt'
-        with open(self.path / fn, 'w') as f:
-            print('# timestamp x y z a b', file=f)
-            for t, (x, y, z, a, b) in self.stage_positions:
-                print(t, x, y, z, a, b, file=f)
-
-        print(f'Wrote file {f.name}')
-
-        if self.mode != 'diff':
-            if len(self.stage_positions) < 3:
-                print('Not enough stage positions for interpolation')
-            else:
-                pos = np.array([p[1] for p in self.stage_positions])  # (t, (x y z a b))
-                idx = np.argmin(np.abs(pos[:, 3]))
-                x_center = pos[:, 0].mean()
-                y_center = pos[idx, 1]
-                z_pos = pos[0:, 2].mean()
-                f = interp1d(pos[:, 3], pos[:, 1] - y_center, fill_value='extrapolate', kind='quadratic')
-
-                d = {}
-                d['y_offset'] = f
-                d['x_offset'] = 0
-                d['x_center'] = x_center
-                d['y_center'] = y_center
-                d['z_pos'] = z_pos
-
-                d['angle_min'] = self.start_angle
-                d['angle_max'] = self.end_angle
-
-                d['i'] = 0
-
-                fn = self.path / f'track.pickle'
-                pickle.dump(d, open(fn, 'wb'))
-
-                print(f'Wrote file {fn.name}')
-
-
-if __name__ == '__main__':
-    from instamatic import TEMController
-    from instamatic.io import get_new_work_subdirectory
-
-    print('Usage:')
-    print(' 1. Start `insteadmatic_module.s` in DM')
-    print(' 2. Run this script.')
-
-    ctrl = TEMController.initialize()
-
-    time.sleep(1)
-
-    expdir = get_new_work_subdirectory()
-    expdir.mkdir(exist_ok=True, parents=True)
-
-    exp = Experiment(ctrl=ctrl, path=expdir)
-    exp.get_ready()
-    exp.start_collection(100)
+import datetime
+import msvcrt
+import pickle
+import time
+from pathlib import Path
+
+import numpy as np
+from scipy.interpolate import interp1d
+
+import instamatic
+from instamatic import config
+from instamatic.formats import write_tiff
+
+
+class Experiment:
+    """Class to control data collection through DM to collect continuous
+    rotation electron diffraction data.
+
+    ctrl: `TEMController`
+        Instance of instamatic.TEMController.TEMController
+    path: str
+        `str` or `pathlib.Path` object giving the path to save data at
+    log: `logging.Logger`
+        Instance of `logging.Logger`
+    exposure: float
+        Exposure time in ms
+    mode: str
+    """
+
+    def __init__(self, ctrl,
+                 path: str = None,
+                 log=None,
+                 track: str = None,
+                 exposure: float = 400,
+                 mode: str = 'diff',
+                 rotation_speed: int = None):
+        super().__init__()
+
+        self.ctrl = ctrl
+        self.cam = ctrl.cam
+        self.path = Path(path)
+
+        self.exposure = exposure
+        self.defocus_offset = 1500
+
+        self.logger = log
+        self.mode = mode
+
+        self.rotation_speed = rotation_speed
+
+        if track:
+            self.load_tracking_file(track)
+            self.track = True
+        else:
+            self.track = False
+
+    def load_tracking_file(self, trackfile):
+        trackfile = Path(trackfile)
+        if trackfile.suffix == '.pickle':
+            print(f'(autotracking) Loading tracking file: {trackfile}')
+            dct = pickle.load(open(trackfile, 'rb'))
+
+            self.track_func = dct['y_offset']
+            self.x_offset = dct['x_offset']
+            self.start_x = dct['x_center']
+            self.start_y = dct['y_center']
+            self.start_z = dct['z_pos']
+
+            self.min_angle = dct['angle_min']
+            self.max_angle = dct['angle_max']
+
+            self.crystal_number = dct['i']
+
+            self.trackfile = trackfile
+
+            self.track_interval = 2
+            self.track_relative = False
+
+        else:
+            raise OSError("I don't know how to read file `{trackfile}`")
+
+    def prepare_tracking(self):
+        if self.track:
+            current_angle = self.ctrl.stage.a
+
+            min_angle = self.min_angle
+            max_angle = self.max_angle
+
+            # find start angle closest to current angle
+            if abs(min_angle - current_angle) > abs(max_angle - current_angle):
+                start_angle, target_angle = max_angle, min_angle
+            else:
+                start_angle, target_angle = min_angle, max_angle
+
+            print(f'(autotracking) Overriding angle range: {start_angle:.0f} -> {target_angle:.0f}')
+
+            y_offset = int(self.track_func(start_angle))
+            x_offset = self.x_offset
+
+            print(f'(autotracking) setting a={start_angle:.0f}, x={self.start_x+x_offset:.0f}, y={self.start_y+y_offset:.0f}, z={self.start_z:.0f}')
+            self.ctrl.stage.set_xy_with_backlash_correction(x=self.start_x + x_offset, y=self.start_y + y_offset, step=10000)
+            self.ctrl.stage.set(a=start_angle, z=self.start_z)
+
+            return start_angle, target_angle
+
+    def track_crystal(self, n, angle):
+        # tracking routine
+        if (n % self.track_interval == 0):
+            target_y = self.start_y + int(self.track_func(angle))
+            self.ctrl.stage.set(y=target_y, wait=False)
+            print(f'(autotracking) set y={target_y:.0f}')
+
+    def get_ready(self):
+        # self.cam.set_exposure(self.exposure)
+
+        if not self.ctrl.beam.is_blanked:
+            self.ctrl.beam.blank()
+
+        self.ctrl.screen.up()
+
+        if self.ctrl.mode != self.mode:
+            print(f'Switching to {self.mode} mode')
+            self.ctrl.mode.set(self.mode)
+
+        if self.mode == 'diff':
+            self.ctrl.difffocus.refocus()
+
+        spotsize = self.ctrl.spotsize
+
+        self.cam.set_tag('exp_directory', str(self.path))
+        self.cam.get_ready_for_record()
+        print('Ready...')
+
+    def manual_activation(self) -> float:
+        ACTIVATION_THRESHOLD = 0.2
+
+        print('Waiting for rotation to start...', end=' ')
+        a0 = a = self.ctrl.stage.a
+        while abs(a - a0) < ACTIVATION_THRESHOLD:
+            a = self.ctrl.stage.a
+
+        print('Rotation started...')
+
+        return a
+
+    def start_collection(self, target_angle: float, start_angle: float = None, manual_control: bool = False):
+        """
+        manual_control : bool
+            Control the rotation using the buttons or pedals
+        """
+        angle_tolerance = 0.5  # degrees
+
+        self.now = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+
+        self.stage_positions = []
+        interval = 0.7  # interval at which it check for rotation to end / does tracking
+
+        if self.track:
+            start_angle, target_angle = self.prepare_tracking()
+
+        if start_angle:
+            print(f'Going to starting angle: {start_angle:.1f}')
+            self.ctrl.stage.a = start_angle
+
+        self.start_position = self.ctrl.stage.get()
+        start_angle = self.start_position.a
+
+        if self.track:
+            # Center crystal position
+            if self.mode == 'diff':
+                self.ctrl.difffocus.defocus(self.defocus_offset)
+            self.ctrl.beam.unblank()
+
+            input('Move SAED aperture to crystal and press <ENTER> to measure! ')
+
+            # cannot do this while lieview is running
+            # img1 = self.ctrl.get_raw_image()
+            # write_tiff(self.path / "image_before.tiff", img1)
+
+            self.ctrl.beam.blank()
+            if self.mode == 'diff':
+                self.ctrl.difffocus.refocus()
+            time.sleep(3)
+
+        self.ctrl.beam.unblank()(delay=0.2)  # give the beamblank some time to dissappear to avoid weak first frame
+
+        if manual_control:
+            start_angle = self.manual_activation()
+            last_angle = 999
+        elif self.rotation_speed:
+            self.ctrl.stage.set_a_with_speed(a=target_angle, speed=self.rotation_speed, wait=False)
+        else:
+            self.ctrl.stage.set(a=target_angle, wait=False)
+
+        self.cam.start_record()  # start recording
+
+        t0 = time.perf_counter()
+        t_delta = t0
+
+        n = 0
+
+        print('Acquiring data...')
+
+        while True:
+            t = time.perf_counter()
+
+            if not manual_control:
+                if abs(self.ctrl.stage.a - target_angle) < angle_tolerance:
+                    print('Target angle reached!')
+                    break
+
+            if t - t_delta > interval:
+
+                n += 1
+                x, y, z, a, _ = pos = self.ctrl.stage.get()
+                self.stage_positions.append((t, pos))
+                t_delta = t
+                # print(t, pos)
+
+                if manual_control:
+                    current_angle = a
+                    if last_angle == current_angle:
+                        print(f'Manual rotation was interrupted (current: {current_angle:.2f} | last {last_angle:.2f})')
+                        break
+                    last_angle = current_angle
+
+                    print(f' >> Current angle: {a:.2f}', end='      \r')
+
+                if self.track:
+                    self.track_crystal(n=n, angle=a)
+
+            # Stop/interrupt and go to next crystal
+            if msvcrt.kbhit():
+                key = msvcrt.getch().decode()
+                if key == ' ':
+                    print('Stopping the stage!')
+                    self.ctrl.stage.stop()
+                    break
+                if key == 'q':
+                    self.ctrl.stage.stop()
+                    raise InterruptedError('Data collection was interrupted!')
+
+        t1 = time.perf_counter()
+        self.cam.stop_record()
+
+        if self.ctrl.beam.is_blanked:
+            self.ctrl.beam.blank()
+
+        self.end_position = self.ctrl.stage.get()
+        end_angle = self.end_position.a
+
+        self.t_start = t0
+        self.t_end = t1
+        self.total_time = t1 - t0
+
+        print('Waiting for DM to finish...')
+        while not self.cam.get_tag('finish_acquire'):
+            time.sleep(0.2)
+
+        self.gatan_readout = self.cam.readout()
+
+        self.nframes = nframes = self.gatan_readout['nframes']
+        if nframes < 1:
+            print('No frames measured??')
+            return
+
+        self.osc_angle = abs(end_angle - start_angle) / nframes
+
+        # acquisition_time = total_time / nframes
+        self.total_angle = abs(end_angle - start_angle)
+        self.rotation_axis = config.camera.camera_rotation_vs_stage_xy
+        self.camera_length = int(self.ctrl.magnification.get())
+        self.spotsize = self.ctrl.spotsize
+        self.rotation_speed = (end_angle - start_angle) / self.total_time
+        # self.exposure_time = self.cam.get_exposure()
+        self.start_angle, self.end_angle = start_angle, end_angle
+
+        self.log_end_status()
+        self.log_stage_positions()
+
+        print('Writing data files...')
+        path_data = self.path / 'tiff'
+        path_data.mkdir(exist_ok=True, parents=True)
+
+        if self.track:
+            # Center crystal position
+            if self.mode == 'diff':
+                self.ctrl.difffocus.defocus(self.defocus_offset)
+            self.ctrl.beam.unblank()
+
+            img2 = self.ctrl.get_rotated_image()
+            write_tiff(self.path / 'image_after.tiff', img2)
+
+            self.ctrl.beam.blank()
+            if self.mode == 'diff':
+                self.ctrl.difffocus.refocus()
+
+        print(f'Wrote {nframes} images to {path_data}')
+
+        if self.track:
+            print(f'Done with this crystal (number #{self.crystal_number})!')
+        else:
+            print('Done with this crystal!')
+
+    def log_end_status(self):
+        wavelength = config.microscope.wavelength
+
+        try:
+            pixelsize = config.calibration['diff']['pixelsize'][self.camera_length]  # px / Angstrom
+        except KeyError:
+            print(f'Warning: No such camera length: {self.camera_length} in diff calibration, defaulting to 1.0')
+            pixelsize = 1.0
+
+        physical_pixelsize = config.camera.physical_pixelsize  # mm
+
+        d = self.gatan_readout
+
+        bin_x, bin_y = d['bin_x'], d['bin_y']
+        image_dimensions_x, image_dimensions_y = d['image_res_x'], d['image_res_y']
+        camera_dimensions_x, camera_dimensions_y = d['cam_res_x'], d['cam_res_y']
+        assert bin_x == bin_y, 'Binnings differ in X and Y direction! (X: {bin_x} | Y: {bin_y})'
+        binning = bin_x
+
+        pixelsize *= binning
+        physical_pixelsize *= binning
+
+        print(f'\nRotated {self.total_angle:.2f} degrees from {self.start_angle:.2f} to {self.end_angle:.2f}')
+        print('Start stage position:  X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:6.1f} | B {:6.1f}'.format(*self.start_position))
+        print('End stage position:    X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:6.1f} | B {:6.1f}'.format(*self.end_position))
+        print(f'Data collection camera length: {self.camera_length} cm')
+        print(f'Data collection spot size: {self.spotsize}')
+        print(f'Rotation speed: {self.rotation_speed:.3f} degrees/s')
+
+        with open(self.path / 'cRED_log.txt', 'w') as f:
+            print(f'Program: {instamatic.__long_title__} + GMS {self.cam.getDMVersion()}', file=f)
+            print(f'Camera: {config.camera.name}', file=f)
+            print(f'Microscope: {config.microscope.name}', file=f)
+            # print(f"Camera type: {self.cam.getCameraType()}", file=f)
+            print(f'Mode: {self.mode}', file=f)
+            print(f'Data Collection Time: {self.now}', file=f)
+            print(f'Time Period Start: {self.t_start}', file=f)
+            print(f'Time Period End: {self.t_end}', file=f)
+            print(f'Number of frames: {self.nframes}', file=f)
+            print(f'Starting angle: {self.start_angle:.2f} degrees', file=f)
+            print(f'Ending angle: {self.end_angle:.2f} degrees', file=f)
+            print(f'Rotation range: {self.end_angle-self.start_angle:.2f} degrees', file=f)
+            print(f'Rotation speed: {self.rotation_speed:.3f} degrees/s', file=f)
+            # print(f"Exposure Time: {self.timings.exposure_time:.3f} s", file=f)
+            # print(f"Acquisition time: {self.timings.acquisition_time:.3f} s", file=f)
+            # print(f"Overhead time: {self.timings.overhead:.3f} s", file=f)
+            print(f'Total time: {self.total_time:.3f} s', file=f)
+            print(f'Wavelength: {wavelength} Angstrom', file=f)
+            print(f'Spot Size: {self.spotsize}', file=f)
+            print(f'Camera length: {self.camera_length} cm', file=f)
+            print(f'Pixelsize: {pixelsize} px/Angstrom', file=f)
+            print(f'Physical pixelsize: {physical_pixelsize} um', file=f)
+            print(f'Binning: {binning}', file=f)
+            print(f'Image dimensions: {image_dimensions_x} {image_dimensions_y}', file=f)
+            print(f'Camera dimensions: {camera_dimensions_x} {camera_dimensions_y}', file=f)
+            print(f'Stretch amplitude: {config.camera.stretch_azimuth} %', file=f)
+            print(f'Stretch azimuth: {config.camera.stretch_amplitude} degrees', file=f)
+            print(f'Rotation axis: {self.rotation_axis} radians', file=f)
+            print(f'Oscillation angle: {self.osc_angle:.4f} degrees', file=f)
+            print('Stage start: X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:8.2f} | B {:8.2f}'.format(*self.start_position), file=f)
+            print('Stage end: X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:8.2f} | B {:8.2f}'.format(*self.end_position), file=f)
+            # print("Beam stopper: yes", file=f)
+
+            if self.track:
+                print()
+                print(f'Crystal number: {self.crystal_number}', file=f)
+                print(f'Tracking data: {self.trackfile}', file=f)
+                print(f'Tracking between {self.min_angle} and {self.max_angle}', file=f)
+
+            print('', file=f)
+
+        print(f'Wrote file {f.name}')
+
+    def log_stage_positions(self):
+        fn = 'stage_positions(tracked).txt' if self.track else 'stage_positions.txt'
+        with open(self.path / fn, 'w') as f:
+            print('# timestamp x y z a b', file=f)
+            for t, (x, y, z, a, b) in self.stage_positions:
+                print(t, x, y, z, a, b, file=f)
+
+        print(f'Wrote file {f.name}')
+
+        if self.mode != 'diff':
+            if len(self.stage_positions) < 3:
+                print('Not enough stage positions for interpolation')
+            else:
+                pos = np.array([p[1] for p in self.stage_positions])  # (t, (x y z a b))
+                idx = np.argmin(np.abs(pos[:, 3]))
+                x_center = pos[:, 0].mean()
+                y_center = pos[idx, 1]
+                z_pos = pos[0:, 2].mean()
+                f = interp1d(pos[:, 3], pos[:, 1] - y_center, fill_value='extrapolate', kind='quadratic')
+
+                d = {}
+                d['y_offset'] = f
+                d['x_offset'] = 0
+                d['x_center'] = x_center
+                d['y_center'] = y_center
+                d['z_pos'] = z_pos
+
+                d['angle_min'] = self.start_angle
+                d['angle_max'] = self.end_angle
+
+                d['i'] = 0
+
+                fn = self.path / 'track.pickle'
+                pickle.dump(d, open(fn, 'wb'))
+
+                print(f'Wrote file {fn.name}')
+
+
+if __name__ == '__main__':
+    from instamatic import TEMController
+    from instamatic.io import get_new_work_subdirectory
+
+    print('Usage:')
+    print(' 1. Start `insteadmatic_module.s` in DM')
+    print(' 2. Run this script.')
+
+    ctrl = TEMController.initialize()
+
+    time.sleep(1)
+
+    expdir = get_new_work_subdirectory()
+    expdir.mkdir(exist_ok=True, parents=True)
+
+    exp = Experiment(ctrl=ctrl, path=expdir)
+    exp.get_ready()
+    exp.start_collection(100)
```

### Comparing `instamatic-1.8.0/instamatic/experiments/cred_tvips/experiment.py` & `instamatic-1.9.0/instamatic/experiments/cred_tvips/experiment.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,575 +1,575 @@
-import datetime
-import msvcrt
-import pickle
-import time
-from pathlib import Path
-
-import numpy as np
-from pyserialem import read_nav_file
-from scipy.interpolate import interp1d
-
-import instamatic
-from instamatic import config
-from instamatic.formats import write_tiff
-from instamatic.tools import get_acquisition_time
-
-
-class SerialExperiment:
-    """Class to handle serial red data acquisition using a TVIPS camera."""
-
-    def __init__(self, ctrl,
-                 path: str = None,
-                 log=None,
-                 instruction_file: str = None,
-                 exposure: float = 400,
-                 mode: str = 'diff',
-                 target_angle: float = 40,
-                 rotation_speed=None):
-        super().__init__()
-
-        self.instruction_file = Path(instruction_file)
-        self.base_drc = self.instruction_file.parent
-
-        if self.instruction_file.suffix == '.nav':
-            self.nav_items = read_nav_file(self.instruction_file, acquire_only=True)
-            self.run = self.run_from_nav_file
-            self.start_angle = target_angle / 2
-            self.end_angle = -self.start_angle
-        else:
-            self.tracks = open(self.instruction_file, 'r').readlines()
-            self.run = self.run_from_tracking_file
-
-        self.log = log
-        self.path = path
-        self.ctrl = ctrl
-        self.exposure = exposure
-        self.mode = mode
-        self.rotation_speed = rotation_speed
-
-    def run(self):
-        raise RuntimeError(f'`{self.__class__.__name__}` has not been initialized.')
-
-    def run_from_nav_file(self):
-        """Run serial RED on all the coordinates from the `.nav` file."""
-        start_angle = self.start_angle
-        end_angle = self.end_angle
-        path = self.path
-        mode = self.mode
-        log = self.log
-        exposure = self.exposure
-
-        if self.rotation_speed:
-            self.ctrl.stage.set_rotation_speed(self.rotation_speed)
-
-        def go_to_first_position(ctrl):
-            ctrl.stage.set(a=start_angle)
-
-        def acquire_cred_data(ctrl):
-            nonlocal start_angle
-            nonlocal end_angle
-
-            tag = ctrl.current_item.tag
-            out_path = path / tag
-
-            out_path.mkdir(exist_ok=True, parents=True)
-
-            print()
-            print(f'Data directory: {out_path}')
-            print(f'Rotating from {start_angle} to {end_angle} degrees')
-            print(ctrl.stage)
-
-            exp = Experiment(ctrl, path=out_path, log=log, exposure=exposure, mode=mode)
-            exp.get_ready()
-            exp.start_collection(target_angle=end_angle, start_angle=start_angle)
-
-            start_angle, end_angle = end_angle, start_angle
-
-        def stop_liveview(ctrl):
-            ctrl.cam.stop_liveview()
-
-        self.ctrl.acquire_at_items(self.nav_items,
-                                   acquire=acquire_cred_data,
-                                   pre_acquire=go_to_first_position,
-                                   post_acquire=stop_liveview)
-
-        if self.rotation_speed:
-            self.ctrl.stage.set_rotation_speed(12)
-
-    def run_from_tracking_file(self):
-        t0 = time.perf_counter()
-        n_measured = 0
-
-        n_items = len(self.tracks)
-
-        for i, track in enumerate(self.tracks):
-            track = track.strip()
-            if not track:
-                continue
-
-            track = self.base_drc / track
-            name = track.name
-            stem = track.stem
-
-            out_path = self.path / stem
-            out_path.mkdir(exist_ok=True, parents=True)
-
-            print()
-            print(f'({i} / {n_items}) Acquiring track: {stem}')
-            print(f'Track file: {self.base_drc / name}')
-            print(f'Data directory: {out_path}')
-            print(self.ctrl.stage)
-            print()
-
-            exp = Experiment(self.ctrl, path=out_path, log=self.log, track=track, exposure=self.exposure, mode=self.mode)
-
-            exp.get_ready()
-
-            try:
-                exp.start_collection(target_angle=0)
-            except InterruptedError:
-                self.ctrl.cam.stop_liveview()
-                break
-            finally:
-                del exp
-
-            n_measured += 1
-
-            time.sleep(3)
-
-        t1 = time.perf_counter()
-        dt = t1 - t0
-        print(f'Serial experiment finished -> {n_measured} crystals measured')
-        print(f'Time taken: {dt:.1f} s, {dt/n_measured:.1f} s/crystal')
-        print(f'Data directory: {self.path}')
-
-
-class Experiment:
-    """Class to control data collection through EMMenu to collect continuous
-    rotation electron diffraction data.
-
-    ctrl: `TEMController`
-        Instance of instamatic.TEMController.TEMController
-    path: str
-        `str` or `pathlib.Path` object giving the path to save data at
-    log: `logging.Logger`
-        Instance of `logging.Logger`
-    exposure: float
-        Exposure time in ms
-    mode: str
-    """
-
-    def __init__(self, ctrl,
-                 path: str = None,
-                 log=None,
-                 track: str = None,
-                 exposure: float = 400,
-                 mode: str = 'diff',
-                 rotation_speed: int = None):
-        super().__init__()
-
-        self.ctrl = ctrl
-        self.emmenu = ctrl.cam
-        self.path = Path(path)
-
-        self.exposure = exposure
-        self.defocus_offset = 1500
-
-        self.logger = log
-        self.mode = mode
-
-        self.rotation_speed = rotation_speed
-
-        if track:
-            self.load_tracking_file(track)
-            self.track = True
-        else:
-            self.track = False
-
-    def load_tracking_file(self, trackfile):
-        trackfile = Path(trackfile)
-        if trackfile.suffix == '.pickle':
-            print(f'(autotracking) Loading tracking file: {trackfile}')
-            dct = pickle.load(open(trackfile, 'rb'))
-
-            self.track_func = dct['y_offset']
-            self.x_offset = dct['x_offset']
-            self.start_x = dct['x_center']
-            self.start_y = dct['y_center']
-            self.start_z = dct['z_pos']
-
-            self.min_angle = dct['angle_min']
-            self.max_angle = dct['angle_max']
-
-            self.crystal_number = dct['i']
-
-            self.trackfile = trackfile
-
-            self.track_interval = 2
-            self.track_relative = False
-
-        else:
-            raise OSError("I don't know how to read file `{trackfile}`")
-
-    def prepare_tracking(self):
-        if self.track:
-            current_angle = self.ctrl.stage.a
-
-            min_angle = self.min_angle
-            max_angle = self.max_angle
-
-            # find start angle closest to current angle
-            if abs(min_angle - current_angle) > abs(max_angle - current_angle):
-                start_angle, target_angle = max_angle, min_angle
-            else:
-                start_angle, target_angle = min_angle, max_angle
-
-            print(f'(autotracking) Overriding angle range: {start_angle:.0f} -> {target_angle:.0f}')
-
-            y_offset = int(self.track_func(start_angle))
-            x_offset = self.x_offset
-
-            print(f'(autotracking) setting a={start_angle:.0f}, x={self.start_x+x_offset:.0f}, y={self.start_y+y_offset:.0f}, z={self.start_z:.0f}')
-            self.ctrl.stage.set_xy_with_backlash_correction(x=self.start_x + x_offset, y=self.start_y + y_offset, step=10000)
-            self.ctrl.stage.set(a=start_angle, z=self.start_z)
-
-            return start_angle, target_angle
-
-    def track_crystal(self, n, angle):
-        # tracking routine
-        if (n % self.track_interval == 0):
-            target_y = self.start_y + int(self.track_func(angle))
-            self.ctrl.stage.set(y=target_y, wait=False)
-            print(f'(autotracking) set y={target_y:.0f}')
-
-    def get_ready(self):
-        self.emmenu.stop_liveview()  # just in case
-
-        try:
-            # next 2 lines are a workaround for EMMENU 5.0.9.0 bugs, FIXME later
-            self.emmenu.set_autoincrement(False)
-            self.emmenu.set_image_index(0)
-        except Exception as e:
-            print(e)
-
-        self.emmenu.set_exposure(self.exposure)
-
-        if not self.ctrl.beam.is_blanked:
-            self.ctrl.beam.blank()
-
-        self.ctrl.screen.up()
-
-        if self.ctrl.mode != self.mode:
-            print(f'Switching to {self.mode} mode')
-            self.ctrl.mode.set(self.mode)
-
-        if self.mode == 'diff':
-            self.ctrl.difffocus.refocus()
-
-        self.emmenu.start_liveview()
-
-        print('Ready...')
-
-    def manual_activation(self) -> float:
-        ACTIVATION_THRESHOLD = 0.2
-
-        print('Waiting for rotation to start...', end=' ')
-        a0 = a = self.ctrl.stage.a
-        while abs(a - a0) < ACTIVATION_THRESHOLD:
-            a = self.ctrl.stage.a
-
-        print('Rotation started...')
-
-        return a
-
-    def start_collection(self, target_angle: float, start_angle: float = None, manual_control: bool = False):
-        """
-        manual_control : bool
-            Control the rotation using the buttons or pedals
-        """
-        angle_tolerance = 0.5  # degrees
-
-        self.now = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-
-        self.stage_positions = []
-        interval = 0.7  # interval at which it check for rotation to end / does tracking
-
-        if self.track:
-            start_angle, target_angle = self.prepare_tracking()
-
-        if start_angle:
-            print(f'Going to starting angle: {start_angle:.1f}')
-            self.ctrl.stage.a = start_angle
-
-        self.start_position = self.ctrl.stage.get()
-        start_angle = self.start_position.a
-
-        if self.track:
-            # Center crystal position
-            if self.mode == 'diff':
-                self.ctrl.difffocus.defocus(self.defocus_offset)
-            self.ctrl.beam.unblank()
-
-            input('Move SAED aperture to crystal and press <ENTER> to measure! ')
-
-            # cannot do this while lieview is running
-            # img1 = self.ctrl.get_rotated_image()
-            # write_tiff(self.path / "image_before.tiff", img1)
-
-            self.ctrl.beam.blank()
-            if self.mode == 'diff':
-                self.ctrl.difffocus.refocus()
-            time.sleep(3)
-
-        self.ctrl.beam.unblank(delay=0.2)  # give the beamblank some time to dissappear to avoid weak first frame
-
-        # with autoincrement(False), otherwise use `get_next_empty_image_index()`
-        # start_index is set to 1, because EMMENU always takes a single image (0) when liveview is activated
-        start_index = 1
-        # start_index = self.emmenu.get_next_empty_image_index()
-
-        if manual_control:
-            start_angle = self.manual_activation()
-            last_angle = 999
-        elif self.rotation_speed:
-            self.ctrl.stage.set_a_with_speed(a=target_angle, speed=self.rotation_speed, wait=False)
-        else:
-            self.ctrl.stage.set(a=target_angle, wait=False)
-
-        self.emmenu.start_record()  # start recording
-
-        t0 = time.perf_counter()
-        t_delta = t0
-
-        n = 0
-
-        print('Acquiring data...')
-
-        while True:
-            t = time.perf_counter()
-
-            if not manual_control:
-                if abs(self.ctrl.stage.a - target_angle) < angle_tolerance:
-                    print('Target angle reached!')
-                    break
-
-            if t - t_delta > interval:
-
-                n += 1
-                x, y, z, a, _ = pos = self.ctrl.stage.get()
-                self.stage_positions.append((t, pos))
-                t_delta = t
-                # print(t, pos)
-
-                if manual_control:
-                    current_angle = a
-                    if last_angle == current_angle:
-                        print(f'Manual rotation was interrupted (current: {current_angle:.2f} | last {last_angle:.2f})')
-                        break
-                    last_angle = current_angle
-
-                    print(f' >> Current angle: {a:.2f}', end='      \r')
-
-                if self.track:
-                    self.track_crystal(n=n, angle=a)
-
-            # Stop/interrupt and go to next crystal
-            if msvcrt.kbhit():
-                key = msvcrt.getch().decode()
-                if key == ' ':
-                    print('Stopping the stage!')
-                    self.ctrl.stage.stop()
-                    break
-                if key == 'q':
-                    self.ctrl.stage.stop()
-                    raise InterruptedError('Data collection was interrupted!')
-
-        t1 = time.perf_counter()
-        self.emmenu.stop_liveview()
-
-        if self.ctrl.beam.is_blanked:
-            self.ctrl.beam.blank()
-
-        self.end_position = self.ctrl.stage.get()
-        end_angle = self.end_position.a
-
-        end_index = self.emmenu.get_image_index()
-
-        self.t_start = t0
-        self.t_end = t1
-        self.total_time = t1 - t0
-
-        self.nframes = nframes = end_index - start_index + 1
-        if nframes < 1:
-            print('No frames measured??')
-            return
-
-        self.osc_angle = abs(end_angle - start_angle) / nframes
-
-        # acquisition_time = total_time / nframes
-        self.total_angle = abs(end_angle - start_angle)
-        self.rotation_axis = config.camera.camera_rotation_vs_stage_xy
-        self.camera_length = int(self.ctrl.magnification.get())
-        self.spotsize = self.ctrl.spotsize
-        self.rotation_speed = (end_angle - start_angle) / self.total_time
-        self.exposure_time = self.emmenu.get_exposure()
-        self.start_angle, self.end_angle = start_angle, end_angle
-
-        try:
-            # sometimes breaks with:
-            # AttributeError: 'NoneType' object has no attribute 'EMVector'
-            timestamps = self.emmenu.get_timestamps(start_index, end_index)
-        except AttributeError as e:
-            print(e)
-            print(f'Timestamps from {start_index} to {end_index}')
-            timestamps = [1, 2, 3, 4, 5]  # just to make it work
-
-        self.timings = get_acquisition_time(timestamps, exp_time=self.exposure_time, savefig=True, drc=self.path)
-
-        self.log_end_status()
-        self.log_stage_positions()
-
-        print('Writing data files...')
-        path_data = self.path / 'tiff'
-        path_data.mkdir(exist_ok=True, parents=True)
-
-        self.emmenu.writeTiffs(start_index, end_index, path=path_data)
-
-        if self.track:
-            # Center crystal position
-            if self.mode == 'diff':
-                self.ctrl.difffocus.defocus(self.defocus_offset)
-            self.ctrl.beam.unblank()
-
-            img2 = self.ctrl.get_rotated_image()
-            write_tiff(self.path / 'image_after.tiff', img2)
-
-            self.ctrl.beam.blank()
-            if self.mode == 'diff':
-                self.ctrl.difffocus.refocus()
-
-        print(f'Wrote {nframes} images (#{start_index}->#{end_index}) to {path_data}')
-
-        if self.track:
-            print(f'Done with this crystal (number #{self.crystal_number})!')
-        else:
-            print('Done with this crystal!')
-
-    def log_end_status(self):
-        wavelength = config.microscope.wavelength
-
-        try:
-            pixelsize = config.calibration['diff']['pixelsize'][self.camera_length]  # px / Angstrom
-        except KeyError:
-            print(f'Warning: No such camera length: {self.camera_length} in diff calibration, defaulting to 1.0')
-            pixelsize = 1.0
-
-        physical_pixelsize = config.camera.physical_pixelsize  # mm
-
-        binning = self.emmenu.getBinning()
-        image_dimensions_x, image_dimensions_y = self.emmenu.getImageDimensions()
-        camera_dimensions_x, camera_dimensions_y = self.emmenu.getCameraDimensions()
-
-        pixelsize *= binning
-        physical_pixelsize *= binning
-
-        print(f'\nRotated {self.total_angle:.2f} degrees from {self.start_angle:.2f} to {self.end_angle:.2f}')
-        print('Start stage position:  X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:6.1f} | B {:6.1f}'.format(*self.start_position))
-        print('End stage position:    X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:6.1f} | B {:6.1f}'.format(*self.end_position))
-        print(f'Data collection camera length: {self.camera_length} cm')
-        print(f'Data collection spot size: {self.spotsize}')
-        print(f'Rotation speed: {self.rotation_speed:.3f} degrees/s')
-
-        with open(self.path / 'cRED_log.txt', 'w') as f:
-            print(f'Program: {instamatic.__long_title__} + EMMenu {self.emmenu.getEMMenuVersion()}', file=f)
-            print(f'Camera: {config.camera.name}', file=f)
-            print(f'Microscope: {config.microscope.name}', file=f)
-            print(f'Camera type: {self.emmenu.getCameraType()}', file=f)
-            print(f'Camera config: {self.emmenu.getCurrentConfigName()}', file=f)
-            print(f'Mode: {self.mode}', file=f)
-            print(f'Data Collection Time: {self.now}', file=f)
-            print(f'Time Period Start: {self.t_start}', file=f)
-            print(f'Time Period End: {self.t_end}', file=f)
-            print(f'Number of frames: {self.nframes}', file=f)
-            print(f'Starting angle: {self.start_angle:.2f} degrees', file=f)
-            print(f'Ending angle: {self.end_angle:.2f} degrees', file=f)
-            print(f'Rotation range: {self.end_angle-self.start_angle:.2f} degrees', file=f)
-            print(f'Rotation speed: {self.rotation_speed:.3f} degrees/s', file=f)
-            print(f'Exposure Time: {self.timings.exposure_time:.3f} s', file=f)
-            print(f'Acquisition time: {self.timings.acquisition_time:.3f} s', file=f)
-            print(f'Overhead time: {self.timings.overhead:.3f} s', file=f)
-            print(f'Total time: {self.total_time:.3f} s', file=f)
-            print(f'Wavelength: {wavelength} Angstrom', file=f)
-            print(f'Spot Size: {self.spotsize}', file=f)
-            print(f'Camera length: {self.camera_length} cm', file=f)
-            print(f'Pixelsize: {pixelsize} px/Angstrom', file=f)
-            print(f'Physical pixelsize: {physical_pixelsize} um', file=f)
-            print(f'Binning: {binning}', file=f)
-            print(f'Image dimensions: {image_dimensions_x} {image_dimensions_y}', file=f)
-            print(f'Camera dimensions: {camera_dimensions_x} {camera_dimensions_y}', file=f)
-            print(f'Stretch amplitude: {config.camera.stretch_azimuth} %', file=f)
-            print(f'Stretch azimuth: {config.camera.stretch_amplitude} degrees', file=f)
-            print(f'Rotation axis: {self.rotation_axis} radians', file=f)
-            print(f'Oscillation angle: {self.osc_angle:.4f} degrees', file=f)
-            print('Stage start: X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:8.2f} | B {:8.2f}'.format(*self.start_position), file=f)
-            print('Beam stopper: yes', file=f)
-
-            if self.track:
-                print()
-                print(f'Crystal number: {self.crystal_number}', file=f)
-                print(f'Tracking data: {self.trackfile}', file=f)
-                print(f'Tracking between {self.min_angle} and {self.max_angle}', file=f)
-
-            print('', file=f)
-
-        print(f'Wrote file {f.name}')
-
-    def log_stage_positions(self):
-        fn = 'stage_positions(tracked).txt' if self.track else 'stage_positions.txt'
-        with open(self.path / fn, 'w') as f:
-            print('# timestamp x y z a b', file=f)
-            for t, (x, y, z, a, b) in self.stage_positions:
-                print(t, x, y, z, a, b, file=f)
-
-        print(f'Wrote file {f.name}')
-
-        if self.mode != 'diff':
-            if len(self.stage_positions) < 3:
-                print('Not enough stage positions for interpolation')
-            else:
-                pos = np.array([p[1] for p in self.stage_positions])  # (t, (x y z a b))
-                idx = np.argmin(np.abs(pos[:, 3]))
-                x_center = pos[:, 0].mean()
-                y_center = pos[idx, 1]
-                z_pos = pos[0:, 2].mean()
-                f = interp1d(pos[:, 3], pos[:, 1] - y_center, fill_value='extrapolate', kind='quadratic')
-
-                d = {}
-                d['y_offset'] = f
-                d['x_offset'] = 0
-                d['x_center'] = x_center
-                d['y_center'] = y_center
-                d['z_pos'] = z_pos
-
-                d['angle_min'] = self.start_angle
-                d['angle_max'] = self.end_angle
-
-                d['i'] = 0
-
-                fn = self.path / f'track.pickle'
-                pickle.dump(d, open(fn, 'wb'))
-
-                print(f'Wrote file {fn.name}')
-
-
-if __name__ == '__main__':
-    from instamatic.io import get_new_work_subdirectory
-    from instamatic import TEMController
-
-    ctrl = TEMController.initialize()
-
-    expdir = get_new_work_subdirectory()
-    expdir.mkdir(exist_ok=True, parents=True)
-
-    exp = Experiment(ctrl, path=expdir)
-    exp.get_ready()
-    exp.run(target_angle=20)
+import datetime
+import msvcrt
+import pickle
+import time
+from pathlib import Path
+
+import numpy as np
+from pyserialem import read_nav_file
+from scipy.interpolate import interp1d
+
+import instamatic
+from instamatic import config
+from instamatic.formats import write_tiff
+from instamatic.tools import get_acquisition_time
+
+
+class SerialExperiment:
+    """Class to handle serial red data acquisition using a TVIPS camera."""
+
+    def __init__(self, ctrl,
+                 path: str = None,
+                 log=None,
+                 instruction_file: str = None,
+                 exposure: float = 400,
+                 mode: str = 'diff',
+                 target_angle: float = 40,
+                 rotation_speed=None):
+        super().__init__()
+
+        self.instruction_file = Path(instruction_file)
+        self.base_drc = self.instruction_file.parent
+
+        if self.instruction_file.suffix == '.nav':
+            self.nav_items = read_nav_file(self.instruction_file, acquire_only=True)
+            self.run = self.run_from_nav_file
+            self.start_angle = target_angle / 2
+            self.end_angle = -self.start_angle
+        else:
+            self.tracks = open(self.instruction_file).readlines()
+            self.run = self.run_from_tracking_file
+
+        self.log = log
+        self.path = path
+        self.ctrl = ctrl
+        self.exposure = exposure
+        self.mode = mode
+        self.rotation_speed = rotation_speed
+
+    def run(self):
+        raise RuntimeError(f'`{self.__class__.__name__}` has not been initialized.')
+
+    def run_from_nav_file(self):
+        """Run serial RED on all the coordinates from the `.nav` file."""
+        start_angle = self.start_angle
+        end_angle = self.end_angle
+        path = self.path
+        mode = self.mode
+        log = self.log
+        exposure = self.exposure
+
+        if self.rotation_speed:
+            self.ctrl.stage.set_rotation_speed(self.rotation_speed)
+
+        def go_to_first_position(ctrl):
+            ctrl.stage.set(a=start_angle)
+
+        def acquire_cred_data(ctrl):
+            nonlocal start_angle
+            nonlocal end_angle
+
+            tag = ctrl.current_item.tag
+            out_path = path / tag
+
+            out_path.mkdir(exist_ok=True, parents=True)
+
+            print()
+            print(f'Data directory: {out_path}')
+            print(f'Rotating from {start_angle} to {end_angle} degrees')
+            print(ctrl.stage)
+
+            exp = Experiment(ctrl, path=out_path, log=log, exposure=exposure, mode=mode)
+            exp.get_ready()
+            exp.start_collection(target_angle=end_angle, start_angle=start_angle)
+
+            start_angle, end_angle = end_angle, start_angle
+
+        def stop_liveview(ctrl):
+            ctrl.cam.stop_liveview()
+
+        self.ctrl.acquire_at_items(self.nav_items,
+                                   acquire=acquire_cred_data,
+                                   pre_acquire=go_to_first_position,
+                                   post_acquire=stop_liveview)
+
+        if self.rotation_speed:
+            self.ctrl.stage.set_rotation_speed(12)
+
+    def run_from_tracking_file(self):
+        t0 = time.perf_counter()
+        n_measured = 0
+
+        n_items = len(self.tracks)
+
+        for i, track in enumerate(self.tracks):
+            track = track.strip()
+            if not track:
+                continue
+
+            track = self.base_drc / track
+            name = track.name
+            stem = track.stem
+
+            out_path = self.path / stem
+            out_path.mkdir(exist_ok=True, parents=True)
+
+            print()
+            print(f'({i} / {n_items}) Acquiring track: {stem}')
+            print(f'Track file: {self.base_drc / name}')
+            print(f'Data directory: {out_path}')
+            print(self.ctrl.stage)
+            print()
+
+            exp = Experiment(self.ctrl, path=out_path, log=self.log, track=track, exposure=self.exposure, mode=self.mode)
+
+            exp.get_ready()
+
+            try:
+                exp.start_collection(target_angle=0)
+            except InterruptedError:
+                self.ctrl.cam.stop_liveview()
+                break
+            finally:
+                del exp
+
+            n_measured += 1
+
+            time.sleep(3)
+
+        t1 = time.perf_counter()
+        dt = t1 - t0
+        print(f'Serial experiment finished -> {n_measured} crystals measured')
+        print(f'Time taken: {dt:.1f} s, {dt/n_measured:.1f} s/crystal')
+        print(f'Data directory: {self.path}')
+
+
+class Experiment:
+    """Class to control data collection through EMMenu to collect continuous
+    rotation electron diffraction data.
+
+    ctrl: `TEMController`
+        Instance of instamatic.TEMController.TEMController
+    path: str
+        `str` or `pathlib.Path` object giving the path to save data at
+    log: `logging.Logger`
+        Instance of `logging.Logger`
+    exposure: float
+        Exposure time in ms
+    mode: str
+    """
+
+    def __init__(self, ctrl,
+                 path: str = None,
+                 log=None,
+                 track: str = None,
+                 exposure: float = 400,
+                 mode: str = 'diff',
+                 rotation_speed: int = None):
+        super().__init__()
+
+        self.ctrl = ctrl
+        self.emmenu = ctrl.cam
+        self.path = Path(path)
+
+        self.exposure = exposure
+        self.defocus_offset = 1500
+
+        self.logger = log
+        self.mode = mode
+
+        self.rotation_speed = rotation_speed
+
+        if track:
+            self.load_tracking_file(track)
+            self.track = True
+        else:
+            self.track = False
+
+    def load_tracking_file(self, trackfile):
+        trackfile = Path(trackfile)
+        if trackfile.suffix == '.pickle':
+            print(f'(autotracking) Loading tracking file: {trackfile}')
+            dct = pickle.load(open(trackfile, 'rb'))
+
+            self.track_func = dct['y_offset']
+            self.x_offset = dct['x_offset']
+            self.start_x = dct['x_center']
+            self.start_y = dct['y_center']
+            self.start_z = dct['z_pos']
+
+            self.min_angle = dct['angle_min']
+            self.max_angle = dct['angle_max']
+
+            self.crystal_number = dct['i']
+
+            self.trackfile = trackfile
+
+            self.track_interval = 2
+            self.track_relative = False
+
+        else:
+            raise OSError("I don't know how to read file `{trackfile}`")
+
+    def prepare_tracking(self):
+        if self.track:
+            current_angle = self.ctrl.stage.a
+
+            min_angle = self.min_angle
+            max_angle = self.max_angle
+
+            # find start angle closest to current angle
+            if abs(min_angle - current_angle) > abs(max_angle - current_angle):
+                start_angle, target_angle = max_angle, min_angle
+            else:
+                start_angle, target_angle = min_angle, max_angle
+
+            print(f'(autotracking) Overriding angle range: {start_angle:.0f} -> {target_angle:.0f}')
+
+            y_offset = int(self.track_func(start_angle))
+            x_offset = self.x_offset
+
+            print(f'(autotracking) setting a={start_angle:.0f}, x={self.start_x+x_offset:.0f}, y={self.start_y+y_offset:.0f}, z={self.start_z:.0f}')
+            self.ctrl.stage.set_xy_with_backlash_correction(x=self.start_x + x_offset, y=self.start_y + y_offset, step=10000)
+            self.ctrl.stage.set(a=start_angle, z=self.start_z)
+
+            return start_angle, target_angle
+
+    def track_crystal(self, n, angle):
+        # tracking routine
+        if (n % self.track_interval == 0):
+            target_y = self.start_y + int(self.track_func(angle))
+            self.ctrl.stage.set(y=target_y, wait=False)
+            print(f'(autotracking) set y={target_y:.0f}')
+
+    def get_ready(self):
+        self.emmenu.stop_liveview()  # just in case
+
+        try:
+            # next 2 lines are a workaround for EMMENU 5.0.9.0 bugs, FIXME later
+            self.emmenu.set_autoincrement(False)
+            self.emmenu.set_image_index(0)
+        except Exception as e:
+            print(e)
+
+        self.emmenu.set_exposure(self.exposure)
+
+        if not self.ctrl.beam.is_blanked:
+            self.ctrl.beam.blank()
+
+        self.ctrl.screen.up()
+
+        if self.ctrl.mode != self.mode:
+            print(f'Switching to {self.mode} mode')
+            self.ctrl.mode.set(self.mode)
+
+        if self.mode == 'diff':
+            self.ctrl.difffocus.refocus()
+
+        self.emmenu.start_liveview()
+
+        print('Ready...')
+
+    def manual_activation(self) -> float:
+        ACTIVATION_THRESHOLD = 0.2
+
+        print('Waiting for rotation to start...', end=' ')
+        a0 = a = self.ctrl.stage.a
+        while abs(a - a0) < ACTIVATION_THRESHOLD:
+            a = self.ctrl.stage.a
+
+        print('Rotation started...')
+
+        return a
+
+    def start_collection(self, target_angle: float, start_angle: float = None, manual_control: bool = False):
+        """
+        manual_control : bool
+            Control the rotation using the buttons or pedals
+        """
+        angle_tolerance = 0.5  # degrees
+
+        self.now = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+
+        self.stage_positions = []
+        interval = 0.7  # interval at which it check for rotation to end / does tracking
+
+        if self.track:
+            start_angle, target_angle = self.prepare_tracking()
+
+        if start_angle:
+            print(f'Going to starting angle: {start_angle:.1f}')
+            self.ctrl.stage.a = start_angle
+
+        self.start_position = self.ctrl.stage.get()
+        start_angle = self.start_position.a
+
+        if self.track:
+            # Center crystal position
+            if self.mode == 'diff':
+                self.ctrl.difffocus.defocus(self.defocus_offset)
+            self.ctrl.beam.unblank()
+
+            input('Move SAED aperture to crystal and press <ENTER> to measure! ')
+
+            # cannot do this while lieview is running
+            # img1 = self.ctrl.get_rotated_image()
+            # write_tiff(self.path / "image_before.tiff", img1)
+
+            self.ctrl.beam.blank()
+            if self.mode == 'diff':
+                self.ctrl.difffocus.refocus()
+            time.sleep(3)
+
+        self.ctrl.beam.unblank(delay=0.2)  # give the beamblank some time to dissappear to avoid weak first frame
+
+        # with autoincrement(False), otherwise use `get_next_empty_image_index()`
+        # start_index is set to 1, because EMMENU always takes a single image (0) when liveview is activated
+        start_index = 1
+        # start_index = self.emmenu.get_next_empty_image_index()
+
+        if manual_control:
+            start_angle = self.manual_activation()
+            last_angle = 999
+        elif self.rotation_speed:
+            self.ctrl.stage.set_a_with_speed(a=target_angle, speed=self.rotation_speed, wait=False)
+        else:
+            self.ctrl.stage.set(a=target_angle, wait=False)
+
+        self.emmenu.start_record()  # start recording
+
+        t0 = time.perf_counter()
+        t_delta = t0
+
+        n = 0
+
+        print('Acquiring data...')
+
+        while True:
+            t = time.perf_counter()
+
+            if not manual_control:
+                if abs(self.ctrl.stage.a - target_angle) < angle_tolerance:
+                    print('Target angle reached!')
+                    break
+
+            if t - t_delta > interval:
+
+                n += 1
+                x, y, z, a, _ = pos = self.ctrl.stage.get()
+                self.stage_positions.append((t, pos))
+                t_delta = t
+                # print(t, pos)
+
+                if manual_control:
+                    current_angle = a
+                    if last_angle == current_angle:
+                        print(f'Manual rotation was interrupted (current: {current_angle:.2f} | last {last_angle:.2f})')
+                        break
+                    last_angle = current_angle
+
+                    print(f' >> Current angle: {a:.2f}', end='      \r')
+
+                if self.track:
+                    self.track_crystal(n=n, angle=a)
+
+            # Stop/interrupt and go to next crystal
+            if msvcrt.kbhit():
+                key = msvcrt.getch().decode()
+                if key == ' ':
+                    print('Stopping the stage!')
+                    self.ctrl.stage.stop()
+                    break
+                if key == 'q':
+                    self.ctrl.stage.stop()
+                    raise InterruptedError('Data collection was interrupted!')
+
+        t1 = time.perf_counter()
+        self.emmenu.stop_liveview()
+
+        if self.ctrl.beam.is_blanked:
+            self.ctrl.beam.blank()
+
+        self.end_position = self.ctrl.stage.get()
+        end_angle = self.end_position.a
+
+        end_index = self.emmenu.get_image_index()
+
+        self.t_start = t0
+        self.t_end = t1
+        self.total_time = t1 - t0
+
+        self.nframes = nframes = end_index - start_index + 1
+        if nframes < 1:
+            print('No frames measured??')
+            return
+
+        self.osc_angle = abs(end_angle - start_angle) / nframes
+
+        # acquisition_time = total_time / nframes
+        self.total_angle = abs(end_angle - start_angle)
+        self.rotation_axis = config.camera.camera_rotation_vs_stage_xy
+        self.camera_length = int(self.ctrl.magnification.get())
+        self.spotsize = self.ctrl.spotsize
+        self.rotation_speed = (end_angle - start_angle) / self.total_time
+        self.exposure_time = self.emmenu.get_exposure()
+        self.start_angle, self.end_angle = start_angle, end_angle
+
+        try:
+            # sometimes breaks with:
+            # AttributeError: 'NoneType' object has no attribute 'EMVector'
+            timestamps = self.emmenu.get_timestamps(start_index, end_index)
+        except AttributeError as e:
+            print(e)
+            print(f'Timestamps from {start_index} to {end_index}')
+            timestamps = [1, 2, 3, 4, 5]  # just to make it work
+
+        self.timings = get_acquisition_time(timestamps, exp_time=self.exposure_time, savefig=True, drc=self.path)
+
+        self.log_end_status()
+        self.log_stage_positions()
+
+        print('Writing data files...')
+        path_data = self.path / 'tiff'
+        path_data.mkdir(exist_ok=True, parents=True)
+
+        self.emmenu.writeTiffs(start_index, end_index, path=path_data)
+
+        if self.track:
+            # Center crystal position
+            if self.mode == 'diff':
+                self.ctrl.difffocus.defocus(self.defocus_offset)
+            self.ctrl.beam.unblank()
+
+            img2 = self.ctrl.get_rotated_image()
+            write_tiff(self.path / 'image_after.tiff', img2)
+
+            self.ctrl.beam.blank()
+            if self.mode == 'diff':
+                self.ctrl.difffocus.refocus()
+
+        print(f'Wrote {nframes} images (#{start_index}->#{end_index}) to {path_data}')
+
+        if self.track:
+            print(f'Done with this crystal (number #{self.crystal_number})!')
+        else:
+            print('Done with this crystal!')
+
+    def log_end_status(self):
+        wavelength = config.microscope.wavelength
+
+        try:
+            pixelsize = config.calibration['diff']['pixelsize'][self.camera_length]  # px / Angstrom
+        except KeyError:
+            print(f'Warning: No such camera length: {self.camera_length} in diff calibration, defaulting to 1.0')
+            pixelsize = 1.0
+
+        physical_pixelsize = config.camera.physical_pixelsize  # mm
+
+        binning = self.emmenu.getBinning()
+        image_dimensions_x, image_dimensions_y = self.emmenu.getImageDimensions()
+        camera_dimensions_x, camera_dimensions_y = self.emmenu.getCameraDimensions()
+
+        pixelsize *= binning
+        physical_pixelsize *= binning
+
+        print(f'\nRotated {self.total_angle:.2f} degrees from {self.start_angle:.2f} to {self.end_angle:.2f}')
+        print('Start stage position:  X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:6.1f} | B {:6.1f}'.format(*self.start_position))
+        print('End stage position:    X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:6.1f} | B {:6.1f}'.format(*self.end_position))
+        print(f'Data collection camera length: {self.camera_length} cm')
+        print(f'Data collection spot size: {self.spotsize}')
+        print(f'Rotation speed: {self.rotation_speed:.3f} degrees/s')
+
+        with open(self.path / 'cRED_log.txt', 'w') as f:
+            print(f'Program: {instamatic.__long_title__} + EMMenu {self.emmenu.getEMMenuVersion()}', file=f)
+            print(f'Camera: {config.camera.name}', file=f)
+            print(f'Microscope: {config.microscope.name}', file=f)
+            print(f'Camera type: {self.emmenu.getCameraType()}', file=f)
+            print(f'Camera config: {self.emmenu.getCurrentConfigName()}', file=f)
+            print(f'Mode: {self.mode}', file=f)
+            print(f'Data Collection Time: {self.now}', file=f)
+            print(f'Time Period Start: {self.t_start}', file=f)
+            print(f'Time Period End: {self.t_end}', file=f)
+            print(f'Number of frames: {self.nframes}', file=f)
+            print(f'Starting angle: {self.start_angle:.2f} degrees', file=f)
+            print(f'Ending angle: {self.end_angle:.2f} degrees', file=f)
+            print(f'Rotation range: {self.end_angle-self.start_angle:.2f} degrees', file=f)
+            print(f'Rotation speed: {self.rotation_speed:.3f} degrees/s', file=f)
+            print(f'Exposure Time: {self.timings.exposure_time:.3f} s', file=f)
+            print(f'Acquisition time: {self.timings.acquisition_time:.3f} s', file=f)
+            print(f'Overhead time: {self.timings.overhead:.3f} s', file=f)
+            print(f'Total time: {self.total_time:.3f} s', file=f)
+            print(f'Wavelength: {wavelength} Angstrom', file=f)
+            print(f'Spot Size: {self.spotsize}', file=f)
+            print(f'Camera length: {self.camera_length} cm', file=f)
+            print(f'Pixelsize: {pixelsize} px/Angstrom', file=f)
+            print(f'Physical pixelsize: {physical_pixelsize} um', file=f)
+            print(f'Binning: {binning}', file=f)
+            print(f'Image dimensions: {image_dimensions_x} {image_dimensions_y}', file=f)
+            print(f'Camera dimensions: {camera_dimensions_x} {camera_dimensions_y}', file=f)
+            print(f'Stretch amplitude: {config.camera.stretch_azimuth} %', file=f)
+            print(f'Stretch azimuth: {config.camera.stretch_amplitude} degrees', file=f)
+            print(f'Rotation axis: {self.rotation_axis} radians', file=f)
+            print(f'Oscillation angle: {self.osc_angle:.4f} degrees', file=f)
+            print('Stage start: X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:8.2f} | B {:8.2f}'.format(*self.start_position), file=f)
+            print('Beam stopper: yes', file=f)
+
+            if self.track:
+                print()
+                print(f'Crystal number: {self.crystal_number}', file=f)
+                print(f'Tracking data: {self.trackfile}', file=f)
+                print(f'Tracking between {self.min_angle} and {self.max_angle}', file=f)
+
+            print('', file=f)
+
+        print(f'Wrote file {f.name}')
+
+    def log_stage_positions(self):
+        fn = 'stage_positions(tracked).txt' if self.track else 'stage_positions.txt'
+        with open(self.path / fn, 'w') as f:
+            print('# timestamp x y z a b', file=f)
+            for t, (x, y, z, a, b) in self.stage_positions:
+                print(t, x, y, z, a, b, file=f)
+
+        print(f'Wrote file {f.name}')
+
+        if self.mode != 'diff':
+            if len(self.stage_positions) < 3:
+                print('Not enough stage positions for interpolation')
+            else:
+                pos = np.array([p[1] for p in self.stage_positions])  # (t, (x y z a b))
+                idx = np.argmin(np.abs(pos[:, 3]))
+                x_center = pos[:, 0].mean()
+                y_center = pos[idx, 1]
+                z_pos = pos[0:, 2].mean()
+                f = interp1d(pos[:, 3], pos[:, 1] - y_center, fill_value='extrapolate', kind='quadratic')
+
+                d = {}
+                d['y_offset'] = f
+                d['x_offset'] = 0
+                d['x_center'] = x_center
+                d['y_center'] = y_center
+                d['z_pos'] = z_pos
+
+                d['angle_min'] = self.start_angle
+                d['angle_max'] = self.end_angle
+
+                d['i'] = 0
+
+                fn = self.path / 'track.pickle'
+                pickle.dump(d, open(fn, 'wb'))
+
+                print(f'Wrote file {fn.name}')
+
+
+if __name__ == '__main__':
+    from instamatic import TEMController
+    from instamatic.io import get_new_work_subdirectory
+
+    ctrl = TEMController.initialize()
+
+    expdir = get_new_work_subdirectory()
+    expdir.mkdir(exist_ok=True, parents=True)
+
+    exp = Experiment(ctrl, path=expdir)
+    exp.get_ready()
+    exp.run(target_angle=20)
```

### Comparing `instamatic-1.8.0/instamatic/experiments/red/experiment.py` & `instamatic-1.9.0/instamatic/experiments/red/experiment.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,221 +1,221 @@
-import datetime
-import os
-import time
-from pathlib import Path
-
-import numpy as np
-from tqdm.auto import tqdm
-
-from instamatic import config
-from instamatic.formats import write_tiff
-from instamatic.processing.ImgConversionTPX import ImgConversionTPX as ImgConversion
-
-
-class Experiment:
-    """Initialize stepwise rotation electron diffraction experiment.
-
-    ctrl:
-        Instance of instamatic.TEMController.TEMController
-    path:
-        `str` or `pathlib.Path` object giving the path to save data at
-    log:
-        Instance of `logging.Logger`
-    flatfield:
-        Path to flatfield correction image
-    """
-
-    def __init__(self, ctrl, path: str = None, log=None, flatfield=None):
-        super().__init__()
-        self.ctrl = ctrl
-        self.path = Path(path)
-
-        self.mrc_path = self.path / 'mrc'
-        self.tiff_path = self.path / 'tiff'
-        self.tiff_image_path = self.path / 'tiff_image'
-
-        self.tiff_path.mkdir(exist_ok=True, parents=True)
-        self.tiff_image_path.mkdir(exist_ok=True, parents=True)
-        self.mrc_path.mkdir(exist_ok=True, parents=True)
-
-        self.logger = log
-        self.camtype = ctrl.cam.name
-
-        self.flatfield = flatfield
-
-        self.offset = 1
-        self.current_angle = None
-        self.buffer = []
-
-    def start_collection(self, exposure_time: float, tilt_range: float, stepsize: float):
-        """Start or continue data collection for `tilt_range` degrees with
-        steps given by `stepsize`, To finalize data collection and write data
-        files, run `self.finalize`.
-
-        The number of images collected is defined by `tilt_range / stepsize`.
-
-        exposure_time:
-            Exposure time for each image in seconds
-        tilt_range:
-            Tilt range starting from the current angle in degrees. Must be positive.
-        stepsize:
-            Step size for the angle in degrees, controls the direction and can be positive or negative
-        """
-        self.spotsize = self.ctrl.spotsize
-        self.now = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-        self.logger.info('Data recording started at: {self.now}')
-        self.logger.info(f'Exposure time: {exposure_time} s, Tilt range: {tilt_range}, step size: {stepsize}')
-
-        ctrl = self.ctrl
-
-        if stepsize < 0:
-            tilt_range = -abs(tilt_range)
-        else:
-            tilt_range = abs(tilt_range)
-
-        if self.current_angle is None:
-            self.start_angle = start_angle = ctrl.stage.a
-        else:
-            start_angle = self.current_angle + stepsize
-
-        tilt_positions = np.arange(start_angle, start_angle + tilt_range, stepsize)
-        print(f'\nStart_angle: {start_angle:.3f}')
-        # print "Angles:", tilt_positions
-
-        image_mode = ctrl.mode.get()
-        if image_mode != 'diff':
-            fn = self.tiff_image_path / f'image_{self.offset}.tiff'
-            img, h = self.ctrl.get_image(exposure_time / 5)
-            write_tiff(fn, img, header=h)
-            ctrl.mode.set('diff')
-            time.sleep(1.0)  # add some delay to account for beam lag
-
-        if ctrl.cam.streamable:
-            ctrl.cam.block()
-
-        # for i, a in enumerate(tilt_positions):
-        for i, angle in enumerate(tqdm(tilt_positions)):
-            ctrl.stage.a = angle
-
-            j = i + self.offset
-
-            img, h = self.ctrl.get_image(exposure_time)
-
-            self.buffer.append((j, img, h))
-
-        self.offset += len(tilt_positions)
-        self.nframes = j
-
-        self.end_angle = end_angle = ctrl.stage.a
-
-        if ctrl.cam.streamable:
-            ctrl.cam.unblock()
-
-        self.camera_length = int(self.ctrl.magnification.get())
-        self.stepsize = stepsize
-        self.exposure_time = exposure_time
-
-        with open(self.path / 'summary.txt', 'a') as f:
-            print(f'{self.now}: Data collected from {start_angle:.2f} degree to {end_angle:.2f} degree in {len(tilt_positions)} frames.', file=f)
-            print(f'Data collected from {start_angle:.2f} degree to {end_angle:.2f} degree in {len(tilt_positions)} frames.')
-
-        self.logger.info('Data collected from {start_angle:.2f} degree to {end_angle:.2f} degree (camera length: {camera_length} mm).')
-
-        self.current_angle = angle
-        print(f'Done, current angle = {self.current_angle:.2f} degrees')
-
-        if image_mode != 'diff':
-            ctrl.mode.set(image_mode)
-
-    def finalize(self):
-        """Finalize data collection after `self.start_collection` has been run.
-
-        Write data in `self.buffer` to path given by `self.path`.
-        """
-        self.logger.info(f'Data saving path: {self.path}')
-        self.rotation_axis = config.camera.camera_rotation_vs_stage_xy
-
-        self.pixelsize = config.calibration['diff']['pixelsize'][self.camera_length]  # px / Angstrom
-        self.physical_pixelsize = config.camera.physical_pixelsize  # mm
-        self.wavelength = config.microscope.wavelength  # angstrom
-        self.stretch_azimuth = config.camera.stretch_azimuth
-        self.stretch_amplitude = config.camera.stretch_amplitude
-
-        with open(self.path / 'summary.txt', 'a') as f:
-            print(f'Rotation range: {self.end_angle-self.start_angle:.2f} degrees', file=f)
-            print(f'Exposure Time: {self.exposure_time:.3f} s', file=f)
-            print(f'Spot Size: {self.spotsize}', file=f)
-            print(f'Camera length: {self.camera_length} mm', file=f)
-            print(f'Pixelsize: {self.pixelsize} px/Angstrom', file=f)
-            print(f'Physical pixelsize: {self.physical_pixelsize} um', file=f)
-            print(f'Wavelength: {self.wavelength} Angstrom', file=f)
-            print(f'Stretch amplitude: {self.stretch_azimuth} %', file=f)
-            print(f'Stretch azimuth: {self.stretch_amplitude} degrees', file=f)
-            print(f'Rotation axis: {self.rotation_axis} radians', file=f)
-            print(f'Stepsize: {self.stepsize:.4f} degrees', file=f)
-            print(f'Number of frames: {self.nframes}', file=f)
-
-        img_conv = ImgConversion(buffer=self.buffer,
-                                 osc_angle=self.stepsize,
-                                 start_angle=self.start_angle,
-                                 end_angle=self.end_angle,
-                                 rotation_axis=self.rotation_axis,
-                                 acquisition_time=self.exposure_time,
-                                 flatfield=self.flatfield,
-                                 pixelsize=self.pixelsize,
-                                 physical_pixelsize=self.physical_pixelsize,
-                                 wavelength=self.wavelength,
-                                 stretch_amplitude=self.stretch_amplitude,
-                                 stretch_azimuth=self.stretch_azimuth,
-                                 )
-
-        print('Writing data files...')
-        img_conv.threadpoolwriter(tiff_path=self.tiff_path,
-                                  mrc_path=self.mrc_path,
-                                  workers=8)
-
-        print('Writing input files...')
-        img_conv.write_ed3d(self.mrc_path)
-        img_conv.write_pets_inp(self.path)
-
-        img_conv.write_beam_centers(self.path)
-
-        print('Data Collection and Conversion Done.')
-        print()
-
-        return True
-
-
-def main():
-    from instamatic import TEMController
-    ctrl = TEMController.initialize()
-
-    import logging
-    log = logging.getLogger(__name__)
-
-    exposure_time = 0.5
-    tilt_range = 10
-    stepsize = 1.0
-
-    i = 1
-    while True:
-        expdir = f'experiment_{i}'
-        if os.path.exists(expdir):
-            i += 1
-        else:
-            break
-
-    print(f'\nData directory: {expdir}')
-
-    red_exp = Experiment(ctrl=ctrl, path=expdir, log=log, flatfield=None)
-    red_exp.start_collection(exposure_time=exposure_time, tilt_range=tilt_range, stepsize=stepsize)
-
-    input('Press << Enter >> to start the experiment... ')
-
-    while not input(f'\nPress << Enter >> to continue for another {tilt_range} degrees. [any key to finalize] '):
-        red_exp.start_collection(exposure_time=exposure_time, tilt_range=tilt_range, stepsize=stepsize)
-
-    red_exp.finalize()
-
-
-if __name__ == '__main__':
-    main()
+import datetime
+import os
+import time
+from pathlib import Path
+
+import numpy as np
+from tqdm.auto import tqdm
+
+from instamatic import config
+from instamatic.formats import write_tiff
+from instamatic.processing.ImgConversionTPX import ImgConversionTPX as ImgConversion
+
+
+class Experiment:
+    """Initialize stepwise rotation electron diffraction experiment.
+
+    ctrl:
+        Instance of instamatic.TEMController.TEMController
+    path:
+        `str` or `pathlib.Path` object giving the path to save data at
+    log:
+        Instance of `logging.Logger`
+    flatfield:
+        Path to flatfield correction image
+    """
+
+    def __init__(self, ctrl, path: str = None, log=None, flatfield=None):
+        super().__init__()
+        self.ctrl = ctrl
+        self.path = Path(path)
+
+        self.mrc_path = self.path / 'mrc'
+        self.tiff_path = self.path / 'tiff'
+        self.tiff_image_path = self.path / 'tiff_image'
+
+        self.tiff_path.mkdir(exist_ok=True, parents=True)
+        self.tiff_image_path.mkdir(exist_ok=True, parents=True)
+        self.mrc_path.mkdir(exist_ok=True, parents=True)
+
+        self.logger = log
+        self.camtype = ctrl.cam.name
+
+        self.flatfield = flatfield
+
+        self.offset = 1
+        self.current_angle = None
+        self.buffer = []
+
+    def start_collection(self, exposure_time: float, tilt_range: float, stepsize: float):
+        """Start or continue data collection for `tilt_range` degrees with
+        steps given by `stepsize`, To finalize data collection and write data
+        files, run `self.finalize`.
+
+        The number of images collected is defined by `tilt_range / stepsize`.
+
+        exposure_time:
+            Exposure time for each image in seconds
+        tilt_range:
+            Tilt range starting from the current angle in degrees. Must be positive.
+        stepsize:
+            Step size for the angle in degrees, controls the direction and can be positive or negative
+        """
+        self.spotsize = self.ctrl.spotsize
+        self.now = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+        self.logger.info('Data recording started at: {self.now}')
+        self.logger.info(f'Exposure time: {exposure_time} s, Tilt range: {tilt_range}, step size: {stepsize}')
+
+        ctrl = self.ctrl
+
+        if stepsize < 0:
+            tilt_range = -abs(tilt_range)
+        else:
+            tilt_range = abs(tilt_range)
+
+        if self.current_angle is None:
+            self.start_angle = start_angle = ctrl.stage.a
+        else:
+            start_angle = self.current_angle + stepsize
+
+        tilt_positions = np.arange(start_angle, start_angle + tilt_range, stepsize)
+        print(f'\nStart_angle: {start_angle:.3f}')
+        # print "Angles:", tilt_positions
+
+        image_mode = ctrl.mode.get()
+        if image_mode != 'diff':
+            fn = self.tiff_image_path / f'image_{self.offset}.tiff'
+            img, h = self.ctrl.get_image(exposure_time / 5)
+            write_tiff(fn, img, header=h)
+            ctrl.mode.set('diff')
+            time.sleep(1.0)  # add some delay to account for beam lag
+
+        if ctrl.cam.streamable:
+            ctrl.cam.block()
+
+        # for i, a in enumerate(tilt_positions):
+        for i, angle in enumerate(tqdm(tilt_positions)):
+            ctrl.stage.a = angle
+
+            j = i + self.offset
+
+            img, h = self.ctrl.get_image(exposure_time)
+
+            self.buffer.append((j, img, h))
+
+        self.offset += len(tilt_positions)
+        self.nframes = j
+
+        self.end_angle = end_angle = ctrl.stage.a
+
+        if ctrl.cam.streamable:
+            ctrl.cam.unblock()
+
+        self.camera_length = int(self.ctrl.magnification.get())
+        self.stepsize = stepsize
+        self.exposure_time = exposure_time
+
+        with open(self.path / 'summary.txt', 'a') as f:
+            print(f'{self.now}: Data collected from {start_angle:.2f} degree to {end_angle:.2f} degree in {len(tilt_positions)} frames.', file=f)
+            print(f'Data collected from {start_angle:.2f} degree to {end_angle:.2f} degree in {len(tilt_positions)} frames.')
+
+        self.logger.info('Data collected from {start_angle:.2f} degree to {end_angle:.2f} degree (camera length: {camera_length} mm).')
+
+        self.current_angle = angle
+        print(f'Done, current angle = {self.current_angle:.2f} degrees')
+
+        if image_mode != 'diff':
+            ctrl.mode.set(image_mode)
+
+    def finalize(self):
+        """Finalize data collection after `self.start_collection` has been run.
+
+        Write data in `self.buffer` to path given by `self.path`.
+        """
+        self.logger.info(f'Data saving path: {self.path}')
+        self.rotation_axis = config.camera.camera_rotation_vs_stage_xy
+
+        self.pixelsize = config.calibration['diff']['pixelsize'][self.camera_length]  # px / Angstrom
+        self.physical_pixelsize = config.camera.physical_pixelsize  # mm
+        self.wavelength = config.microscope.wavelength  # angstrom
+        self.stretch_azimuth = config.camera.stretch_azimuth
+        self.stretch_amplitude = config.camera.stretch_amplitude
+
+        with open(self.path / 'summary.txt', 'a') as f:
+            print(f'Rotation range: {self.end_angle-self.start_angle:.2f} degrees', file=f)
+            print(f'Exposure Time: {self.exposure_time:.3f} s', file=f)
+            print(f'Spot Size: {self.spotsize}', file=f)
+            print(f'Camera length: {self.camera_length} mm', file=f)
+            print(f'Pixelsize: {self.pixelsize} px/Angstrom', file=f)
+            print(f'Physical pixelsize: {self.physical_pixelsize} um', file=f)
+            print(f'Wavelength: {self.wavelength} Angstrom', file=f)
+            print(f'Stretch amplitude: {self.stretch_azimuth} %', file=f)
+            print(f'Stretch azimuth: {self.stretch_amplitude} degrees', file=f)
+            print(f'Rotation axis: {self.rotation_axis} radians', file=f)
+            print(f'Stepsize: {self.stepsize:.4f} degrees', file=f)
+            print(f'Number of frames: {self.nframes}', file=f)
+
+        img_conv = ImgConversion(buffer=self.buffer,
+                                 osc_angle=self.stepsize,
+                                 start_angle=self.start_angle,
+                                 end_angle=self.end_angle,
+                                 rotation_axis=self.rotation_axis,
+                                 acquisition_time=self.exposure_time,
+                                 flatfield=self.flatfield,
+                                 pixelsize=self.pixelsize,
+                                 physical_pixelsize=self.physical_pixelsize,
+                                 wavelength=self.wavelength,
+                                 stretch_amplitude=self.stretch_amplitude,
+                                 stretch_azimuth=self.stretch_azimuth,
+                                 )
+
+        print('Writing data files...')
+        img_conv.threadpoolwriter(tiff_path=self.tiff_path,
+                                  mrc_path=self.mrc_path,
+                                  workers=8)
+
+        print('Writing input files...')
+        img_conv.write_ed3d(self.mrc_path)
+        img_conv.write_pets_inp(self.path)
+
+        img_conv.write_beam_centers(self.path)
+
+        print('Data Collection and Conversion Done.')
+        print()
+
+        return True
+
+
+def main():
+    from instamatic import TEMController
+    ctrl = TEMController.initialize()
+
+    import logging
+    log = logging.getLogger(__name__)
+
+    exposure_time = 0.5
+    tilt_range = 10
+    stepsize = 1.0
+
+    i = 1
+    while True:
+        expdir = f'experiment_{i}'
+        if os.path.exists(expdir):
+            i += 1
+        else:
+            break
+
+    print(f'\nData directory: {expdir}')
+
+    red_exp = Experiment(ctrl=ctrl, path=expdir, log=log, flatfield=None)
+    red_exp.start_collection(exposure_time=exposure_time, tilt_range=tilt_range, stepsize=stepsize)
+
+    input('Press << Enter >> to start the experiment... ')
+
+    while not input(f'\nPress << Enter >> to continue for another {tilt_range} degrees. [any key to finalize] '):
+        red_exp.start_collection(exposure_time=exposure_time, tilt_range=tilt_range, stepsize=stepsize)
+
+    red_exp.finalize()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `instamatic-1.8.0/instamatic/experiments/serialed/experiment.py` & `instamatic-1.9.0/instamatic/experiments/serialed/experiment.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,581 +1,578 @@
-import json
-import logging
-import time
-from pathlib import Path
-
-import matplotlib.pyplot as plt
-import numpy as np
-from tqdm.auto import tqdm
-
-from instamatic import config
-from instamatic.calibrate import CalibBeamShift
-from instamatic.calibrate import CalibDirectBeam
-from instamatic.formats import *
-from instamatic.processing.find_crystals import find_crystals
-from instamatic.processing.find_crystals import find_crystals_timepix
-from instamatic.processing.flatfield import apply_flatfield_correction
-from instamatic.processing.flatfield import remove_deadpixels
-
-
-def make_grid_on_stage(startpoint, endpoint, padding=2.0):
-    """Divide the stage up in a grid, starting at 'startpoint' ending at
-    'endpoint'."""
-    stepsize = np.array((0.016 * 512, 0.016 * 512))
-
-    x1, y1 = pos1 = np.array((0, 0))
-    x2, y2 = pos2 = np.array((1000, 1000))
-
-    pos_delta = pos2 - pos1
-
-    nx, ny = np.abs(pos_delta / (stepsize + padding)).astype(int)
-
-    xgrid, ygrid = np.meshgrid(np.linspace(x1, x2, nx), np.linspace(y1, y2, ny))
-
-    return np.stack((xgrid.flatten(), ygrid.flatten())).T
-
-
-def get_gridpoints_in_circle(nx, ny=0, radius=1, borderwidth=0.8):
-    """Make a grid (size=n*n), and return the coordinates of those
-    fitting inside a circle (radius=r)
-    nx: `int`
-    ny: `int` (optional)
-        Used to define a mesh nx*ny, if ny is missing, nx*nx is used
-    radius: `float`
-        radius of circle
-    borderwidth: `float`, 0.0 - 1.0
-        define a border around the circumference not to place any points
-        should probably be related to the effective camera size:
-    """
-    xr = np.linspace(-1, 1, nx)
-    if ny:
-        yr = np.linspace(-1, 1, ny)
-    else:
-        yr = xr
-    xgrid, ygrid = np.meshgrid(xr, yr)
-    # reverse order of every other row for more efficient pathing
-    xgrid[1::2] = np.fliplr(xgrid[1::2])
-
-    sel = xgrid**2 + ygrid**2 < 1.0 * (1 - borderwidth)
-    xvals = xgrid[sel].flatten()
-    yvals = ygrid[sel].flatten()
-    return xvals * radius, yvals * radius
-
-
-def get_offsets_in_scan_area(box_x, box_y=0, radius=75, padding=2, k=1.0, angle=0, plot=False):
-    """
-    box_x: float or int,
-        x-dimensions of the box in micrometers.
-        if box_y is missing, box_y = box_x
-    box_y: float or int,
-        y-dimension of the box in micrometers (optional)
-    radius: int or float,
-        radius of the scan_area in micrometer
-    padding: int or float
-        distance between boxes in micrometers
-    k: float,
-        scaling factor for the borderwidth
-    """
-
-    nx = 1 + int(2.0 * radius / (box_x + padding))
-    if box_y:
-        ny = 1 + int(2.0 * radius / (box_y + padding))
-        diff = 0.5 * (2 * max(box_x, box_y)**2)**0.5
-    else:
-        diff = 0.5 * (2 * (box_x)**2)**0.5
-        ny = 0
-
-    borderwidth = k * (1.0 - (radius - diff) / radius)
-
-    x_offsets, y_offsets = get_gridpoints_in_circle(nx=nx, ny=ny, radius=radius, borderwidth=borderwidth)
-
-    if angle:
-        sin = np.sin(angle)
-        cos = np.cos(angle)
-        r = np.array([
-            [cos, -sin],
-            [sin, cos]])
-        x_offsets, y_offsets = np.dot(np.vstack([x_offsets, y_offsets]).T, r).T
-
-    if plot:
-        from matplotlib import patches
-
-        num = len(x_offsets)
-        textstr = f'grid: {nx} x {ny}\nk: {k}\nborder: {borderwidth:.2f}\nradius: {radius:.2f}\nboxsize: {box_x:.2f} x {box_y:.2f} um\nnumber: {num}'
-
-        print()
-        print(textstr)
-
-        cx, cy = (box_x / 2.0, box_y / 2.0)
-        if angle:
-            cx, cy = np.dot((cx, cy), r)
-
-        if num < 1000:
-            fig = plt.figure(figsize=(10, 5))
-            ax = fig.add_subplot(111)
-            plt.scatter(0, 0)
-            plt.scatter(x_offsets, y_offsets, picker=8, marker='+')
-            circle = plt.Circle((0, 0), radius, fill=False, color='blue')
-            ax.add_artist(circle)
-            circle = plt.Circle((0, 0), radius * (1 - borderwidth / 2), fill=False, color='red')
-            ax.add_artist(circle)
-
-            for dx, dy in zip(x_offsets, y_offsets):
-                rect = patches.Rectangle((dx - cx, dy - cy), box_x, box_y, fill=False, angle=np.degrees(-angle))
-                ax.add_artist(rect)
-
-            ax.text(1.05, 0.95, textstr, transform=ax.transAxes, fontsize=14,
-                    verticalalignment='top', bbox={'boxstyle': 'round', 'facecolor': 'wheat', 'alpha': 0.5})
-
-            ax.set_xlim(-100, 100)
-            ax.set_ylim(-100, 100)
-            ax.set_aspect('equal')
-            plt.show()
-
-    return np.vstack((x_offsets, y_offsets)).T
-
-
-class Experiment:
-    """Data collection protocol for serial electron diffraction.
-
-    Related publication:     J. Appl. Cryst. (2018). 51, 1262-1273
-    https://doi.org/10.1107/S1600576718009500.
-    """
-
-    def __init__(self, ctrl, params, scan_radius=None, begin_here=False, expdir=None, log=None):
-        super().__init__()
-        self.ctrl = ctrl
-        self.camera = ctrl.cam.name
-        self.log = log
-
-        self.scan_radius = scan_radius
-        self.begin_here = begin_here
-
-        self.setup_folders(expdir=expdir)
-
-        self.load_calibration(**params)
-
-        # set flags
-        self.ctrl.tem.VERIFY_STAGE_POSITION = False
-
-    def setup_folders(self, expdir=None, name='experiment'):
-        if not expdir:
-            n = 1
-            while True:
-                expdir = Path(f'{name}_{n}')
-                if expdir.exists():
-                    n += 1
-                else:
-                    break
-
-        self.expdir = expdir
-        self.calibdir = self.expdir / 'calib'
-        self.imagedir = self.expdir / 'images'
-        self.datadir = self.expdir / 'data'
-
-        for drc in self.expdir, self.calibdir, self.imagedir, self.datadir:
-            drc.mkdir(exist_ok=True, parents=True)
-
-        return self.expdir
-
-    def load_calibration(self, **kwargs):
-        """Load user specified config and calibration files."""
-
-        self.ctrl.mode.set('mag1')
-        self.ctrl.brightness.max()
-
-        if (not self.begin_here) or (not self.scan_radius):
-            print('\nSelect area to scan')
-            print('-------------------')
-        if not self.begin_here:
-            input(' >> Move the stage to where you want to start and press <ENTER> to continue')
-        x, y, _, _, _ = self.ctrl.stage.get()
-        self.scan_centers = np.array([[x, y]])
-        if not self.scan_radius:
-            self.scan_radius = float(input(' >> Enter the radius (micrometer) of the area to scan: [100] ') or 100)
-        border_k = 0
-
-        self.image_binsize = kwargs.get('image_binsize', self.ctrl.cam.default_binsize)
-        self.image_exposure = kwargs.get('image_exposure', self.ctrl.cam.default_exposure)
-        self.image_spotsize = kwargs.get('image_spotsize', 4)
-        # self.magnification   = kwargs["magnification"]
-        self.image_threshold = kwargs.get('image_threshold', 100)
-        # do not store brightness to self, as this is set later when calibrating the direct beam
-        image_brightness = kwargs.get('diff_brightness', 38000)
-
-        try:
-            self.calib_beamshift = CalibBeamShift.from_file()
-        except OSError:
-            self.ctrl.mode.set('mag1')
-            self.ctrl.store('image')
-            self.ctrl.brightness.set(image_brightness)
-            self.ctrl.tem.setSpotSize(self.image_spotsize)
-
-            self.calib_beamshift = CalibBeamShift.live(self.ctrl, outdir=self.calibdir)
-
-            self.magnification = self.ctrl.magnification.value
-            self.log.info('Brightness=%s', self.ctrl.brightness)
-
-        self.pixelsize_mag1 = config.calibration['mag1']['pixelsize'][self.magnification] / 1000  # nm -> um
-        xdim, ydim = self.ctrl.cam.getCameraDimensions()
-        self.image_dimensions = self.pixelsize_mag1 * xdim, self.pixelsize_mag1 * ydim
-        self.log.info('Image dimensions %s', self.image_dimensions)
-
-        self.diff_binsize = kwargs.get('diff_binsize', self.ctrl.cam.default_binsize)  # this also messes with calibrate_beamshift class
-        self.diff_exposure = kwargs.get('diff_exposure', self.ctrl.cam.default_exposure)
-        self.diff_spotsize = kwargs.get('diff_spotsize', 4)
-        # self.diff_cameralength = kwargs.get("diff_cameralength",       800)
-
-        try:
-            self.calib_directbeam = CalibDirectBeam.from_file()
-        except OSError:
-            self.ctrl.mode.set('diff')
-            self.ctrl.store('diffraction')
-            self.ctrl.tem.setSpotSize(self.diff_spotsize)
-
-            self.calib_directbeam = CalibDirectBeam.live(self.ctrl, outdir=self.calibdir)
-
-            self.diff_brightness = self.ctrl.brightness.value
-            self.diff_difffocus = self.ctrl.difffocus.value
-            self.diff_cameralength = self.ctrl.magnification.value
-
-        self.diff_pixelsize = config.calibration['diff']['pixelsize'][self.diff_cameralength]
-        self.change_spotsize = self.diff_spotsize != self.image_spotsize
-        self.crystal_spread = kwargs.get('crystal_spread', 0.6)
-
-        if self.ctrl.cam.name == 'timepix':
-            self.find_crystals = find_crystals_timepix
-            self.flatfield = kwargs.get('flatfield', 'flatfield.tiff')
-        else:
-            self.find_crystals = find_crystals
-            self.flatfield = None
-
-        if self.flatfield is not None:
-            self.flatfield, h_flatfield = read_tiff(self.flatfield)
-            self.deadpixels = h_flatfield['deadpixels']
-
-        # self.sample_rotation_angles = ( -10, -5, 5, 10 )
-        # self.sample_rotation_angles = (-5, 5)
-        self.sample_rotation_angles = ()
-
-        self.camera_rotation_angle = config.camera.camera_rotation_vs_stage_xy
-
-        # Make negative to reflect config change 2019-07-03 to make omega more in line with other software
-        self.camera_rotation_angle = -self.camera_rotation_angle
-
-        box_x, box_y = self.image_dimensions
-
-        offsets = get_offsets_in_scan_area(box_x, box_y, self.scan_radius, k=border_k, padding=2, angle=self.camera_rotation_angle, plot=False)
-        self.offsets = offsets * 1000
-
-        # store kwargs to experiment drc
-        kwargs['diff_brightness'] = self.diff_brightness
-        kwargs['diff_cameralength'] = self.diff_cameralength
-        kwargs['diff_difffocus'] = self.diff_difffocus
-        kwargs['scan_radius'] = self.scan_radius
-        kwargs['scan_centers'] = self.scan_centers.tolist()
-        kwargs['stage_positions'] = len(self.offsets)
-        kwargs['image_dimensions'] = self.image_dimensions
-
-        self.log.info('params', kwargs)
-
-        json.dump(kwargs, open(self.expdir / 'params_out.json', 'w'), indent=2)
-
-    def initialize_microscope(self):
-        """Intialize microscope."""
-
-        import atexit
-        atexit.register(self.ctrl.restore)
-
-        self.ctrl.mode.set('diff')
-        self.ctrl.brightness.set(self.diff_brightness)
-        self.ctrl.difffocus.set(self.diff_difffocus)
-        self.ctrl.tem.setSpotSize(self.diff_spotsize)
-        input('\nPress <ENTER> to get neutral diffraction shift')
-        self.neutral_diffshift = np.array(self.ctrl.diffshift.get())
-        self.log.info('DiffShift(x=%d, y=%d)', *self.neutral_diffshift)
-
-        self.ctrl.mode.set('mag1')
-        self.ctrl.magnification.value = self.magnification
-        self.ctrl.brightness.max()
-        self.calib_beamshift.center(self.ctrl)
-        self.neutral_beamshift = self.ctrl.beamshift.get()
-        self.ctrl.tem.setSpotSize(self.image_spotsize)
-
-    def image_mode(self, delay=0.2):
-        """Switch to image mode (mag1), reset beamshift/diffshift, spread
-        beam."""
-
-        # self.log.debug("Switching back to image mode")
-        time.sleep(delay)
-
-        self.ctrl.beamshift.set(*self.neutral_beamshift)
-        # avoid setting diffshift in image mode, because it messes with the beam position
-        if self.ctrl.mode == 'diff':
-            self.ctrl.diffshift.set(*self.neutral_diffshift)
-
-        self.ctrl.mode.set('mag1')
-        self.ctrl.brightness.max()
-
-    def diffraction_mode(self, delay=0.2):
-        """Switch to diffraction mode, focus the beam, and set the correct
-        focus."""
-        # self.log.debug("Switching to diffraction mode")
-        time.sleep(delay)
-
-        self.ctrl.brightness.set(self.diff_brightness)
-        self.ctrl.mode.set('diff')
-        self.ctrl.difffocus.value = self.diff_difffocus  # difffocus must be set AFTER switching to diffraction mode
-
-    def report_status(self):
-        """Report experiment status."""
-
-        print()
-        print(f'Output directory:\n{self.expdir}')
-        print()
-        print(f'Imaging     : binsize = {self.image_binsize}')
-        print(f'              exposure = {self.image_exposure}')
-        print(f'              magnification = {self.magnification}')
-        print(f'              spotsize = {self.image_spotsize}')
-        print(f'Diffraction : binsize = {self.diff_binsize}')
-        print(f'              exposure = {self.diff_exposure}')
-        print(f'              brightness = {self.diff_brightness}')
-        print(f'              spotsize = {self.diff_spotsize}')
-
-    def loop_centers(self):
-        """Loop over scan centers defined Move the stage to all positions
-        defined in centers.
-
-        Return
-            di: dict, contains information on scan areas
-        """
-        ncenters = len(self.scan_centers)
-
-        for i, (x, y) in enumerate(self.scan_centers):
-            try:
-                self.ctrl.stage.set(x=x, y=y)
-            except ValueError as e:
-                print(e)
-                print(' >> Moving to next center...')
-                print()
-                continue
-            else:
-                self.log.info('Stage position: center %d/%d -> (x=%0.1f, y=%0.1f)', i, ncenters, x, y)
-                yield i, (x, y)
-
-    def loop_positions(self, delay=0.05):
-        """Loop over positions defined Move the stage to each of the positions
-        in self.offsets.
-
-        Return
-            dct: dict, contains information on positions
-        """
-        for i, scan_center in self.loop_centers():
-            center_x, center_y = scan_center
-
-            t = tqdm(self.offsets, desc='                           ')
-            for j, (x_offset, y_offset) in enumerate(t):
-                x = center_x + x_offset
-                y = center_y + y_offset
-                try:
-                    self.ctrl.stage.set(x=x, y=y)
-                except ValueError as e:
-                    print(e)
-                    print(' >> Moving to next position...')
-                    print()
-                    continue
-                else:
-                    time.sleep(delay)
-                    t.set_description(f'Stage(x={x:7.0f}, y={y:7.0f})')
-
-                    dct = {'exp_scan_number': i, 'exp_image_number': j, 'exp_scan_offset': (x_offset, y_offset), 'exp_scan_center': (center_x, center_y), 'exp_stage_position': (x, y)}
-                    dct['ImageComment'] = 'scan {exp_scan_number} image {exp_image_number}'.format(**dct)
-                    yield dct
-
-    def loop_crystals(self, crystal_coords, delay=0):
-        """Loop over crystal coordinates (pixels) Switch to diffraction mode,
-        and shift the beam to be on the crystal.
-
-        Return
-            dct: dict, contains information on beam/diffshift
-        """
-        ncrystals = len(crystal_coords)
-        if ncrystals == 0:
-            raise StopIteration('No crystals found.')
-
-        self.diffraction_mode()
-        beamshift_coords = self.calib_beamshift.pixelcoord_to_beamshift(crystal_coords)
-
-        t = tqdm(beamshift_coords, desc='                           ')
-
-        for k, beamshift in enumerate(t):
-            # self.log.debug("Diffraction: crystal %d/%d", k+1, ncrystals)
-            self.ctrl.beamshift.set(*beamshift)
-
-            # compensate beamshift
-            beamshift_offset = beamshift - self.neutral_beamshift
-            pixelshift = self.calib_directbeam.beamshift2pixelshift(beamshift_offset)
-
-            diffshift_offset = self.calib_directbeam.pixelshift2diffshift(pixelshift)
-            diffshift = self.neutral_diffshift - diffshift_offset
-
-            self.ctrl.diffshift.set(*diffshift.astype(int))
-
-            t.set_description('BeamShift(x={:5.0f}, y={:5.0f})'.format(*beamshift))
-            time.sleep(delay)
-
-            dct = {'exp_pattern_number': k,
-                   'exp_diffshift_offset': diffshift_offset,
-                   'exp_beamshift_offset': beamshift_offset,
-                   'exp_beamshift': beamshift,
-                   'exp_diffshift': diffshift}
-
-            yield dct
-
-    def apply_corrections(self, img, h):
-        if self.flatfield is not None:
-            img = remove_deadpixels(img, deadpixels=self.deadpixels)
-            h['DeadPixelCorrection'] = True
-            img = apply_flatfield_correction(img, flatfield=self.flatfield)
-            h['FlatfieldCorrection'] = True
-        return img, h
-
-    def run(self, ctrl=None, **kwargs):
-        """Run serial electron diffraction experiment."""
-
-        self.initialize_microscope()
-
-        header_keys = kwargs.get('header_keys', None)
-
-        d_image = {
-            'exp_neutral_diffshift': self.neutral_beamshift,
-            'exp_neutral_beamshift': self.neutral_diffshift,
-            'exp_image_spotsize': self.image_spotsize,
-            'exp_magnification': self.magnification,
-            'ImageDimensions': self.image_dimensions,
-        }
-        d_diff = {
-            'exp_neutral_diffshift': self.neutral_beamshift,
-            'exp_neutral_beamshift': self.neutral_diffshift,
-            'exp_diff_brightness': self.diff_brightness,
-            'exp_diff_spotsize': self.diff_spotsize,
-            'exp_diff_cameralength': self.diff_cameralength,
-            'exp_diff_difffocus': self.diff_difffocus,
-            'ImagePixelsize': self.diff_pixelsize,
-        }
-
-        self.log.info('d_image', d_image)
-        self.log.info('d_tiff', d_diff)
-
-        input("\nPress <ENTER> to start experiment ('Ctrl-C' to interrupt)\n")
-
-        for i, d_pos in enumerate(self.loop_positions()):
-
-            outfile = self.imagedir / f'image_{i:04d}'
-
-            if self.change_spotsize:
-                self.ctrl.tem.setSpotSize(self.image_spotsize)
-
-            img, h = self.ctrl.get_image(exposure=self.image_exposure, binsize=self.image_binsize, header_keys=header_keys)
-
-            if self.change_spotsize:
-                self.ctrl.tem.setSpotSize(self.image_spotsize)
-
-            self.ctrl.tem.setSpotSize(self.diff_spotsize)
-
-            im_mean = img.mean()
-            if im_mean < self.image_threshold:
-                # self.log.debug("Dark image detected (mean=%f)", im_mean)
-                continue
-
-            img, h = self.apply_corrections(img, h)
-
-            crystal_positions = self.find_crystals(img, self.magnification, spread=self.crystal_spread) * self.image_binsize
-            crystal_coords = [(crystal.x, crystal.y) for crystal in crystal_positions]
-
-            for d in (d_image, d_pos):
-                h.update(d)
-            h['exp_crystal_coords'] = crystal_coords
-
-            write_hdf5(outfile, img, header=h)
-
-            ncrystals = len(crystal_coords)
-            if ncrystals == 0:
-                continue
-
-            self.log.info('%d crystals found in %s', ncrystals, outfile)
-
-            for k, d_cryst in enumerate(self.loop_crystals(crystal_coords)):
-                outfile = self.datadir / f'image_{i:04d}_{k:04d}'
-                comment = f'Image {i} Crystal {k}'
-                img, h = self.ctrl.get_image(binsize=self.diff_binsize, exposure=self.diff_exposure, comment=comment, header_keys=header_keys)
-                img, h = self.apply_corrections(img, h)
-
-                for d in (d_diff, d_pos, d_cryst):
-                    h.update(d)
-
-                h['crystal_is_isolated'] = crystal_positions[k].isolated
-                h['crystal_clusters'] = crystal_positions[k].n_clusters
-                h['total_area_micrometer'] = crystal_positions[k].area_micrometer
-                h['total_area_pixel'] = crystal_positions[k].area_pixel
-
-                # img_processed = neural_network.preprocess(img.astype(float))
-                # quality = neural_network.predict(img_processed)
-                # h["crystal_quality"] = quality
-
-                write_hdf5(outfile, img, header=h)
-
-                if self.sample_rotation_angles:
-                    for rotation_angle in self.sample_rotation_angles:
-                        self.log.debug('Rotation angle = %f', rotation_angle)
-                        self.ctrl.stage.a = rotation_angle
-
-                        outfile = self.datadir / f'image_{i:04d}_{k:04d}_{rotation_angle}'
-                        img, h = self.ctrl.get_image(exposure=self.diff_exposure, binsize=self.diff_binsize, comment=comment, header_keys=header_keys)
-                        img, h = self.apply_corrections(img, h)
-
-                        for d in (d_diff, d_pos, d_cryst):
-                            h.update(d)
-
-                        write_hdf5(outfile, img, header=h)
-
-                    self.ctrl.stage.a = 0
-
-            self.image_mode()
-
-        print('\n\nData collection finished.')
-
-
-def main():
-    import argparse
-    description = """Command line program to run the serial ED data collection routine."""
-
-    parser = argparse.ArgumentParser(
-        description=description,
-        formatter_class=argparse.RawDescriptionHelpFormatter)
-
-    options = parser.parse_args()
-
-    from instamatic import TEMController
-
-    try:
-        params = json.load(open('params.json'))
-    except OSError:
-        params = {}
-
-    logging.basicConfig(format='%(asctime)s | %(module)s:%(lineno)s | %(levelname)s | %(message)s',
-                        filename='instamatic.log',
-                        level=logging.DEBUG)
-    logging.captureWarnings(True)
-    log = logging.getLogger(__name__)
-
-    ctrl = TEMController.initialize()
-
-    exp = Experiment(ctrl, params, log=log)
-    exp.report_status()
-    exp.run()
-
-    ctrl.close()
-
-
-if __name__ == '__main__':
-    main()
+import json
+import logging
+import time
+from pathlib import Path
+
+import matplotlib.pyplot as plt
+import numpy as np
+from tqdm.auto import tqdm
+
+from instamatic import config
+from instamatic.calibrate import CalibBeamShift, CalibDirectBeam
+from instamatic.formats import *
+from instamatic.processing.find_crystals import find_crystals, find_crystals_timepix
+from instamatic.processing.flatfield import apply_flatfield_correction, remove_deadpixels
+
+
+def make_grid_on_stage(startpoint, endpoint, padding=2.0):
+    """Divide the stage up in a grid, starting at 'startpoint' ending at
+    'endpoint'."""
+    stepsize = np.array((0.016 * 512, 0.016 * 512))
+
+    x1, y1 = pos1 = np.array((0, 0))
+    x2, y2 = pos2 = np.array((1000, 1000))
+
+    pos_delta = pos2 - pos1
+
+    nx, ny = np.abs(pos_delta / (stepsize + padding)).astype(int)
+
+    xgrid, ygrid = np.meshgrid(np.linspace(x1, x2, nx), np.linspace(y1, y2, ny))
+
+    return np.stack((xgrid.flatten(), ygrid.flatten())).T
+
+
+def get_gridpoints_in_circle(nx, ny=0, radius=1, borderwidth=0.8):
+    """Make a grid (size=n*n), and return the coordinates of those
+    fitting inside a circle (radius=r)
+    nx: `int`
+    ny: `int` (optional)
+        Used to define a mesh nx*ny, if ny is missing, nx*nx is used
+    radius: `float`
+        radius of circle
+    borderwidth: `float`, 0.0 - 1.0
+        define a border around the circumference not to place any points
+        should probably be related to the effective camera size:
+    """
+    xr = np.linspace(-1, 1, nx)
+    if ny:
+        yr = np.linspace(-1, 1, ny)
+    else:
+        yr = xr
+    xgrid, ygrid = np.meshgrid(xr, yr)
+    # reverse order of every other row for more efficient pathing
+    xgrid[1::2] = np.fliplr(xgrid[1::2])
+
+    sel = xgrid**2 + ygrid**2 < 1.0 * (1 - borderwidth)
+    xvals = xgrid[sel].flatten()
+    yvals = ygrid[sel].flatten()
+    return xvals * radius, yvals * radius
+
+
+def get_offsets_in_scan_area(box_x, box_y=0, radius=75, padding=2, k=1.0, angle=0, plot=False):
+    """
+    box_x: float or int,
+        x-dimensions of the box in micrometers.
+        if box_y is missing, box_y = box_x
+    box_y: float or int,
+        y-dimension of the box in micrometers (optional)
+    radius: int or float,
+        radius of the scan_area in micrometer
+    padding: int or float
+        distance between boxes in micrometers
+    k: float,
+        scaling factor for the borderwidth
+    """
+
+    nx = 1 + int(2.0 * radius / (box_x + padding))
+    if box_y:
+        ny = 1 + int(2.0 * radius / (box_y + padding))
+        diff = 0.5 * (2 * max(box_x, box_y)**2)**0.5
+    else:
+        diff = 0.5 * (2 * (box_x)**2)**0.5
+        ny = 0
+
+    borderwidth = k * (1.0 - (radius - diff) / radius)
+
+    x_offsets, y_offsets = get_gridpoints_in_circle(nx=nx, ny=ny, radius=radius, borderwidth=borderwidth)
+
+    if angle:
+        sin = np.sin(angle)
+        cos = np.cos(angle)
+        r = np.array([
+            [cos, -sin],
+            [sin, cos]])
+        x_offsets, y_offsets = np.dot(np.vstack([x_offsets, y_offsets]).T, r).T
+
+    if plot:
+        from matplotlib import patches
+
+        num = len(x_offsets)
+        textstr = f'grid: {nx} x {ny}\nk: {k}\nborder: {borderwidth:.2f}\nradius: {radius:.2f}\nboxsize: {box_x:.2f} x {box_y:.2f} um\nnumber: {num}'
+
+        print()
+        print(textstr)
+
+        cx, cy = (box_x / 2.0, box_y / 2.0)
+        if angle:
+            cx, cy = np.dot((cx, cy), r)
+
+        if num < 1000:
+            fig = plt.figure(figsize=(10, 5))
+            ax = fig.add_subplot(111)
+            plt.scatter(0, 0)
+            plt.scatter(x_offsets, y_offsets, picker=8, marker='+')
+            circle = plt.Circle((0, 0), radius, fill=False, color='blue')
+            ax.add_artist(circle)
+            circle = plt.Circle((0, 0), radius * (1 - borderwidth / 2), fill=False, color='red')
+            ax.add_artist(circle)
+
+            for dx, dy in zip(x_offsets, y_offsets):
+                rect = patches.Rectangle((dx - cx, dy - cy), box_x, box_y, fill=False, angle=np.degrees(-angle))
+                ax.add_artist(rect)
+
+            ax.text(1.05, 0.95, textstr, transform=ax.transAxes, fontsize=14,
+                    verticalalignment='top', bbox={'boxstyle': 'round', 'facecolor': 'wheat', 'alpha': 0.5})
+
+            ax.set_xlim(-100, 100)
+            ax.set_ylim(-100, 100)
+            ax.set_aspect('equal')
+            plt.show()
+
+    return np.vstack((x_offsets, y_offsets)).T
+
+
+class Experiment:
+    """Data collection protocol for serial electron diffraction.
+
+    Related publication:     J. Appl. Cryst. (2018). 51, 1262-1273
+    https://doi.org/10.1107/S1600576718009500.
+    """
+
+    def __init__(self, ctrl, params, scan_radius=None, begin_here=False, expdir=None, log=None):
+        super().__init__()
+        self.ctrl = ctrl
+        self.camera = ctrl.cam.name
+        self.log = log
+
+        self.scan_radius = scan_radius
+        self.begin_here = begin_here
+
+        self.setup_folders(expdir=expdir)
+
+        self.load_calibration(**params)
+
+        # set flags
+        self.ctrl.tem.VERIFY_STAGE_POSITION = False
+
+    def setup_folders(self, expdir=None, name='experiment'):
+        if not expdir:
+            n = 1
+            while True:
+                expdir = Path(f'{name}_{n}')
+                if expdir.exists():
+                    n += 1
+                else:
+                    break
+
+        self.expdir = expdir
+        self.calibdir = self.expdir / 'calib'
+        self.imagedir = self.expdir / 'images'
+        self.datadir = self.expdir / 'data'
+
+        for drc in self.expdir, self.calibdir, self.imagedir, self.datadir:
+            drc.mkdir(exist_ok=True, parents=True)
+
+        return self.expdir
+
+    def load_calibration(self, **kwargs):
+        """Load user specified config and calibration files."""
+
+        self.ctrl.mode.set('mag1')
+        self.ctrl.brightness.max()
+
+        if (not self.begin_here) or (not self.scan_radius):
+            print('\nSelect area to scan')
+            print('-------------------')
+        if not self.begin_here:
+            input(' >> Move the stage to where you want to start and press <ENTER> to continue')
+        x, y, _, _, _ = self.ctrl.stage.get()
+        self.scan_centers = np.array([[x, y]])
+        if not self.scan_radius:
+            self.scan_radius = float(input(' >> Enter the radius (micrometer) of the area to scan: [100] ') or 100)
+        border_k = 0
+
+        self.image_binsize = kwargs.get('image_binsize', self.ctrl.cam.default_binsize)
+        self.image_exposure = kwargs.get('image_exposure', self.ctrl.cam.default_exposure)
+        self.image_spotsize = kwargs.get('image_spotsize', 4)
+        # self.magnification   = kwargs["magnification"]
+        self.image_threshold = kwargs.get('image_threshold', 100)
+        # do not store brightness to self, as this is set later when calibrating the direct beam
+        image_brightness = kwargs.get('diff_brightness', 38000)
+
+        try:
+            self.calib_beamshift = CalibBeamShift.from_file()
+        except OSError:
+            self.ctrl.mode.set('mag1')
+            self.ctrl.store('image')
+            self.ctrl.brightness.set(image_brightness)
+            self.ctrl.tem.setSpotSize(self.image_spotsize)
+
+            self.calib_beamshift = CalibBeamShift.live(self.ctrl, outdir=self.calibdir)
+
+            self.magnification = self.ctrl.magnification.value
+            self.log.info('Brightness=%s', self.ctrl.brightness)
+
+        self.pixelsize_mag1 = config.calibration['mag1']['pixelsize'][self.magnification] / 1000  # nm -> um
+        xdim, ydim = self.ctrl.cam.getCameraDimensions()
+        self.image_dimensions = self.pixelsize_mag1 * xdim, self.pixelsize_mag1 * ydim
+        self.log.info('Image dimensions %s', self.image_dimensions)
+
+        self.diff_binsize = kwargs.get('diff_binsize', self.ctrl.cam.default_binsize)  # this also messes with calibrate_beamshift class
+        self.diff_exposure = kwargs.get('diff_exposure', self.ctrl.cam.default_exposure)
+        self.diff_spotsize = kwargs.get('diff_spotsize', 4)
+        # self.diff_cameralength = kwargs.get("diff_cameralength",       800)
+
+        try:
+            self.calib_directbeam = CalibDirectBeam.from_file()
+        except OSError:
+            self.ctrl.mode.set('diff')
+            self.ctrl.store('diffraction')
+            self.ctrl.tem.setSpotSize(self.diff_spotsize)
+
+            self.calib_directbeam = CalibDirectBeam.live(self.ctrl, outdir=self.calibdir)
+
+            self.diff_brightness = self.ctrl.brightness.value
+            self.diff_difffocus = self.ctrl.difffocus.value
+            self.diff_cameralength = self.ctrl.magnification.value
+
+        self.diff_pixelsize = config.calibration['diff']['pixelsize'][self.diff_cameralength]
+        self.change_spotsize = self.diff_spotsize != self.image_spotsize
+        self.crystal_spread = kwargs.get('crystal_spread', 0.6)
+
+        if self.ctrl.cam.name == 'timepix':
+            self.find_crystals = find_crystals_timepix
+            self.flatfield = kwargs.get('flatfield', 'flatfield.tiff')
+        else:
+            self.find_crystals = find_crystals
+            self.flatfield = None
+
+        if self.flatfield is not None:
+            self.flatfield, h_flatfield = read_tiff(self.flatfield)
+            self.deadpixels = h_flatfield['deadpixels']
+
+        # self.sample_rotation_angles = ( -10, -5, 5, 10 )
+        # self.sample_rotation_angles = (-5, 5)
+        self.sample_rotation_angles = ()
+
+        self.camera_rotation_angle = config.camera.camera_rotation_vs_stage_xy
+
+        # Make negative to reflect config change 2019-07-03 to make omega more in line with other software
+        self.camera_rotation_angle = -self.camera_rotation_angle
+
+        box_x, box_y = self.image_dimensions
+
+        offsets = get_offsets_in_scan_area(box_x, box_y, self.scan_radius, k=border_k, padding=2, angle=self.camera_rotation_angle, plot=False)
+        self.offsets = offsets * 1000
+
+        # store kwargs to experiment drc
+        kwargs['diff_brightness'] = self.diff_brightness
+        kwargs['diff_cameralength'] = self.diff_cameralength
+        kwargs['diff_difffocus'] = self.diff_difffocus
+        kwargs['scan_radius'] = self.scan_radius
+        kwargs['scan_centers'] = self.scan_centers.tolist()
+        kwargs['stage_positions'] = len(self.offsets)
+        kwargs['image_dimensions'] = self.image_dimensions
+
+        self.log.info('params', kwargs)
+
+        json.dump(kwargs, open(self.expdir / 'params_out.json', 'w'), indent=2)
+
+    def initialize_microscope(self):
+        """Intialize microscope."""
+
+        import atexit
+        atexit.register(self.ctrl.restore)
+
+        self.ctrl.mode.set('diff')
+        self.ctrl.brightness.set(self.diff_brightness)
+        self.ctrl.difffocus.set(self.diff_difffocus)
+        self.ctrl.tem.setSpotSize(self.diff_spotsize)
+        input('\nPress <ENTER> to get neutral diffraction shift')
+        self.neutral_diffshift = np.array(self.ctrl.diffshift.get())
+        self.log.info('DiffShift(x=%d, y=%d)', *self.neutral_diffshift)
+
+        self.ctrl.mode.set('mag1')
+        self.ctrl.magnification.value = self.magnification
+        self.ctrl.brightness.max()
+        self.calib_beamshift.center(self.ctrl)
+        self.neutral_beamshift = self.ctrl.beamshift.get()
+        self.ctrl.tem.setSpotSize(self.image_spotsize)
+
+    def image_mode(self, delay=0.2):
+        """Switch to image mode (mag1), reset beamshift/diffshift, spread
+        beam."""
+
+        # self.log.debug("Switching back to image mode")
+        time.sleep(delay)
+
+        self.ctrl.beamshift.set(*self.neutral_beamshift)
+        # avoid setting diffshift in image mode, because it messes with the beam position
+        if self.ctrl.mode == 'diff':
+            self.ctrl.diffshift.set(*self.neutral_diffshift)
+
+        self.ctrl.mode.set('mag1')
+        self.ctrl.brightness.max()
+
+    def diffraction_mode(self, delay=0.2):
+        """Switch to diffraction mode, focus the beam, and set the correct
+        focus."""
+        # self.log.debug("Switching to diffraction mode")
+        time.sleep(delay)
+
+        self.ctrl.brightness.set(self.diff_brightness)
+        self.ctrl.mode.set('diff')
+        self.ctrl.difffocus.value = self.diff_difffocus  # difffocus must be set AFTER switching to diffraction mode
+
+    def report_status(self):
+        """Report experiment status."""
+
+        print()
+        print(f'Output directory:\n{self.expdir}')
+        print()
+        print(f'Imaging     : binsize = {self.image_binsize}')
+        print(f'              exposure = {self.image_exposure}')
+        print(f'              magnification = {self.magnification}')
+        print(f'              spotsize = {self.image_spotsize}')
+        print(f'Diffraction : binsize = {self.diff_binsize}')
+        print(f'              exposure = {self.diff_exposure}')
+        print(f'              brightness = {self.diff_brightness}')
+        print(f'              spotsize = {self.diff_spotsize}')
+
+    def loop_centers(self):
+        """Loop over scan centers defined Move the stage to all positions
+        defined in centers.
+
+        Return
+            di: dict, contains information on scan areas
+        """
+        ncenters = len(self.scan_centers)
+
+        for i, (x, y) in enumerate(self.scan_centers):
+            try:
+                self.ctrl.stage.set(x=x, y=y)
+            except ValueError as e:
+                print(e)
+                print(' >> Moving to next center...')
+                print()
+                continue
+            else:
+                self.log.info('Stage position: center %d/%d -> (x=%0.1f, y=%0.1f)', i, ncenters, x, y)
+                yield i, (x, y)
+
+    def loop_positions(self, delay=0.05):
+        """Loop over positions defined Move the stage to each of the positions
+        in self.offsets.
+
+        Return
+            dct: dict, contains information on positions
+        """
+        for i, scan_center in self.loop_centers():
+            center_x, center_y = scan_center
+
+            t = tqdm(self.offsets, desc='                           ')
+            for j, (x_offset, y_offset) in enumerate(t):
+                x = center_x + x_offset
+                y = center_y + y_offset
+                try:
+                    self.ctrl.stage.set(x=x, y=y)
+                except ValueError as e:
+                    print(e)
+                    print(' >> Moving to next position...')
+                    print()
+                    continue
+                else:
+                    time.sleep(delay)
+                    t.set_description(f'Stage(x={x:7.0f}, y={y:7.0f})')
+
+                    dct = {'exp_scan_number': i, 'exp_image_number': j, 'exp_scan_offset': (x_offset, y_offset), 'exp_scan_center': (center_x, center_y), 'exp_stage_position': (x, y)}
+                    dct['ImageComment'] = 'scan {exp_scan_number} image {exp_image_number}'.format(**dct)
+                    yield dct
+
+    def loop_crystals(self, crystal_coords, delay=0):
+        """Loop over crystal coordinates (pixels) Switch to diffraction mode,
+        and shift the beam to be on the crystal.
+
+        Return
+            dct: dict, contains information on beam/diffshift
+        """
+        ncrystals = len(crystal_coords)
+        if ncrystals == 0:
+            raise StopIteration('No crystals found.')
+
+        self.diffraction_mode()
+        beamshift_coords = self.calib_beamshift.pixelcoord_to_beamshift(crystal_coords)
+
+        t = tqdm(beamshift_coords, desc='                           ')
+
+        for k, beamshift in enumerate(t):
+            # self.log.debug("Diffraction: crystal %d/%d", k+1, ncrystals)
+            self.ctrl.beamshift.set(*beamshift)
+
+            # compensate beamshift
+            beamshift_offset = beamshift - self.neutral_beamshift
+            pixelshift = self.calib_directbeam.beamshift2pixelshift(beamshift_offset)
+
+            diffshift_offset = self.calib_directbeam.pixelshift2diffshift(pixelshift)
+            diffshift = self.neutral_diffshift - diffshift_offset
+
+            self.ctrl.diffshift.set(*diffshift.astype(int))
+
+            t.set_description('BeamShift(x={:5.0f}, y={:5.0f})'.format(*beamshift))
+            time.sleep(delay)
+
+            dct = {'exp_pattern_number': k,
+                   'exp_diffshift_offset': diffshift_offset,
+                   'exp_beamshift_offset': beamshift_offset,
+                   'exp_beamshift': beamshift,
+                   'exp_diffshift': diffshift}
+
+            yield dct
+
+    def apply_corrections(self, img, h):
+        if self.flatfield is not None:
+            img = remove_deadpixels(img, deadpixels=self.deadpixels)
+            h['DeadPixelCorrection'] = True
+            img = apply_flatfield_correction(img, flatfield=self.flatfield)
+            h['FlatfieldCorrection'] = True
+        return img, h
+
+    def run(self, ctrl=None, **kwargs):
+        """Run serial electron diffraction experiment."""
+
+        self.initialize_microscope()
+
+        header_keys = kwargs.get('header_keys', None)
+
+        d_image = {
+            'exp_neutral_diffshift': self.neutral_beamshift,
+            'exp_neutral_beamshift': self.neutral_diffshift,
+            'exp_image_spotsize': self.image_spotsize,
+            'exp_magnification': self.magnification,
+            'ImageDimensions': self.image_dimensions,
+        }
+        d_diff = {
+            'exp_neutral_diffshift': self.neutral_beamshift,
+            'exp_neutral_beamshift': self.neutral_diffshift,
+            'exp_diff_brightness': self.diff_brightness,
+            'exp_diff_spotsize': self.diff_spotsize,
+            'exp_diff_cameralength': self.diff_cameralength,
+            'exp_diff_difffocus': self.diff_difffocus,
+            'ImagePixelsize': self.diff_pixelsize,
+        }
+
+        self.log.info('d_image', d_image)
+        self.log.info('d_tiff', d_diff)
+
+        input("\nPress <ENTER> to start experiment ('Ctrl-C' to interrupt)\n")
+
+        for i, d_pos in enumerate(self.loop_positions()):
+
+            outfile = self.imagedir / f'image_{i:04d}'
+
+            if self.change_spotsize:
+                self.ctrl.tem.setSpotSize(self.image_spotsize)
+
+            img, h = self.ctrl.get_image(exposure=self.image_exposure, binsize=self.image_binsize, header_keys=header_keys)
+
+            if self.change_spotsize:
+                self.ctrl.tem.setSpotSize(self.image_spotsize)
+
+            self.ctrl.tem.setSpotSize(self.diff_spotsize)
+
+            im_mean = img.mean()
+            if im_mean < self.image_threshold:
+                # self.log.debug("Dark image detected (mean=%f)", im_mean)
+                continue
+
+            img, h = self.apply_corrections(img, h)
+
+            crystal_positions = self.find_crystals(img, self.magnification, spread=self.crystal_spread) * self.image_binsize
+            crystal_coords = [(crystal.x, crystal.y) for crystal in crystal_positions]
+
+            for d in (d_image, d_pos):
+                h.update(d)
+            h['exp_crystal_coords'] = crystal_coords
+
+            write_hdf5(outfile, img, header=h)
+
+            ncrystals = len(crystal_coords)
+            if ncrystals == 0:
+                continue
+
+            self.log.info('%d crystals found in %s', ncrystals, outfile)
+
+            for k, d_cryst in enumerate(self.loop_crystals(crystal_coords)):
+                outfile = self.datadir / f'image_{i:04d}_{k:04d}'
+                comment = f'Image {i} Crystal {k}'
+                img, h = self.ctrl.get_image(binsize=self.diff_binsize, exposure=self.diff_exposure, comment=comment, header_keys=header_keys)
+                img, h = self.apply_corrections(img, h)
+
+                for d in (d_diff, d_pos, d_cryst):
+                    h.update(d)
+
+                h['crystal_is_isolated'] = crystal_positions[k].isolated
+                h['crystal_clusters'] = crystal_positions[k].n_clusters
+                h['total_area_micrometer'] = crystal_positions[k].area_micrometer
+                h['total_area_pixel'] = crystal_positions[k].area_pixel
+
+                # img_processed = neural_network.preprocess(img.astype(float))
+                # quality = neural_network.predict(img_processed)
+                # h["crystal_quality"] = quality
+
+                write_hdf5(outfile, img, header=h)
+
+                if self.sample_rotation_angles:
+                    for rotation_angle in self.sample_rotation_angles:
+                        self.log.debug('Rotation angle = %f', rotation_angle)
+                        self.ctrl.stage.a = rotation_angle
+
+                        outfile = self.datadir / f'image_{i:04d}_{k:04d}_{rotation_angle}'
+                        img, h = self.ctrl.get_image(exposure=self.diff_exposure, binsize=self.diff_binsize, comment=comment, header_keys=header_keys)
+                        img, h = self.apply_corrections(img, h)
+
+                        for d in (d_diff, d_pos, d_cryst):
+                            h.update(d)
+
+                        write_hdf5(outfile, img, header=h)
+
+                    self.ctrl.stage.a = 0
+
+            self.image_mode()
+
+        print('\n\nData collection finished.')
+
+
+def main():
+    import argparse
+    description = """Command line program to run the serial ED data collection routine."""
+
+    parser = argparse.ArgumentParser(
+        description=description,
+        formatter_class=argparse.RawDescriptionHelpFormatter)
+
+    options = parser.parse_args()
+
+    from instamatic import TEMController
+
+    try:
+        params = json.load(open('params.json'))
+    except OSError:
+        params = {}
+
+    logging.basicConfig(format='%(asctime)s | %(module)s:%(lineno)s | %(levelname)s | %(message)s',
+                        filename='instamatic.log',
+                        level=logging.DEBUG)
+    logging.captureWarnings(True)
+    log = logging.getLogger(__name__)
+
+    ctrl = TEMController.initialize()
+
+    exp = Experiment(ctrl, params, log=log)
+    exp.report_status()
+    exp.run()
+
+    ctrl.close()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `instamatic-1.8.0/instamatic/formats/__init__.py` & `instamatic-1.9.0/instamatic/formats/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,16 @@
 from pathlib import Path
 
 import h5py
 import numpy as np
 import tifffile
 import yaml
 
-from .adscimage import read_adsc
-from .adscimage import write_adsc
-from .csvIO import read_csv
-from .csvIO import read_ycsv
-from .csvIO import write_csv
-from .csvIO import write_ycsv
+from .adscimage import read_adsc, write_adsc
+from .csvIO import read_csv, read_ycsv, write_csv, write_ycsv
 from .mrc import read_image as read_mrc
 from .mrc import write_image as write_mrc
 from .xdscbf import write as write_cbf
 
 
 def read_image(fname: str) -> (np.array, dict):
     """Guess filetype by extension."""
```

### Comparing `instamatic-1.8.0/instamatic/formats/adscimage.py` & `instamatic-1.9.0/instamatic/formats/adscimage.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-import numpy as np
-
-# from https://github.com/silx-kit/fabio/blob/master/fabio/adscimage.py
-
-
-def swap_needed(header: dict) -> bool:
-    if 'BYTE_ORDER' not in header:
-        # logger.warning("No byte order specified, assuming little_endian")
-        BYTE_ORDER = 'little_endian'
-    else:
-        BYTE_ORDER = header['BYTE_ORDER']
-    if 'little' in BYTE_ORDER and np.little_endian:
-        return False
-    elif 'big' in BYTE_ORDER and not np.little_endian:
-        return False
-    elif 'little' in BYTE_ORDER and not np.little_endian:
-        return True
-    elif 'big' in BYTE_ORDER and np.little_endian:
-        return True
-
-
-def write_adsc(fname: str, data: np.array, header: dict = {}):
-    """Write adsc format."""
-    if 'SIZE1' not in header and 'SIZE2' not in header:
-        dim2, dim1 = data.shape
-        header['SIZE1'] = dim1
-        header['SIZE2'] = dim2
-
-    out = b'{\n'
-    for key in header:
-        out += f'{key}={header[key]};\n'.encode()
-    if 'HEADER_BYTES' in header:
-        pad = int(header['HEADER_BYTES']) - len(out) - 2
-    else:
-        #         hsize = ((len(out) + 23) // 512 + 1) * 512
-        hsize = (len(out) + 533) & ~(512 - 1)
-        out += f'HEADER_BYTES={hsize:d};\n'.encode()
-        pad = hsize - len(out) - 2
-    out += b'}' + (pad + 1) * b'\x00'
-    assert len(out) % 512 == 0, 'Header is not multiple of 512'
-
-    # NOTE: XDS can handle only "SMV" images of TYPE=unsigned_short.
-    dtype = np.uint16
-    data = np.round(data, 0).astype(dtype, copy=False)  # copy=False ensures that no copy is made if dtype is already satisfied
-    if swap_needed(header):
-        data.byteswap(True)
-
-    with open(fname, 'wb') as outf:
-        outf.write(out)
-        outf.write(data.tobytes())
-
-
-def readheader(infile):
-    """read an adsc header."""
-    header = {}
-    line = infile.readline()
-    bytesread = len(line)
-    while b'}' not in line:
-        string = line.decode().strip()
-        if '=' in string:
-            (key, val) = string.split('=')
-            val = val.strip(';')
-            key = key.strip()
-            header[key] = val
-        line = infile.readline()
-        bytesread = bytesread + len(line)
-    return header
-
-
-def read_adsc(fname: str) -> (np.array, dict):
-    """read in the file."""
-    with open(fname, 'rb', buffering=0) as infile:
-        try:
-            header = readheader(infile)
-        except BaseException:
-            raise Exception('Error processing adsc header')
-        # banned by bzip/gzip???
-        try:
-            infile.seek(int(header['HEADER_BYTES']), 0)
-        except TypeError:
-            # Gzipped does not allow a seek and read header is not
-            # promising to stop in the right place
-            infile.close()
-            infile = open(fname, 'rb', buffering=0)
-            infile.read(int(header['HEADER_BYTES']))
-        binary = infile.read()
-    # infile.close()
-
-    # now read the data into the array
-    dim1 = int(header['SIZE1'])
-    dim2 = int(header['SIZE2'])
-    data = np.frombuffer(binary, np.uint16)
-    if swap_needed(header):
-        data.byteswap(True)
-    try:
-        data.shape = (dim2, dim1)
-    except ValueError:
-        raise OSError(f'Size spec in ADSC-header does not match size of image data field {dim1}x{dim2} != {data.size}')
-
-    return data, header
-
-
-if __name__ == '__main__':
-    fn = 'test.img'
-    img = (np.random.random((512, 512)) * 100000).astype(np.uint16)
-
-    header = {}
-    header['SIZE1'] = 512
-    header['SIZE2'] = 512
-
-    write_adsc(fn, img, header=header)
-    print('writing:', img.shape)
-    print('header:', header)
-    print()
-
-    arr, h = read_adsc(fn)
-    print('reading', arr.shape)
-    print('header', h)
-
-    print()
-    print('allclose:', np.allclose(img, arr))
+import numpy as np
+
+# from https://github.com/silx-kit/fabio/blob/master/fabio/adscimage.py
+
+
+def swap_needed(header: dict) -> bool:
+    if 'BYTE_ORDER' not in header:
+        # logger.warning("No byte order specified, assuming little_endian")
+        BYTE_ORDER = 'little_endian'
+    else:
+        BYTE_ORDER = header['BYTE_ORDER']
+    if 'little' in BYTE_ORDER and np.little_endian:
+        return False
+    elif 'big' in BYTE_ORDER and not np.little_endian:
+        return False
+    elif 'little' in BYTE_ORDER and not np.little_endian:
+        return True
+    elif 'big' in BYTE_ORDER and np.little_endian:
+        return True
+
+
+def write_adsc(fname: str, data: np.array, header: dict = {}):
+    """Write adsc format."""
+    if 'SIZE1' not in header and 'SIZE2' not in header:
+        dim2, dim1 = data.shape
+        header['SIZE1'] = dim1
+        header['SIZE2'] = dim2
+
+    out = b'{\n'
+    for key in header:
+        out += f'{key}={header[key]};\n'.encode()
+    if 'HEADER_BYTES' in header:
+        pad = int(header['HEADER_BYTES']) - len(out) - 2
+    else:
+        #         hsize = ((len(out) + 23) // 512 + 1) * 512
+        hsize = (len(out) + 533) & ~(512 - 1)
+        out += f'HEADER_BYTES={hsize:d};\n'.encode()
+        pad = hsize - len(out) - 2
+    out += b'}' + (pad + 1) * b'\x00'
+    assert len(out) % 512 == 0, 'Header is not multiple of 512'
+
+    # NOTE: XDS can handle only "SMV" images of TYPE=unsigned_short.
+    dtype = np.uint16
+    data = np.round(data, 0).astype(dtype, copy=False)  # copy=False ensures that no copy is made if dtype is already satisfied
+    if swap_needed(header):
+        data.byteswap(True)
+
+    with open(fname, 'wb') as outf:
+        outf.write(out)
+        outf.write(data.tobytes())
+
+
+def readheader(infile):
+    """read an adsc header."""
+    header = {}
+    line = infile.readline()
+    bytesread = len(line)
+    while b'}' not in line:
+        string = line.decode().strip()
+        if '=' in string:
+            (key, val) = string.split('=')
+            val = val.strip(';')
+            key = key.strip()
+            header[key] = val
+        line = infile.readline()
+        bytesread = bytesread + len(line)
+    return header
+
+
+def read_adsc(fname: str) -> (np.array, dict):
+    """read in the file."""
+    with open(fname, 'rb', buffering=0) as infile:
+        try:
+            header = readheader(infile)
+        except BaseException:
+            raise Exception('Error processing adsc header')
+        # banned by bzip/gzip???
+        try:
+            infile.seek(int(header['HEADER_BYTES']), 0)
+        except TypeError:
+            # Gzipped does not allow a seek and read header is not
+            # promising to stop in the right place
+            infile.close()
+            infile = open(fname, 'rb', buffering=0)
+            infile.read(int(header['HEADER_BYTES']))
+        binary = infile.read()
+    # infile.close()
+
+    # now read the data into the array
+    dim1 = int(header['SIZE1'])
+    dim2 = int(header['SIZE2'])
+    data = np.frombuffer(binary, np.uint16)
+    if swap_needed(header):
+        data.byteswap(True)
+    try:
+        data.shape = (dim2, dim1)
+    except ValueError:
+        raise OSError(f'Size spec in ADSC-header does not match size of image data field {dim1}x{dim2} != {data.size}')
+
+    return data, header
+
+
+if __name__ == '__main__':
+    fn = 'test.img'
+    img = (np.random.random((512, 512)) * 100000).astype(np.uint16)
+
+    header = {}
+    header['SIZE1'] = 512
+    header['SIZE2'] = 512
+
+    write_adsc(fn, img, header=header)
+    print('writing:', img.shape)
+    print('header:', header)
+    print()
+
+    arr, h = read_adsc(fn)
+    print('reading', arr.shape)
+    print('header', h)
+
+    print()
+    print('allclose:', np.allclose(img, arr))
```

### Comparing `instamatic-1.8.0/instamatic/formats/csvIO.py` & `instamatic-1.9.0/instamatic/formats/csvIO.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,17 +36,16 @@
 
     format:
         ---
         $YAML_BLOCK
         ---
         $CSV_BLOCK
     """
-
     if isinstance(f, str):
-        f = open(f, 'r')
+        f = open(f)
 
     first_line = f.tell()
 
     in_yaml_block = False
 
     yaml_block = []
 
@@ -84,15 +83,14 @@
 
     format:
         ---
         $YAML_BLOCK
         ---
         $CSV_BLOCK
     """
-
     if isinstance(f, str):
         f = open(f, 'w')
 
     f.write('---\n')
     yaml.dump(metadata, f, default_flow_style=False, sort_keys=False)
 
     f.write('---\n')
```

### Comparing `instamatic-1.8.0/instamatic/formats/mrc.py` & `instamatic-1.9.0/instamatic/formats/mrc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,730 +1,729 @@
-# https://github.com/ezralanglois/arachnid/blob/master/arachnid/core/image/formats/mrc.py
-# Licenced under GPL
-"""Read and write images in the MRC format.
-
-.. todo:: define arachnid header and map to mrc
-
-.. note::
-
-    This code is heavily modified version of the MRC parser/writer
-    found in the Scripps Appion program.
-
-
-.. Created on Aug 9, 2012
-.. codeauthor:: Robert Langlois <rl2528@columbia.edu>
-"""
-import logging
-import os
-import sys
-
-import numpy
-
-from . import util
-# import util
-
-_logger = logging.getLogger(__name__)
-_logger.setLevel(logging.INFO)
-
-mrc2numpy = {
-    0: numpy.int8,
-    1: numpy.int16,
-    2: numpy.float32,
-    3: numpy.dtype([('real', numpy.int16), ('imag', numpy.int16)]),
-    # complex made of two int16.  No such thing in numpy
-    #     however, we could manually build a complex array by reading two
-    #     int16 arrays somehow.
-    4: numpy.complex64,
-
-    6: numpy.uint16,    # according to UCSF
-    7: numpy.uint8,    # according to UCSF
-}
-
-# mapping of numpy type to MRC mode
-numpy2mrc = {
-    # convert these to int8
-    numpy.int8: 0,
-    #    numpy.uint8: 0,
-    numpy.bool_: 0,
-
-    # convert these to int16
-    numpy.int16: 1,
-    #    numpy.int8: 1,
-
-    # convert these to float32
-    numpy.float32: 2,
-    numpy.float64: 2,
-    numpy.int32: 2,
-    numpy.int64: 2,
-    numpy.uint32: 2,
-    numpy.uint64: 2,
-
-    # convert these to complex64
-    numpy.complex64: 4,
-    numpy.complex128: 4,
-
-    # convert these to uint16
-    numpy.uint16: 6,
-    numpy.uint8: 7,
-}
-
-intbyteorder = {
-    0x11110000: 'big',
-    0x44440000: 'little',  # hack
-    0x44410000: 'little',  # 0x4144 - 16708
-    286326784: 'big',
-    1145110528: 'little',
-}
-byteorderint = {
-    'big': 0x11110000,
-    'little': 0x44410000,
-}
-byteorderint2 = {
-    'big': 286326784,
-    'little': 1145110528,
-}
-
-
-mrc_defaults = {'alpha': 90, 'beta': 90, 'gamma': 90, 'mapc': 1, 'mapr': 2, 'maps': 3, 'map': 'MAP ', 'byteorder': byteorderint[sys.byteorder]}
-
-
-def _gen_header():
-    """Create the header for an MRC image and stack.
-
-    .. note::
-
-        The following code was adopted from mrc.py in Scripps Appion Package
-
-    :Returns:
-
-    header_image_dtype : numpy.dtype
-                         Header for an MRC image
-    """
-
-    shared_fields = [
-        ('nx', numpy.int32),
-        ('ny', numpy.int32),
-        ('nz', numpy.int32),
-        ('mode', numpy.int32),
-        ('nxstart', numpy.int32),
-        ('nystart', numpy.int32),
-        ('nzstart', numpy.int32),
-        ('mx', numpy.int32),
-        ('my', numpy.int32),
-        ('mz', numpy.int32),
-        ('xlen', numpy.float32),
-        ('ylen', numpy.float32),
-        ('zlen', numpy.float32),
-        ('alpha', numpy.float32),  # defocus
-        ('beta', numpy.float32),  # astig_ang
-        ('gamma', numpy.float32),  # astig_mag
-        ('mapc', numpy.int32),
-        ('mapr', numpy.int32),
-        ('maps', numpy.int32),
-        ('amin', numpy.float32),
-        ('amax', numpy.float32),
-        ('amean', numpy.float32),
-        ('ispg', numpy.int32),
-        ('nsymbt', numpy.int32),
-    ]
-
-    header_image_dtype = numpy.dtype(shared_fields + [
-        ('extra', 'S100'),
-        ('xorigin', numpy.float32),  # 208 320  4   char    cmap;      Contains "MAP "
-        ('yorigin', numpy.float32),
-        ('zorigin', numpy.float32),
-        ('map', 'S4'),
-        ('byteorder', numpy.int32),
-        ('rms', numpy.float32),
-        ('nlabels', numpy.int32),
-        ('label0', 'S80'),
-        ('label1', 'S80'),  # Image Type
-        # Allow image `type`s are:
-        #    - Power Spectra: 'P'
-        #    - Windowed Particle: 'W'
-        #    - Micrograph: 'M'
-        ('label2', 'S80'),
-        ('label3', 'S80'),
-        ('label4', 'S80'),
-        ('label5', 'S80'),
-        ('label6', 'S80'),
-        ('label7', 'S80'),
-        ('label8', 'S80'),
-        ('label9', 'S80'),
-    ])
-
-    return header_image_dtype
-
-# --------------------------------------------------------------------
-# End attribution
-# --------------------------------------------------------------------
-
-
-header_image_dtype = _gen_header()
-
-mrc2ara = {'': ''}
-mrc2ara.update({h[0]: 'mrc' + h[0] for h in header_image_dtype.names})
-ara2mrc = {val: key for key, val in mrc2ara.items()}
-
-
-def create_header(shape, dtype, order='C', header=None):
-    """Create a header for the MRC image format.
-
-    @todo support header parameters
-
-    :Parameters:
-
-    shape : tuple
-            Shape of the array
-    dtype : numpy.dtype
-            Data type for NumPy ndarray
-    header : dict
-             Header values  for image
-    :Returns:
-
-    h : dtype
-        Data type for NumPy ndarray describing the header
-    """
-
-    pass
-
-
-def array_from_header(header):
-    """Convert header information to array parameters.
-
-    :Parameters:
-
-    header : header_dtype
-             Header fields
-
-    :Returns:
-
-    header : dict
-             File header
-    dtype : dtype
-            Data type
-    shape : tuple
-            Shape of the array
-    order : str
-            Order of the array
-    offset : int
-             Header offset
-    swap : bool
-            Swap byte order
-    """
-
-    pass
-
-
-def cache_data():
-    """Get keywords to be added as data cache.
-
-    :Returns:
-
-    extra : dict
-            Keyword arguments
-    """
-
-    return {'header': None, 'no_strict_mrc': False, 'force_volume': False}
-
-
-def is_format_header(h):
-    """Test if the given header has the proper format.
-
-    :Parameters:
-
-    h : array
-        Header to test
-
-    :Returns:
-
-    val : bool
-          Test if dtype matches format dtype
-    """
-
-    return h.dtype == header_image_dtype or h.dtype == header_image_dtype.newbyteorder()
-
-
-bad_mrc_header = False
-
-
-def is_readable(filename, no_strict_mrc=False):
-    """Test if the file read has a valid MRC header.
-
-    :Parameters:
-
-    filename : str or file object
-               Filename or open stream for a file
-    no_strict_mrc : bool
-                    Perform strict MRC header checking (recommended) - Only
-                    EPU MRC files and Yifan's frame alignment require this
-                    to be off.
-
-    :Returns:
-
-    out : bool
-          True if the header conforms to MRC
-    """
-
-    global bad_mrc_header
-
-    if hasattr(filename, 'dtype'):
-        h = filename
-        if not is_format_header(h):
-            raise ValueError('Array dtype incorrect')
-    else:
-        try:
-            h = read_mrc_header(filename)
-        except BaseException:
-            return False
-    if _logger.isEnabledFor(logging.DEBUG):
-        _logger.debug('Mode: %d - %d' % (h['mode'][0], (h['mode'][0] not in mrc2numpy)))
-        _logger.debug('Byteorder: %d - %d' % (h['byteorder'][0], ((h['byteorder'][0] & -65536) not in intbyteorder)))
-        _logger.debug('Byteorder-swap: %d - %d' % ((h['byteorder'][0].byteswap() & -65536), ((h['byteorder'][0].byteswap() & -65536) not in intbyteorder)))
-        for name in ('alpha', 'beta', 'gamma'):
-            _logger.debug('%s: %f - %d' % (name, h[name][0], (h[name][0] != 90.0)))
-        for name in ('nx', 'ny', 'nz'):
-            _logger.debug('%s: %d - %d' % (name, h[name][0], (h[name][0] > 0)))
-    if h['mode'][0] not in mrc2numpy:
-        _logger.debug('Failed to read proper mode - not MRC!')
-        return False
-
-    if (h['byteorder'][0] & -65536) not in intbyteorder and \
-       (h['byteorder'][0].byteswap() & -65536) not in intbyteorder:
-        if h['alpha'][0] == 0.0 and h['beta'][0] == 0.0 and h['gamma'][0] == 0.0 and int(h['mode'][0]) == 6:  # this line hack for non-standard writers
-            if not bad_mrc_header:
-                bad_mrc_header = True
-                if not no_strict_mrc and 1 == 0:
-                    _logger.warn('This image could be MRC format likely this image came from EPU. Use --no-strict-mrc to read this image')
-                    return False
-                _logger.warn('Assuming image is MRC format - format is not correct (Likely this image came from EPU)')
-        elif h['alpha'][0] == 90.0 and h['beta'][0] == 90.0 and h['gamma'][0] == 90.0:  # this line hack for non-standard writers
-            if not bad_mrc_header:
-                bad_mrc_header = True
-                if not no_strict_mrc and 1 == 0:
-                    _logger.warn("This image could be MRC format likely this image came from Yifan's GPU alignment. Use --no-strict-mrc to read this image")
-                    return False
-                _logger.warn("Assuming image is MRC format - format is not correct (Likely this image came from Yifan's GPU alignment)")
-        else:
-            _logger.debug('Failed to read proper machine stamp - not MRC!')
-            # return False
-    if not numpy.alltrue([h[v][0] > 0 for v in ('nx', 'ny', 'nz')]):
-        _logger.debug('Failed to read proper dimensions - not MRC!')
-        return False
-    return True
-
-
-def read_header(filename, index=None, no_strict_mrc=False, force_volume=False):
-    """Read the MRC header.
-
-    :Parameters:
-
-    filename : str or file object
-               Filename or open stream for a file
-    index : int, ignored
-            Index of image to get the header, if None, the stack header (Default: None)
-    no_strict_mrc : bool
-                    Perform strict MRC header checking (recommended) - Only
-                    EPU MRC files and Yifan's frame alignment require this
-                    to be off.
-    force_volume : bool
-                   Force image to be treated as a volume
-
-    :Returns:
-
-    header : dict
-             Dictionary with header information
-    """
-
-    h = read_mrc_header(filename, index, no_strict_mrc) if not hasattr(filename, 'ndim') else filename
-    header = {}
-    header['apix'] = float(h['xlen'][0]) / float(h['nx'][0])
-    header['count'] = int(h['nz'][0]) if int(h['nz'][0]) != int(h['nx'][0]) and not force_volume else 1
-    header['nx'] = int(h['nx'][0])
-    header['ny'] = int(h['ny'][0])
-    header['nz'] = int(h['nz'][0]) if int(h['nz'][0]) == int(h['nx'][0]) or force_volume else 1
-    for key in h.dtype.fields.keys():
-        header['mrc_' + key] = h[key][0]
-    header['format'] = 'mrc'
-    return header
-
-
-def read_mrc_header(filename, index=None, no_strict_mrc=False):
-    """Read the MRC header.
-
-    :Parameters:
-
-    filename : str or file object
-               Filename or open stream for a file
-    index : int, ignored
-            Index of image to get the header, if None, the stack header (Default: None)
-    no_strict_mrc : bool
-                    Perform strict MRC header checking (recommended) - Only
-                    EPU MRC files and Yifan's frame alignment require this
-                    to be off.
-
-    :Returns:
-
-    out : array
-          Array with header information in the file
-    """
-
-    f = util.uopen(filename, 'rb')
-    try:
-        # curr = f.tell()
-        h = util.fromfile(f, dtype=header_image_dtype, count=1)
-        if not is_readable(h, no_strict_mrc):
-            h = h.newbyteorder()
-        if not is_readable(h, no_strict_mrc):
-            raise OSError('Not MRC header')
-    finally:
-        util.close(filename, f)
-    return h
-
-
-def is_volume(filename):
-    if hasattr(filename, 'dtype'):
-        h = filename
-    else:
-        h = read_mrc_header(filename)
-    return h['nz'][0] == h['nx'][0] and h['nz'][0] == h['ny'][0]
-
-
-def count_images(filename, no_strict_mrc=False):
-    """Count the number of images in the file.
-
-    :Parameters:
-
-    filename : str or file object
-               Filename or open stream for a file
-    no_strict_mrc : bool
-                    Perform strict MRC header checking (recommended) - Only
-                    EPU MRC files and Yifan's frame alignment require this
-                    to be off.
-
-    :Returns:
-
-    out : int
-          Number of images in the file
-    """
-
-    if hasattr(filename, 'dtype'):
-        h = filename
-    else:
-        h = read_mrc_header(filename, no_strict_mrc)
-    return h['nz'][0]
-
-
-def iter_images(filename, index=None, header=None, no_strict_mrc=False):
-    """Read a set of SPIDER images.
-
-    :Parameters:
-
-    filename : str or file object
-               Filename or open stream for a file
-    index : int, optional
-            Index of image to start, if None, start with the first image (Default: None)
-    header : dict, optional
-             Output dictionary to place header values
-    no_strict_mrc : bool
-                    Perform strict MRC header checking (recommended) - Only
-                    EPU MRC files and Yifan's frame alignment require this
-                    to be off.
-
-    :Returns:
-
-    out : array
-          Array with image information from the file
-    """
-
-    f = util.uopen(filename, 'rb')
-    if index is None:
-        index = 0
-    try:
-        h = read_mrc_header(f, no_strict_mrc)
-        count = count_images(h)
-        # if header is not None:  util.update_header(header, h, mrc2ara, 'mrc')
-        tmp = read_header(h)
-        if header is not None:
-            header.update(tmp)
-        d_len = h['nx'][0] * h['ny'][0]
-        dtype = numpy.dtype(mrc2numpy[h['mode'][0]])
-        offset = 1024 + int(h['nsymbt']) + 0 * d_len * dtype.itemsize
-        try:
-            f.seek(int(offset))
-        except BaseException:
-            _logger.error(f'{str(offset)} -- {str(offset.__class__.__name__)}')
-            raise
-        if not hasattr(index, '__iter__'):
-            index = range(index, count)
-        else:
-            index = index.astype(numpy.int)
-        last = 0
-        total = file_size(f)
-        if total != (1024 + int(h['nsymbt']) + int(h['nx'][0]) * int(h['ny'][0]) * int(h['nz'][0]) * dtype.itemsize):
-            raise util.InvalidHeaderException('file size != header: %d != %d -- %d' % (total, (1024 + int(h['nsymbt']) + int(h['nx'][0]) * int(h['ny'][0]) * int(h['nz'][0]) * dtype.itemsize), int(h['nsymbt'])))
-        for i in index:
-            if i != (last + 1):
-                f.seek(int(1024 + int(h['nsymbt']) + i * d_len * dtype.itemsize))
-            out = util.fromfile(f, dtype=dtype, count=d_len)
-
-            out = reshape_data(out, h, index, count)
-            if header_image_dtype.newbyteorder()[0] == h.dtype[0]:
-                out = out.byteswap()
-            yield out
-    finally:
-        util.close(filename, f)
-
-
-def valid_image(filename, no_strict_mrc=False):
-    """Test if the image is valid.
-
-    :Parameters:
-
-        filename : str
-                   Input filename to test
-        no_strict_mrc : bool
-                        Perform strict MRC header checking (recommended) - Only
-                        EPU MRC files and Yifan's frame alignment require this
-                        to be off.
-
-    :Returns:
-
-        flag : bool
-               True if image is valid
-    """
-
-    f = util.uopen(filename, 'rb')
-    try:
-        h = read_mrc_header(f, no_strict_mrc)
-        total = file_size(f)
-        dtype = numpy.dtype(mrc2numpy[h['mode'][0]])
-        return total == (1024 + int(h['nsymbt']) + int(h['nx'][0]) * int(h['ny'][0]) * int(h['nz'][0]) * dtype.itemsize)
-    finally:
-        util.close(filename, f)
-
-
-def read_image(filename, index=None, cache=None, no_strict_mrc=False, force_volume=False):
-    """Read an image from the specified file in the MRC format.
-
-    :Parameters:
-
-        filename : str or file object
-                   Filename or open stream for a file
-        index : int, optional
-                Index of image to get, if None, first image (Default: None)
-        no_strict_mrc : bool
-                        Perform strict MRC header checking (recommended) - Only
-                        EPU MRC files and Yifan's frame alignment require this
-                        to be off.
-        force_volume : bool
-                       For image to be read as a volume
-
-    :Returns:
-
-        out : array
-              Array with image information from the file
-    """
-
-    idx = 0 if index is None else index
-    f = util.uopen(filename, 'rb')
-    try:
-        h = read_mrc_header(f, no_strict_mrc)
-        # if header is not None: util.update_header(header, h, mrc2ara, 'mrc')
-        header = read_header(h, force_volume=force_volume)
-        count = count_images(h)
-        if idx >= count:
-            raise OSError('Index exceeds number of images in stack: %d < %d' % (idx, count))
-        if index is None and (count == h['nx'][0] or force_volume):
-            d_len = h['nx'][0] * h['ny'][0] * h['nz'][0]
-        else:
-            d_len = h['nx'][0] * h['ny'][0]
-        dtype = numpy.dtype(mrc2numpy[h['mode'][0]])
-        offset = 1024 + int(h['nsymbt']) + idx * d_len * dtype.itemsize
-        total = file_size(f)
-        if total != (1024 + int(h['nsymbt']) + int(h['nx'][0]) * int(h['ny'][0]) * int(h['nz'][0]) * dtype.itemsize):
-            raise util.InvalidHeaderException('file size != header: %d != %d -- %s, %d' % (total, (1024 + int(h['nsymbt']) + int(h['nx'][0]) * int(h['ny'][0]) * int(h['nz'][0]) * dtype.itemsize), str(idx), int(h['nsymbt'])))
-        f.seek(int(offset))
-        out = util.fromfile(f, dtype=dtype, count=d_len)
-        out = reshape_data(out, h, index, count, force_volume)
-        if header_image_dtype.newbyteorder()[0] == h.dtype[0]:
-            out = out.byteswap()
-    finally:
-        util.close(filename, f)
-    # assert(numpy.alltrue(numpy.logical_not(numpy.isnan(out))))
-    # if header_image_dtype.newbyteorder()==h.dtype:out = out.byteswap()
-    return out, header
-
-
-def reshape_data(out, h, index, count, force_volume=False):
-    """Reshape the data to the proper dimensions.
-
-    :Parameters:
-
-    out : array
-          Array with image information from the file
-    h : array
-        Header information
-    index : int
-            Index of image
-    count : int
-            Number of images in file
-
-    :Returns:
-
-    out : array
-          Array with image information from the file
-    """
-
-    if index is None and int(h['nz'][0]) > 1 and (count == h['nx'][0] or force_volume):
-        if h['mapc'][0] == 2 and h['mapr'][0] == 1:
-            out = out.reshape((int(h['nx'][0]), int(h['ny'][0]), int(h['nz'][0])))
-            for i in range(out.shape[2]):
-                out[:, :, i] = out[:, :, i].squeeze().T
-        else:
-            out = out.reshape((int(h['nx'][0]), int(h['ny'][0]), int(h['nz'][0])))
-    elif int(h['ny']) > 1:
-        if h['mapc'][0] == 2 and h['mapr'][0] == 1:
-            out = out.reshape((int(h['ny'][0]), int(h['nx'][0])))  # .transpose() # Test this!
-        else:
-            out = out.reshape((int(h['ny'][0]), int(h['nx'][0])))
-    return out
-
-
-def file_size(fileobject):
-    fileobject.seek(0, 2)  # move the cursor to the end of the file
-    size = fileobject.tell()
-    return size
-
-
-def is_writable(filename):
-    """Test if the image extension of the given filename is understood as a
-    writable format.
-
-    :Parameters:
-
-    filename : str
-               Output filename to test
-
-    :Returns:
-
-    write : bool
-            True if the format is recognized
-    """
-
-    ext = os.path.splitext(filename)[1][1:].lower()
-    return ext == 'mrc' or \
-        ext == 'ccp4' or \
-        ext == 'map'
-
-
-def write_image(filename, img, index=None, header=None, inplace=False):
-    """Write an image array to a file in the MRC format.
-
-    :Parameters:
-
-    filename : str
-               Name of the output file
-    img : array
-          Image array
-    index : int, optional
-            Index to write image in the stack
-    header : dict, optional
-             Dictionary of header values
-    inplace : bool
-              Write new image to stack without removing the stack
-    """
-
-    if header is None and hasattr(img, 'header'):
-        header = img.header
-    try:
-        img = img.astype(mrc2numpy[numpy2mrc[img.dtype.type]])
-    except BaseException:
-        raise TypeError('Unsupported type for MRC writing: %s' % str(img.dtype))
-
-    mode = 'rb+' if index is not None and (index > 0 or inplace and index > -1) else 'wb+'
-    f = util.uopen(filename, mode)
-    if header is None or not hasattr(header, 'dtype') or not is_format_header(header):
-        h = numpy.zeros(1, header_image_dtype)
-        util.update_header(h, mrc_defaults, ara2mrc)
-        pix = header.get('apix', 1.0) if header is not None else 1.0
-        header = util.update_header(h, header, ara2mrc, 'mrc')
-        header['nx'] = img.T.shape[0]
-        header['ny'] = img.T.shape[1] if img.ndim > 1 else 1
-        if header['nz'] == 0:
-            header['nz'] = img.shape[2] if img.ndim > 2 else 1
-        header['mode'] = numpy2mrc[img.dtype.type]
-        header['mx'] = header['nx']
-        header['my'] = header['ny']
-        header['mz'] = header['nz']
-        header['xlen'] = header['nx'] * pix
-        header['ylen'] = header['ny'] * pix
-        header['zlen'] = header['nz'] * pix
-        header['alpha'] = 90
-        header['beta'] = 90
-        header['gamma'] = 90
-        header['mapc'] = 1
-        header['mapr'] = 2
-        header['maps'] = 3
-        header['amin'] = numpy.min(img)
-        header['amax'] = numpy.max(img)
-        header['amean'] = numpy.mean(img)
-
-        header['map'] = 'MAP'
-        header['byteorder'] = byteorderint2[sys.byteorder]  # 'DA\x00\x00'
-        header['nlabels'] = 1
-        header['label0'] = 'Created by Instamatic'
-
-        # header['byteorder'] = numpy.fromstring('\x44\x41\x00\x00', dtype=header['byteorder'].dtype)
-
-        # header['rms'] = numpy.std(img)
-        if img.ndim == 3:
-            header['nxstart'] = header['nx'] / -2
-            header['nystart'] = header['ny'] / -2
-            header['nzstart'] = header['nz'] / -2
-        if index is not None:
-            stack_count = index + 1
-            header['nz'] = stack_count
-            header['mz'] = stack_count
-            header['zlen'] = stack_count
-            # header['zorigin'] = stack_count/2.0
-        else:
-            index = 0
-
-    try:
-        if inplace:
-            f.seek(int(1024 + int(h['nsymbt']) + index * img.ravel().shape[0] * img.dtype.itemsize))
-        elif f != filename:
-            f.seek(0)
-            header.tofile(f)
-            if index > 0:
-                f.seek(int(1024 + int(h['nsymbt']) + index * img.ravel().shape[0] * img.dtype.itemsize))
-        img.tofile(f)
-    finally:
-        util.close(filename, f)
-
-
-if __name__ == '__main__':
-    import numpy as np
-
-    from pathlib import Path
-
-    fn = Path('test.mrc')
-    img = (np.random.random((512, 512)) * 100000).astype(np.uint16)
-
-    header = {}
-    header['SIZE1'] = 512
-    header['SIZE2'] = 512
-
-    write_image(fn, img, header=header)
-    print('writing:', img.shape)
-    print('header:', header)
-    print()
-
-    arr, h = read_image(fn)
-    print('reading', arr.shape, arr.dtype)
-    print('header', h)
-
-    print()
-    print('allclose:', np.allclose(img, arr))
-
-    print(len(header_image_dtype))
+# https://github.com/ezralanglois/arachnid/blob/master/arachnid/core/image/formats/mrc.py
+# Licenced under GPL
+"""Read and write images in the MRC format.
+
+.. todo:: define arachnid header and map to mrc
+
+.. note::
+
+    This code is heavily modified version of the MRC parser/writer
+    found in the Scripps Appion program.
+
+
+.. Created on Aug 9, 2012
+.. codeauthor:: Robert Langlois <rl2528@columbia.edu>
+"""
+import logging
+import os
+import sys
+
+import numpy
+
+from . import util
+
+# import util
+
+_logger = logging.getLogger(__name__)
+_logger.setLevel(logging.INFO)
+
+mrc2numpy = {
+    0: numpy.int8,
+    1: numpy.int16,
+    2: numpy.float32,
+    3: numpy.dtype([('real', numpy.int16), ('imag', numpy.int16)]),
+    # complex made of two int16.  No such thing in numpy
+    #     however, we could manually build a complex array by reading two
+    #     int16 arrays somehow.
+    4: numpy.complex64,
+
+    6: numpy.uint16,    # according to UCSF
+    7: numpy.uint8,    # according to UCSF
+}
+
+# mapping of numpy type to MRC mode
+numpy2mrc = {
+    # convert these to int8
+    numpy.int8: 0,
+    #    numpy.uint8: 0,
+    numpy.bool_: 0,
+
+    # convert these to int16
+    numpy.int16: 1,
+    #    numpy.int8: 1,
+
+    # convert these to float32
+    numpy.float32: 2,
+    numpy.float64: 2,
+    numpy.int32: 2,
+    numpy.int64: 2,
+    numpy.uint32: 2,
+    numpy.uint64: 2,
+
+    # convert these to complex64
+    numpy.complex64: 4,
+    numpy.complex128: 4,
+
+    # convert these to uint16
+    numpy.uint16: 6,
+    numpy.uint8: 7,
+}
+
+intbyteorder = {
+    0x11110000: 'big',
+    0x44440000: 'little',  # hack
+    0x44410000: 'little',
+}
+byteorderint = {
+    'big': 0x11110000,
+    'little': 0x44410000,
+}
+byteorderint2 = {
+    'big': 286326784,
+    'little': 1145110528,
+}
+
+
+mrc_defaults = {'alpha': 90, 'beta': 90, 'gamma': 90, 'mapc': 1, 'mapr': 2, 'maps': 3, 'map': 'MAP ', 'byteorder': byteorderint[sys.byteorder]}
+
+
+def _gen_header():
+    """Create the header for an MRC image and stack.
+
+    .. note::
+
+        The following code was adopted from mrc.py in Scripps Appion Package
+
+    :Returns:
+
+    header_image_dtype : numpy.dtype
+                         Header for an MRC image
+    """
+
+    shared_fields = [
+        ('nx', numpy.int32),
+        ('ny', numpy.int32),
+        ('nz', numpy.int32),
+        ('mode', numpy.int32),
+        ('nxstart', numpy.int32),
+        ('nystart', numpy.int32),
+        ('nzstart', numpy.int32),
+        ('mx', numpy.int32),
+        ('my', numpy.int32),
+        ('mz', numpy.int32),
+        ('xlen', numpy.float32),
+        ('ylen', numpy.float32),
+        ('zlen', numpy.float32),
+        ('alpha', numpy.float32),  # defocus
+        ('beta', numpy.float32),  # astig_ang
+        ('gamma', numpy.float32),  # astig_mag
+        ('mapc', numpy.int32),
+        ('mapr', numpy.int32),
+        ('maps', numpy.int32),
+        ('amin', numpy.float32),
+        ('amax', numpy.float32),
+        ('amean', numpy.float32),
+        ('ispg', numpy.int32),
+        ('nsymbt', numpy.int32),
+    ]
+
+    header_image_dtype = numpy.dtype(shared_fields + [
+        ('extra', 'S100'),
+        ('xorigin', numpy.float32),  # 208 320  4   char    cmap;      Contains "MAP "
+        ('yorigin', numpy.float32),
+        ('zorigin', numpy.float32),
+        ('map', 'S4'),
+        ('byteorder', numpy.int32),
+        ('rms', numpy.float32),
+        ('nlabels', numpy.int32),
+        ('label0', 'S80'),
+        ('label1', 'S80'),  # Image Type
+        # Allow image `type`s are:
+        #    - Power Spectra: 'P'
+        #    - Windowed Particle: 'W'
+        #    - Micrograph: 'M'
+        ('label2', 'S80'),
+        ('label3', 'S80'),
+        ('label4', 'S80'),
+        ('label5', 'S80'),
+        ('label6', 'S80'),
+        ('label7', 'S80'),
+        ('label8', 'S80'),
+        ('label9', 'S80'),
+    ])
+
+    return header_image_dtype
+
+# --------------------------------------------------------------------
+# End attribution
+# --------------------------------------------------------------------
+
+
+header_image_dtype = _gen_header()
+
+mrc2ara = {'': ''}
+mrc2ara.update({h[0]: 'mrc' + h[0] for h in header_image_dtype.names})
+ara2mrc = {val: key for key, val in mrc2ara.items()}
+
+
+def create_header(shape, dtype, order='C', header=None):
+    """Create a header for the MRC image format.
+
+    @todo support header parameters
+
+    :Parameters:
+
+    shape : tuple
+            Shape of the array
+    dtype : numpy.dtype
+            Data type for NumPy ndarray
+    header : dict
+             Header values  for image
+    :Returns:
+
+    h : dtype
+        Data type for NumPy ndarray describing the header
+    """
+
+    pass
+
+
+def array_from_header(header):
+    """Convert header information to array parameters.
+
+    :Parameters:
+
+    header : header_dtype
+             Header fields
+
+    :Returns:
+
+    header : dict
+             File header
+    dtype : dtype
+            Data type
+    shape : tuple
+            Shape of the array
+    order : str
+            Order of the array
+    offset : int
+             Header offset
+    swap : bool
+            Swap byte order
+    """
+
+    pass
+
+
+def cache_data():
+    """Get keywords to be added as data cache.
+
+    :Returns:
+
+    extra : dict
+            Keyword arguments
+    """
+
+    return {'header': None, 'no_strict_mrc': False, 'force_volume': False}
+
+
+def is_format_header(h):
+    """Test if the given header has the proper format.
+
+    :Parameters:
+
+    h : array
+        Header to test
+
+    :Returns:
+
+    val : bool
+          Test if dtype matches format dtype
+    """
+
+    return h.dtype == header_image_dtype or h.dtype == header_image_dtype.newbyteorder()
+
+
+bad_mrc_header = False
+
+
+def is_readable(filename, no_strict_mrc=False):
+    """Test if the file read has a valid MRC header.
+
+    :Parameters:
+
+    filename : str or file object
+               Filename or open stream for a file
+    no_strict_mrc : bool
+                    Perform strict MRC header checking (recommended) - Only
+                    EPU MRC files and Yifan's frame alignment require this
+                    to be off.
+
+    :Returns:
+
+    out : bool
+          True if the header conforms to MRC
+    """
+
+    global bad_mrc_header
+
+    if hasattr(filename, 'dtype'):
+        h = filename
+        if not is_format_header(h):
+            raise ValueError('Array dtype incorrect')
+    else:
+        try:
+            h = read_mrc_header(filename)
+        except BaseException:
+            return False
+    if _logger.isEnabledFor(logging.DEBUG):
+        _logger.debug('Mode: %d - %d' % (h['mode'][0], (h['mode'][0] not in mrc2numpy)))
+        _logger.debug('Byteorder: %d - %d' % (h['byteorder'][0], ((h['byteorder'][0] & -65536) not in intbyteorder)))
+        _logger.debug('Byteorder-swap: %d - %d' % ((h['byteorder'][0].byteswap() & -65536), ((h['byteorder'][0].byteswap() & -65536) not in intbyteorder)))
+        for name in ('alpha', 'beta', 'gamma'):
+            _logger.debug('%s: %f - %d' % (name, h[name][0], (h[name][0] != 90.0)))
+        for name in ('nx', 'ny', 'nz'):
+            _logger.debug('%s: %d - %d' % (name, h[name][0], (h[name][0] > 0)))
+    if h['mode'][0] not in mrc2numpy:
+        _logger.debug('Failed to read proper mode - not MRC!')
+        return False
+
+    if (h['byteorder'][0] & -65536) not in intbyteorder and \
+       (h['byteorder'][0].byteswap() & -65536) not in intbyteorder:
+        if h['alpha'][0] == 0.0 and h['beta'][0] == 0.0 and h['gamma'][0] == 0.0 and int(h['mode'][0]) == 6:  # this line hack for non-standard writers
+            if not bad_mrc_header:
+                bad_mrc_header = True
+                if not no_strict_mrc and 1 == 0:
+                    _logger.warn('This image could be MRC format likely this image came from EPU. Use --no-strict-mrc to read this image')
+                    return False
+                _logger.warn('Assuming image is MRC format - format is not correct (Likely this image came from EPU)')
+        elif h['alpha'][0] == 90.0 and h['beta'][0] == 90.0 and h['gamma'][0] == 90.0:  # this line hack for non-standard writers
+            if not bad_mrc_header:
+                bad_mrc_header = True
+                if not no_strict_mrc and 1 == 0:
+                    _logger.warn("This image could be MRC format likely this image came from Yifan's GPU alignment. Use --no-strict-mrc to read this image")
+                    return False
+                _logger.warn("Assuming image is MRC format - format is not correct (Likely this image came from Yifan's GPU alignment)")
+        else:
+            _logger.debug('Failed to read proper machine stamp - not MRC!')
+            # return False
+    if not numpy.alltrue([h[v][0] > 0 for v in ('nx', 'ny', 'nz')]):
+        _logger.debug('Failed to read proper dimensions - not MRC!')
+        return False
+    return True
+
+
+def read_header(filename, index=None, no_strict_mrc=False, force_volume=False):
+    """Read the MRC header.
+
+    :Parameters:
+
+    filename : str or file object
+               Filename or open stream for a file
+    index : int, ignored
+            Index of image to get the header, if None, the stack header (Default: None)
+    no_strict_mrc : bool
+                    Perform strict MRC header checking (recommended) - Only
+                    EPU MRC files and Yifan's frame alignment require this
+                    to be off.
+    force_volume : bool
+                   Force image to be treated as a volume
+
+    :Returns:
+
+    header : dict
+             Dictionary with header information
+    """
+
+    h = read_mrc_header(filename, index, no_strict_mrc) if not hasattr(filename, 'ndim') else filename
+    header = {}
+    header['apix'] = float(h['xlen'][0]) / float(h['nx'][0])
+    header['count'] = int(h['nz'][0]) if int(h['nz'][0]) != int(h['nx'][0]) and not force_volume else 1
+    header['nx'] = int(h['nx'][0])
+    header['ny'] = int(h['ny'][0])
+    header['nz'] = int(h['nz'][0]) if int(h['nz'][0]) == int(h['nx'][0]) or force_volume else 1
+    for key in h.dtype.fields.keys():
+        header['mrc_' + key] = h[key][0]
+    header['format'] = 'mrc'
+    return header
+
+
+def read_mrc_header(filename, index=None, no_strict_mrc=False):
+    """Read the MRC header.
+
+    :Parameters:
+
+    filename : str or file object
+               Filename or open stream for a file
+    index : int, ignored
+            Index of image to get the header, if None, the stack header (Default: None)
+    no_strict_mrc : bool
+                    Perform strict MRC header checking (recommended) - Only
+                    EPU MRC files and Yifan's frame alignment require this
+                    to be off.
+
+    :Returns:
+
+    out : array
+          Array with header information in the file
+    """
+
+    f = util.uopen(filename, 'rb')
+    try:
+        # curr = f.tell()
+        h = util.fromfile(f, dtype=header_image_dtype, count=1)
+        if not is_readable(h, no_strict_mrc):
+            h = h.newbyteorder()
+        if not is_readable(h, no_strict_mrc):
+            raise OSError('Not MRC header')
+    finally:
+        util.close(filename, f)
+    return h
+
+
+def is_volume(filename):
+    if hasattr(filename, 'dtype'):
+        h = filename
+    else:
+        h = read_mrc_header(filename)
+    return h['nz'][0] == h['nx'][0] and h['nz'][0] == h['ny'][0]
+
+
+def count_images(filename, no_strict_mrc=False):
+    """Count the number of images in the file.
+
+    :Parameters:
+
+    filename : str or file object
+               Filename or open stream for a file
+    no_strict_mrc : bool
+                    Perform strict MRC header checking (recommended) - Only
+                    EPU MRC files and Yifan's frame alignment require this
+                    to be off.
+
+    :Returns:
+
+    out : int
+          Number of images in the file
+    """
+
+    if hasattr(filename, 'dtype'):
+        h = filename
+    else:
+        h = read_mrc_header(filename, no_strict_mrc)
+    return h['nz'][0]
+
+
+def iter_images(filename, index=None, header=None, no_strict_mrc=False):
+    """Read a set of SPIDER images.
+
+    :Parameters:
+
+    filename : str or file object
+               Filename or open stream for a file
+    index : int, optional
+            Index of image to start, if None, start with the first image (Default: None)
+    header : dict, optional
+             Output dictionary to place header values
+    no_strict_mrc : bool
+                    Perform strict MRC header checking (recommended) - Only
+                    EPU MRC files and Yifan's frame alignment require this
+                    to be off.
+
+    :Returns:
+
+    out : array
+          Array with image information from the file
+    """
+
+    f = util.uopen(filename, 'rb')
+    if index is None:
+        index = 0
+    try:
+        h = read_mrc_header(f, no_strict_mrc)
+        count = count_images(h)
+        # if header is not None:  util.update_header(header, h, mrc2ara, 'mrc')
+        tmp = read_header(h)
+        if header is not None:
+            header.update(tmp)
+        d_len = h['nx'][0] * h['ny'][0]
+        dtype = numpy.dtype(mrc2numpy[h['mode'][0]])
+        offset = 1024 + int(h['nsymbt']) + 0 * d_len * dtype.itemsize
+        try:
+            f.seek(int(offset))
+        except BaseException:
+            _logger.error(f'{str(offset)} -- {str(offset.__class__.__name__)}')
+            raise
+        if not hasattr(index, '__iter__'):
+            index = range(index, count)
+        else:
+            index = index.astype(numpy.int)
+        last = 0
+        total = file_size(f)
+        if total != (1024 + int(h['nsymbt']) + int(h['nx'][0]) * int(h['ny'][0]) * int(h['nz'][0]) * dtype.itemsize):
+            raise util.InvalidHeaderException('file size != header: %d != %d -- %d' % (total, (1024 + int(h['nsymbt']) + int(h['nx'][0]) * int(h['ny'][0]) * int(h['nz'][0]) * dtype.itemsize), int(h['nsymbt'])))
+        for i in index:
+            if i != (last + 1):
+                f.seek(int(1024 + int(h['nsymbt']) + i * d_len * dtype.itemsize))
+            out = util.fromfile(f, dtype=dtype, count=d_len)
+
+            out = reshape_data(out, h, index, count)
+            if header_image_dtype.newbyteorder()[0] == h.dtype[0]:
+                out = out.byteswap()
+            yield out
+    finally:
+        util.close(filename, f)
+
+
+def valid_image(filename, no_strict_mrc=False):
+    """Test if the image is valid.
+
+    :Parameters:
+
+        filename : str
+                   Input filename to test
+        no_strict_mrc : bool
+                        Perform strict MRC header checking (recommended) - Only
+                        EPU MRC files and Yifan's frame alignment require this
+                        to be off.
+
+    :Returns:
+
+        flag : bool
+               True if image is valid
+    """
+
+    f = util.uopen(filename, 'rb')
+    try:
+        h = read_mrc_header(f, no_strict_mrc)
+        total = file_size(f)
+        dtype = numpy.dtype(mrc2numpy[h['mode'][0]])
+        return total == (1024 + int(h['nsymbt']) + int(h['nx'][0]) * int(h['ny'][0]) * int(h['nz'][0]) * dtype.itemsize)
+    finally:
+        util.close(filename, f)
+
+
+def read_image(filename, index=None, cache=None, no_strict_mrc=False, force_volume=False):
+    """Read an image from the specified file in the MRC format.
+
+    :Parameters:
+
+        filename : str or file object
+                   Filename or open stream for a file
+        index : int, optional
+                Index of image to get, if None, first image (Default: None)
+        no_strict_mrc : bool
+                        Perform strict MRC header checking (recommended) - Only
+                        EPU MRC files and Yifan's frame alignment require this
+                        to be off.
+        force_volume : bool
+                       For image to be read as a volume
+
+    :Returns:
+
+        out : array
+              Array with image information from the file
+    """
+
+    idx = 0 if index is None else index
+    f = util.uopen(filename, 'rb')
+    try:
+        h = read_mrc_header(f, no_strict_mrc)
+        # if header is not None: util.update_header(header, h, mrc2ara, 'mrc')
+        header = read_header(h, force_volume=force_volume)
+        count = count_images(h)
+        if idx >= count:
+            raise OSError('Index exceeds number of images in stack: %d < %d' % (idx, count))
+        if index is None and (count == h['nx'][0] or force_volume):
+            d_len = h['nx'][0] * h['ny'][0] * h['nz'][0]
+        else:
+            d_len = h['nx'][0] * h['ny'][0]
+        dtype = numpy.dtype(mrc2numpy[h['mode'][0]])
+        offset = 1024 + int(h['nsymbt']) + idx * d_len * dtype.itemsize
+        total = file_size(f)
+        if total != (1024 + int(h['nsymbt']) + int(h['nx'][0]) * int(h['ny'][0]) * int(h['nz'][0]) * dtype.itemsize):
+            raise util.InvalidHeaderException('file size != header: %d != %d -- %s, %d' % (total, (1024 + int(h['nsymbt']) + int(h['nx'][0]) * int(h['ny'][0]) * int(h['nz'][0]) * dtype.itemsize), str(idx), int(h['nsymbt'])))
+        f.seek(int(offset))
+        out = util.fromfile(f, dtype=dtype, count=d_len)
+        out = reshape_data(out, h, index, count, force_volume)
+        if header_image_dtype.newbyteorder()[0] == h.dtype[0]:
+            out = out.byteswap()
+    finally:
+        util.close(filename, f)
+    # assert(numpy.alltrue(numpy.logical_not(numpy.isnan(out))))
+    # if header_image_dtype.newbyteorder()==h.dtype:out = out.byteswap()
+    return out, header
+
+
+def reshape_data(out, h, index, count, force_volume=False):
+    """Reshape the data to the proper dimensions.
+
+    :Parameters:
+
+    out : array
+          Array with image information from the file
+    h : array
+        Header information
+    index : int
+            Index of image
+    count : int
+            Number of images in file
+
+    :Returns:
+
+    out : array
+          Array with image information from the file
+    """
+
+    if index is None and int(h['nz'][0]) > 1 and (count == h['nx'][0] or force_volume):
+        if h['mapc'][0] == 2 and h['mapr'][0] == 1:
+            out = out.reshape((int(h['nx'][0]), int(h['ny'][0]), int(h['nz'][0])))
+            for i in range(out.shape[2]):
+                out[:, :, i] = out[:, :, i].squeeze().T
+        else:
+            out = out.reshape((int(h['nx'][0]), int(h['ny'][0]), int(h['nz'][0])))
+    elif int(h['ny']) > 1:
+        if h['mapc'][0] == 2 and h['mapr'][0] == 1:
+            out = out.reshape((int(h['ny'][0]), int(h['nx'][0])))  # .transpose() # Test this!
+        else:
+            out = out.reshape((int(h['ny'][0]), int(h['nx'][0])))
+    return out
+
+
+def file_size(fileobject):
+    fileobject.seek(0, 2)  # move the cursor to the end of the file
+    size = fileobject.tell()
+    return size
+
+
+def is_writable(filename):
+    """Test if the image extension of the given filename is understood as a
+    writable format.
+
+    :Parameters:
+
+    filename : str
+               Output filename to test
+
+    :Returns:
+
+    write : bool
+            True if the format is recognized
+    """
+
+    ext = os.path.splitext(filename)[1][1:].lower()
+    return ext == 'mrc' or \
+        ext == 'ccp4' or \
+        ext == 'map'
+
+
+def write_image(filename, img, index=None, header=None, inplace=False):
+    """Write an image array to a file in the MRC format.
+
+    :Parameters:
+
+    filename : str
+               Name of the output file
+    img : array
+          Image array
+    index : int, optional
+            Index to write image in the stack
+    header : dict, optional
+             Dictionary of header values
+    inplace : bool
+              Write new image to stack without removing the stack
+    """
+
+    if header is None and hasattr(img, 'header'):
+        header = img.header
+    try:
+        img = img.astype(mrc2numpy[numpy2mrc[img.dtype.type]])
+    except BaseException:
+        raise TypeError('Unsupported type for MRC writing: %s' % str(img.dtype))
+
+    mode = 'rb+' if index is not None and (index > 0 or inplace and index > -1) else 'wb+'
+    f = util.uopen(filename, mode)
+    if header is None or not hasattr(header, 'dtype') or not is_format_header(header):
+        h = numpy.zeros(1, header_image_dtype)
+        util.update_header(h, mrc_defaults, ara2mrc)
+        pix = header.get('apix', 1.0) if header is not None else 1.0
+        header = util.update_header(h, header, ara2mrc, 'mrc')
+        header['nx'] = img.T.shape[0]
+        header['ny'] = img.T.shape[1] if img.ndim > 1 else 1
+        if header['nz'] == 0:
+            header['nz'] = img.shape[2] if img.ndim > 2 else 1
+        header['mode'] = numpy2mrc[img.dtype.type]
+        header['mx'] = header['nx']
+        header['my'] = header['ny']
+        header['mz'] = header['nz']
+        header['xlen'] = header['nx'] * pix
+        header['ylen'] = header['ny'] * pix
+        header['zlen'] = header['nz'] * pix
+        header['alpha'] = 90
+        header['beta'] = 90
+        header['gamma'] = 90
+        header['mapc'] = 1
+        header['mapr'] = 2
+        header['maps'] = 3
+        header['amin'] = numpy.min(img)
+        header['amax'] = numpy.max(img)
+        header['amean'] = numpy.mean(img)
+
+        header['map'] = 'MAP'
+        header['byteorder'] = byteorderint2[sys.byteorder]  # 'DA\x00\x00'
+        header['nlabels'] = 1
+        header['label0'] = 'Created by Instamatic'
+
+        # header['byteorder'] = numpy.fromstring('\x44\x41\x00\x00', dtype=header['byteorder'].dtype)
+
+        # header['rms'] = numpy.std(img)
+        if img.ndim == 3:
+            header['nxstart'] = header['nx'] / -2
+            header['nystart'] = header['ny'] / -2
+            header['nzstart'] = header['nz'] / -2
+        if index is not None:
+            stack_count = index + 1
+            header['nz'] = stack_count
+            header['mz'] = stack_count
+            header['zlen'] = stack_count
+            # header['zorigin'] = stack_count/2.0
+        else:
+            index = 0
+
+    try:
+        if inplace:
+            f.seek(int(1024 + int(h['nsymbt']) + index * img.ravel().shape[0] * img.dtype.itemsize))
+        elif f != filename:
+            f.seek(0)
+            header.tofile(f)
+            if index > 0:
+                f.seek(int(1024 + int(h['nsymbt']) + index * img.ravel().shape[0] * img.dtype.itemsize))
+        img.tofile(f)
+    finally:
+        util.close(filename, f)
+
+
+if __name__ == '__main__':
+    from pathlib import Path
+
+    import numpy as np
+
+    fn = Path('test.mrc')
+    img = (np.random.random((512, 512)) * 100000).astype(np.uint16)
+
+    header = {}
+    header['SIZE1'] = 512
+    header['SIZE2'] = 512
+
+    write_image(fn, img, header=header)
+    print('writing:', img.shape)
+    print('header:', header)
+    print()
+
+    arr, h = read_image(fn)
+    print('reading', arr.shape, arr.dtype)
+    print('header', h)
+
+    print()
+    print('allclose:', np.allclose(img, arr))
+
+    print(len(header_image_dtype))
```

### Comparing `instamatic-1.8.0/instamatic/formats/util.py` & `instamatic-1.9.0/instamatic/formats/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,28 +7,26 @@
 import logging
 import os
 
 import numpy
 import numpy as np
 from scipy import ndimage
 
-
 _logger = logging.getLogger(__name__)
 _logger.setLevel(logging.DEBUG)
 
 
 class InvalidHeaderException(Exception):
     """Thrown when the image file has an invalid header."""
 
     pass
 
 
 def fromfile(fin, dtype, count, sep=''):
     """"""
-
     if hasattr(fin, 'fileno'):
         return np.fromfile(fin, dtype, count, sep)
     else:
         return np.frombuffer(fin.read(count * dtype.itemsize), dtype, count)
 
 
 def uopen(filename, mode):
@@ -42,15 +40,14 @@
            Mode to open file
 
     :Returns:
 
     fd : File
          File descriptor
     """
-
     try:
         os.fspath(filename)
     except BaseException:
         f = filename
     else:
         if os.path.splitext(filename)[1] == '.bz2':
             f = bz2.BZ2File(filename, mode)
@@ -67,15 +64,14 @@
     """Close the file descriptor (if it was opened by caller)
 
     filename : str
                Name of the file
     fd : File
          File descriptor
     """
-
     if fd != filename:
         fd.close()
 
 
 def update_header(dest, source, header_map, tag=None):
     """Map values from or to the format and the internal header.
 
@@ -91,15 +87,14 @@
           Format specific attribute tag
 
     :Returns:
 
     dest : array or dict
            Destination of the header values
     """
-
     if source is None:
         return dest
     keys = dest.dtype.names if hasattr(dest, 'dtype') else dest.keys()
     tag = None
     for key in keys:
         try:
             dest[key] = source[header_map.get(key, key)]
@@ -133,15 +128,14 @@
             Layout of a 2 or 3D array
 
     :Returns:
 
     out : ndarray
           Array of image data
     """
-
     out = np.fromfile(f, dtype=dtype, count=dlen)
     out.shape = shape
     out = out.squeeze()
     if order == 'F':
         out.shape = out.shape[::-1]
         out = out.transpose()
     if swap:
```

### Comparing `instamatic-1.8.0/instamatic/goniotool.py` & `instamatic-1.9.0/instamatic/goniotool.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 import subprocess as sp
 import time
 from functools import wraps
 
 from pywinauto import Application
 
 from instamatic import config
-from instamatic.exceptions import exception_list
-from instamatic.exceptions import TEMCommunicationError
-from instamatic.server.serializer import dumper
-from instamatic.server.serializer import loader
+from instamatic.exceptions import TEMCommunicationError, exception_list
+from instamatic.server.serializer import dumper, loader
 
 GONIOTOOL_EXE = 'C:\\JEOL\\TOOL\\GonioTool.exe'
 DEFAULT_SPEED = 12
 
 HOST = config.settings.goniotool_server_host
 PORT = config.settings.goniotool_server_port
 BUFSIZE = 1024
@@ -92,15 +90,14 @@
                    'kwargs': kwargs}
             return self._eval_dct(dct)
 
         return wrapper
 
     def _eval_dct(self, dct):
         """Takes approximately 0.2-0.3 ms per call if HOST=='localhost'."""
-
         self.s.send(dumper(dct))
         response = self.s.recv(self._bufsize)
         if response:
             status, data = loader(response)
 
         if status == 200:
             return data
@@ -187,15 +184,15 @@
     def click_cmd(self):
         """Select CMD radio button."""
         self.rb_cmd.click()
 
     def set_rate(self, speed: int):
         """Set rate value for TX."""
         assert isinstance(speed, int), f'Variable `speed` must be of type `int`, is `{type(speed)}`'
-        assert 0 < speed <= 12, f'Variable `speed` must have a value of 1 to 12.'
+        assert 0 < speed <= 12, 'Variable `speed` must have a value of 1 to 12.'
 
         s = self.edit.select()
         s.set_text(speed)
         self.click_set_button()
 
     def get_rate(self) -> int:
         """Get current rate value for TX."""
```

### Comparing `instamatic-1.8.0/instamatic/gridmontage.py` & `instamatic-1.9.0/instamatic/gridmontage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import matplotlib.pyplot as plt
 import numpy as np
-from pyserialem.montage import make_grid
-from pyserialem.montage import sorted_grid_indices
+from pyserialem.montage import make_grid, sorted_grid_indices
 
-from .montage import *
 from instamatic import config
 from instamatic.config import defaults
 
+from .montage import *
+
 
 class GridMontage:
     """Set up an automated montage map."""
 
     def __init__(self, ctrl):
         super().__init__()
         self.ctrl = ctrl
```

### Comparing `instamatic-1.8.0/instamatic/gui/about_frame.py` & `instamatic-1.9.0/instamatic/gui/about_frame.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-from tkinter import *
-from tkinter import Label as tkLabel
-from tkinter.font import Font
-from tkinter.font import nametofont
-from tkinter.ttk import *
-
-import instamatic
-from .base_module import BaseModule
-
-
-def get_background_of_widget(widget):
-    """http://code.activestate.com/recipes/580774-tkinter-link-or-hyperlink-
-    button/"""
-    try:
-        # We assume first tk widget
-        background = widget.cget('background')
-    except BaseException:
-        # Otherwise this is a ttk widget
-        style = widget.cget('style')
-
-        if style == '':
-            # if there is not style configuration option, default style is the same than widget class
-            style = widget.winfo_class()
-
-        background = Style().lookup(style, 'background')
-
-    return background
-
-
-class Link_Button(tkLabel):
-    """http://code.activestate.com/recipes/580774-tkinter-link-or-hyperlink-
-    button/"""
-
-    def __init__(self, master, text, background=None, font=None, familiy=None, size=None, underline=True, visited_fg='#551A8B', normal_fg='#0000EE', visited=False, action=None):
-        self._visited_fg = visited_fg
-        self._normal_fg = normal_fg
-
-        if visited:
-            fg = self._visited_fg
-        else:
-            fg = self._normal_fg
-
-        if font is None:
-            default_font = nametofont('TkDefaultFont')
-            family = default_font.cget('family')
-
-            if size is None:
-                size = default_font.cget('size')
-
-            font = Font(family=family, size=size, underline=underline)
-
-        tkLabel.__init__(self, master, text=text, fg=fg, cursor='hand2', font=font)
-
-        if background is None:
-            background = get_background_of_widget(master)
-
-        self.configure(background=background)
-
-        self._visited = visited
-        self._action = action
-
-        self.bind('<Button-1>', self._on_click)
-
-    @property
-    def visited(self):
-        return self._visited
-
-    @visited.setter
-    def visited(self, is_visited):
-        if is_visited:
-            self.configure(fg=self._visited_fg)
-            self._visited = True
-        else:
-            self.configure(fg=self._normal_fg)
-            self._visited = False
-
-    def _on_click(self, event):
-        if not self._visited:
-            self.configure(fg=self._visited_fg)
-
-        self._visited = True
-
-        if self._action:
-            self._action()
-
-
-class AboutFrame(LabelFrame):
-    """`About` panel for the GUI."""
-
-    def __init__(self, parent):
-        LabelFrame.__init__(self, parent, text='About instamatic')
-        self.parent = parent
-
-        frame = Frame(self)
-
-        Label(frame, text='').grid(row=0, column=0, sticky='W')
-        Label(frame, text='Contact:').grid(row=1, column=0, sticky='W', padx=10)
-        Label(frame, text=f'{instamatic.__author__} ({instamatic.__author_email__}').grid(row=1, column=1, sticky='W')
-        Label(frame, text='').grid(row=5, column=0, sticky='W')
-
-        Label(frame, text='Source code:').grid(row=10, column=0, sticky='W', padx=10)
-        link = Link_Button(frame, text=instamatic.__url__, action=self.link_github)
-        link.grid(row=10, column=1, sticky='W')
-        Label(frame, text='').grid(row=12, column=0, sticky='W')
-
-        Label(frame, text='Docs:').grid(row=20, column=0, sticky='W', padx=10)
-        link = Link_Button(frame, text=instamatic.__docs__, action=self.link_github)
-        link.grid(row=20, column=1, sticky='W')
-        Label(frame, text='').grid(row=22, column=0, sticky='W')
-
-        Label(frame, text='Bugs:').grid(row=30, column=0, sticky='W', padx=10)
-        link = Link_Button(frame, text=instamatic.__issues__, action=self.link_github)
-        link.grid(row=30, column=1, sticky='W')
-        Label(frame, text='').grid(row=32, column=0, sticky='W')
-
-        Label(frame, text='If you found this software useful, please cite:').grid(row=40, column=0, sticky='W', columnspan=2, padx=10)
-        txt = Message(frame, text=instamatic.__citation__, width=320, justify=LEFT)
-        txt.grid(row=41, column=1, sticky='W')
-
-        Label(frame, text='').grid(row=41, column=0, sticky='W', padx=10)
-
-        frame.pack(side='top', fill='x')
-
-    def link_github(self, event=None):
-        import webbrowser
-        webbrowser.open_new(instamatic.__url__)
-
-    def link_manual(self, event=None):
-        import webbrowser
-        webbrowser.open_new(instamatic.__url__)
-
-
-module = BaseModule(name='about', display_name='about', tk_frame=AboutFrame, location='bottom')
-commands = {}
-
-
-if __name__ == '__main__':
-    root = Tk()
-    About(root).pack(side='top', fill='both', expand=True)
-    root.mainloop()
+from tkinter import *
+from tkinter import Label as tkLabel
+from tkinter.font import Font, nametofont
+from tkinter.ttk import *
+
+import instamatic
+
+from .base_module import BaseModule
+
+
+def get_background_of_widget(widget):
+    """http://code.activestate.com/recipes/580774-tkinter-link-or-hyperlink-
+    button/"""
+    try:
+        # We assume first tk widget
+        background = widget.cget('background')
+    except BaseException:
+        # Otherwise this is a ttk widget
+        style = widget.cget('style')
+
+        if style == '':
+            # if there is not style configuration option, default style is the same than widget class
+            style = widget.winfo_class()
+
+        background = Style().lookup(style, 'background')
+
+    return background
+
+
+class Link_Button(tkLabel):
+    """http://code.activestate.com/recipes/580774-tkinter-link-or-hyperlink-
+    button/"""
+
+    def __init__(self, master, text, background=None, font=None, familiy=None, size=None, underline=True, visited_fg='#551A8B', normal_fg='#0000EE', visited=False, action=None):
+        self._visited_fg = visited_fg
+        self._normal_fg = normal_fg
+
+        if visited:
+            fg = self._visited_fg
+        else:
+            fg = self._normal_fg
+
+        if font is None:
+            default_font = nametofont('TkDefaultFont')
+            family = default_font.cget('family')
+
+            if size is None:
+                size = default_font.cget('size')
+
+            font = Font(family=family, size=size, underline=underline)
+
+        tkLabel.__init__(self, master, text=text, fg=fg, cursor='hand2', font=font)
+
+        if background is None:
+            background = get_background_of_widget(master)
+
+        self.configure(background=background)
+
+        self._visited = visited
+        self._action = action
+
+        self.bind('<Button-1>', self._on_click)
+
+    @property
+    def visited(self):
+        return self._visited
+
+    @visited.setter
+    def visited(self, is_visited):
+        if is_visited:
+            self.configure(fg=self._visited_fg)
+            self._visited = True
+        else:
+            self.configure(fg=self._normal_fg)
+            self._visited = False
+
+    def _on_click(self, event):
+        if not self._visited:
+            self.configure(fg=self._visited_fg)
+
+        self._visited = True
+
+        if self._action:
+            self._action()
+
+
+class AboutFrame(LabelFrame):
+    """`About` panel for the GUI."""
+
+    def __init__(self, parent):
+        LabelFrame.__init__(self, parent, text='About instamatic')
+        self.parent = parent
+
+        frame = Frame(self)
+
+        Label(frame, text='').grid(row=0, column=0, sticky='W')
+        Label(frame, text='Contact:').grid(row=1, column=0, sticky='W', padx=10)
+        Label(frame, text=f'{instamatic.__author__} ({instamatic.__author_email__}').grid(row=1, column=1, sticky='W')
+        Label(frame, text='').grid(row=5, column=0, sticky='W')
+
+        Label(frame, text='Source code:').grid(row=10, column=0, sticky='W', padx=10)
+        link = Link_Button(frame, text=instamatic.__url__, action=self.link_github)
+        link.grid(row=10, column=1, sticky='W')
+        Label(frame, text='').grid(row=12, column=0, sticky='W')
+
+        Label(frame, text='Docs:').grid(row=20, column=0, sticky='W', padx=10)
+        link = Link_Button(frame, text=instamatic.__docs__, action=self.link_github)
+        link.grid(row=20, column=1, sticky='W')
+        Label(frame, text='').grid(row=22, column=0, sticky='W')
+
+        Label(frame, text='Bugs:').grid(row=30, column=0, sticky='W', padx=10)
+        link = Link_Button(frame, text=instamatic.__issues__, action=self.link_github)
+        link.grid(row=30, column=1, sticky='W')
+        Label(frame, text='').grid(row=32, column=0, sticky='W')
+
+        Label(frame, text='If you found this software useful, please cite:').grid(row=40, column=0, sticky='W', columnspan=2, padx=10)
+        txt = Message(frame, text=instamatic.__citation__, width=320, justify=LEFT)
+        txt.grid(row=41, column=1, sticky='W')
+
+        Label(frame, text='').grid(row=41, column=0, sticky='W', padx=10)
+
+        frame.pack(side='top', fill='x')
+
+    def link_github(self, event=None):
+        import webbrowser
+        webbrowser.open_new(instamatic.__url__)
+
+    def link_manual(self, event=None):
+        import webbrowser
+        webbrowser.open_new(instamatic.__url__)
+
+
+module = BaseModule(name='about', display_name='about', tk_frame=AboutFrame, location='bottom')
+commands = {}
+
+
+if __name__ == '__main__':
+    root = Tk()
+    About(root).pack(side='top', fill='both', expand=True)
+    root.mainloop()
```

### Comparing `instamatic-1.8.0/instamatic/gui/autocred_frame.py` & `instamatic-1.9.0/instamatic/gui/autocred_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 import threading
 from pathlib import Path
 from tkinter import *
 from tkinter.ttk import *
 
 import matplotlib.pyplot as plt
 
-from .base_module import BaseModule
 from instamatic import config
 from instamatic.calibrate import CalibBeamShift
 from instamatic.calibrate.filenames import *
 
+from .base_module import BaseModule
+
 
 class ExperimentalautocRED(LabelFrame):
     """Data collection protocol for SerialRED data collection on a high-speed
     Timepix camera using automated screening and crystal tracking.
 
     Related publication:     IUCrJ (2019). 6(5), 854-867
-    https://doi.org/10.1107/S2052252519007681 .
+    https://doi.org/10.1107/S2052252519007681
+    .
     """
 
     def __init__(self, parent):
         LabelFrame.__init__(self, parent, text='Serial Rotation Electron Diffraction (SerialRED)')
         self.parent = parent
 
         self.init_vars()
```

### Comparing `instamatic-1.8.0/instamatic/gui/base_module.py` & `instamatic-1.9.0/instamatic/gui/base_module.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/gui/console_frame.py` & `instamatic-1.9.0/instamatic/gui/console_frame.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import time
 from pathlib import Path
 from tkinter import *
 from tkinter import filedialog
 from tkinter.scrolledtext import ScrolledText
 from tkinter.ttk import *
 
-from .base_module import BaseModule
 from instamatic import config
 
+from .base_module import BaseModule
+
 
 class Writer:
     """Overwrite stdout with this class to write to a tkinter text widget.
 
     text: `tkinter.Text`
         Tkinter text / scrolledtext widget to redirect stdout to
     """
@@ -123,15 +124,14 @@
 
     def clear_text(self):
         """Clear the text in the console."""
         self.text.delete('0.0', END)
 
     def export_text(self):
         """Export text from the text widget to a file."""
-
         drc = config.settings.work_directory
 
         f = filedialog.asksaveasfile(mode='w',
                                      defaultextension='.txt',
                                      filetypes=(('Text', '*.txt'),),
                                      initialdir=drc,
                                      initialfile='console.txt')
```

### Comparing `instamatic-1.8.0/instamatic/gui/cred_fei_frame.py` & `instamatic-1.9.0/instamatic/gui/cred_fei_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from tkinter import *
 from tkinter.ttk import *
 
-from .base_module import BaseModule
 from instamatic.utils.spinbox import Spinbox
 
+from .base_module import BaseModule
+
 
 class ExperimentalcRED_FEI(LabelFrame):
     """Simple panel to assist cRED data collection (mainly rotation control) on
     a FEI microscope."""
 
     def __init__(self, parent):
         LabelFrame.__init__(self, parent, text='cRED_FEI')
```

### Comparing `instamatic-1.8.0/instamatic/gui/cred_frame.py` & `instamatic-1.9.0/instamatic/gui/cred_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import threading
 from tkinter import *
 from tkinter.ttk import *
 
-from .base_module import BaseModule
 from instamatic.utils.spinbox import Spinbox
 
+from .base_module import BaseModule
+
 ENABLE_FOOTFREE_OPTION = False
 
 
 class ExperimentalcRED(LabelFrame):
     """GUI panel for doing cRED experiments on a Timepix camera."""
 
     def __init__(self, parent):
```

### Comparing `instamatic-1.8.0/instamatic/gui/cred_tvips_frame.py` & `instamatic-1.9.0/instamatic/gui/cred_tvips_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import threading
 from pathlib import Path
 from tkinter import *
 from tkinter import filedialog
 from tkinter.ttk import *
 
-from .base_module import BaseModule
 from instamatic import config
 from instamatic.utils.spinbox import Spinbox
 
+from .base_module import BaseModule
+
 barrier = threading.Barrier(2, timeout=60)
 
 
 class ExperimentalTVIPS(LabelFrame):
     """GUI panel for doing cRED / SerialRED experiments on a TVIPS camera."""
 
     def __init__(self, parent):
```

### Comparing `instamatic-1.8.0/instamatic/gui/ctrl_frame.py` & `instamatic-1.9.0/instamatic/gui/ctrl_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import threading
 from tkinter import *
 from tkinter.ttk import *
 
-from .base_module import BaseModule
 from instamatic import config
 from instamatic.utils.spinbox import Spinbox
 
+from .base_module import BaseModule
+
 
 class ExperimentalCtrl(LabelFrame):
     """This panel holds some frequently used functions to control the electron
     microscope."""
 
     def __init__(self, parent):
         LabelFrame.__init__(self, parent, text='Stage Control')
```

### Comparing `instamatic-1.8.0/instamatic/gui/debug_frame.py` & `instamatic-1.9.0/instamatic/gui/debug_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import socket
 import tkinter.filedialog
 from pathlib import Path
 from tkinter import *
 from tkinter.ttk import *
 
-from .base_module import BaseModule
 from instamatic import config
 
+from .base_module import BaseModule
+
 scripts_drc = config.locations['scripts']
 
 SERVER_EXE = config.settings.indexing_server_exe
 HOST = config.settings.indexing_server_host
 PORT = config.settings.indexing_server_port
 BUFSIZE = 1024
 
@@ -228,15 +229,15 @@
         self.q.put(('debug', {'task': 'report_status'}))
         self.triggerEvent.set()
 
     def close_down(self):
         script = self.scripts_drc / 'close_down.py'
         # print(script, script.exists())
         if not script.exists():
-            return IOError(f'No such script: {script}')
+            return OSError(f'No such script: {script}')
         self.q.put(('debug', {'task': 'run_script', 'script': script}))
         self.triggerEvent.set()
 
     def browse(self):
         fn = tkinter.filedialog.askopenfilename(parent=self.parent, title='Select Python script')
         if not fn:
             return
@@ -286,15 +287,14 @@
     elif task == 'run_script':
         ctrl = controller.ctrl
         script = kwargs.pop('script')
         ctrl.run_script(script)
 
 
 def autoindex(controller, **kwargs):
-
     task = kwargs.get('task')
     if task == 'start_server':
         import subprocess as sp
         # cmd = "start /wait cmd /c instamatic.dialsserver"
         cmd = f'start {SERVER_EXE}'
         controller.indexing_server_process = sp.call(cmd, shell=True)
         print(f'Indexing server `{SERVER_EXE}` started on {HOST}:{PORT}')
@@ -323,15 +323,14 @@
         print(data)
 
     if task == 'kill':
         del controller.indexing_server_process
 
 
 def autoindex_xdsVM(controller, **kwargs):
-
     task = kwargs.get('task')
     if task == 'start_server_xdsVM':
         import subprocess as sp
 
         compos = kwargs.get('compos')
         unitcell = kwargs.get('unitcell')
         spgr = kwargs.get('spgr')
@@ -351,21 +350,21 @@
                     cmd += ' -s '
                     cmd += spgr
             else:
                 print('No composition information provided. SHELXT cannot run.')
 
         controller.indexing_server_process = sp.call(cmd, shell=True)
         print(f'Indexing server `{VM_SERVER_EXE}` starting on {VMHOST}:{VMPORT}')
-        #controller.use_indexing_server_xds = True
+        # controller.use_indexing_server_xds = True
         print('VM XDS Indexing server registered. Please wait for around 2 min before XDS server is ready.')
         print('Please refer to the server console for the current status of the server.')
         return
 
     elif task == 'register_server_xdsVM':
-        #controller.use_indexing_server_xds = True
+        # controller.use_indexing_server_xds = True
         print('VM XDS Indexing server registered')
         return
 
     elif task == 'run':
         payload = bytes(kwargs.get('path'))
 
     elif task == 'kill_server_xdsVM':
```

### Comparing `instamatic-1.8.0/instamatic/gui/defocus_button.py` & `instamatic-1.9.0/instamatic/gui/defocus_button.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,13 +72,13 @@
     root = Tk()
     DefocusButton(root).pack(side='top', fill='both', expand=True, padx=10, pady=10)
     root.lift()
 
     # keep window in front of other windows
     root.attributes('-topmost', True)
 
-    root.title(f'Instamatic defocus helper')
+    root.title('Instamatic defocus helper')
     root.mainloop()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `instamatic-1.8.0/instamatic/gui/gui.py` & `instamatic-1.9.0/instamatic/gui/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import sys
 import threading
 import traceback
 from tkinter import *
 from tkinter.ttk import *
 
 import instamatic
-from .modules import JOBS
-from .modules import MODULES
 from instamatic.formats import *
 
+from .modules import JOBS, MODULES
+
 
 class DataCollectionController(threading.Thread):
     """Event loop for the GUI.
 
     This class interfaces between the GUI and the underlying
     experiments. It runs in a separate thread and uses a queue to
     communicate tasks from the GUI to the instrument interface. This is
@@ -90,15 +90,14 @@
 
     def __init__(self):
         super().__init__()
         self.modules = {}
         self.locations = ['left', 'top', 'bottom', 'right']
 
     def load(self, modules, master):
-
         panels = {}
 
         for location in self.locations:
             selected_modules = [module for module in modules if module.location == location]
 
             is_group = len(selected_modules) > 1
```

### Comparing `instamatic-1.8.0/instamatic/gui/io_frame.py` & `instamatic-1.9.0/instamatic/gui/io_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import datetime
 import os
 import tkinter.filedialog
 from pathlib import Path
 from tkinter import *
 from tkinter.ttk import *
 
-from .base_module import BaseModule
 from instamatic import config
 from instamatic.utils.spinbox import Spinbox
 
+from .base_module import BaseModule
+
 
 class IOFrame(LabelFrame):
     """Simple interface to set the working directory and experiment
     name/numbering, and access the configs/work directory."""
 
     def __init__(self, parent):
         LabelFrame.__init__(self, parent, text='Input/Output')
```

### Comparing `instamatic-1.8.0/instamatic/gui/jobs.py` & `instamatic-1.9.0/instamatic/gui/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 function they were originally written for.
 
 Should be generally applicable.
 """
 import time
 from datetime import datetime
 
-from instamatic.formats import read_tiff
-from instamatic.formats import write_tiff
+from instamatic.formats import read_tiff, write_tiff
 
 
 def microscope_control(controller, **kwargs):
     from operator import attrgetter
 
     task = kwargs.pop('task')
```

### Comparing `instamatic-1.8.0/instamatic/gui/machine_learning_frame.py` & `instamatic-1.9.0/instamatic/gui/machine_learning_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from pathlib import Path
 from tkinter import *
 from tkinter.ttk import *
 
 import matplotlib.pyplot as plt
 import numpy as np
 
+from instamatic.formats import read_image
+
 from .base_module import BaseModule
 from .mpl_frame import ShowMatplotlibFig
-from instamatic.formats import read_image
 
 
 def treeview_sort_column(tv, col, reverse):
     """https://stackoverflow.com/a/22032582."""
     lst = [(tv.set(k, col), k) for k in tv.get_children('')]
     lst.sort(key=lambda t: float(t[0]), reverse=reverse)
 
@@ -83,15 +84,15 @@
         fn = tkinter.filedialog.askopenfilename(parent=self.parent, initialdir=self.var_directory.get(), title='Select crystal data')
         if not fn:
             return
         fn = Path(fn).resolve()
 
         import csv
 
-        with open(fn, 'r') as f:
+        with open(fn) as f:
             reader = csv.reader(f)
             for row in reader:
                 if not row:
                     continue
                 fn_patt, frame, number, prediction, size, stage_x, stage_y = row
                 self.tv.insert('', 'end', text=fn_patt, values=(frame, number, prediction, size, stage_x, stage_y))
                 self.fns[(int(frame), int(number))] = fn
```

### Comparing `instamatic-1.8.0/instamatic/gui/mpl_frame.py` & `instamatic-1.9.0/instamatic/gui/mpl_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/gui/red_frame.py` & `instamatic-1.9.0/instamatic/gui/red_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from tkinter import *
 from tkinter.ttk import *
 
-from .base_module import BaseModule
 from instamatic.utils.spinbox import Spinbox
 
+from .base_module import BaseModule
+
 
 class ExperimentalRED(LabelFrame):
     """GUI panel to perform a simple RED experiment using discrete rotation
     steps."""
 
     def __init__(self, parent):
         LabelFrame.__init__(self, parent, text='Rotation electron diffraction')
```

### Comparing `instamatic-1.8.0/instamatic/gui/sed_frame.py` & `instamatic-1.9.0/instamatic/gui/sed_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 import tkinter.messagebox
 from pathlib import Path
 from tkinter import *
 from tkinter.ttk import *
 
-from .base_module import BaseModule
 from instamatic.calibrate import CalibDirectBeam
-from instamatic.calibrate.filenames import CALIB_BEAMSHIFT
-from instamatic.calibrate.filenames import CALIB_DIRECTBEAM
+from instamatic.calibrate.filenames import CALIB_BEAMSHIFT, CALIB_DIRECTBEAM
+
+from .base_module import BaseModule
+
 # import matplotlib
 # matplotlib.use('TkAgg')
 
 
 PARAMS = {
     'flatfield': 'C:/instamatic/flatfield.tiff',
     'diff_binsize': 1,
@@ -169,15 +170,15 @@
 
     workdir = controller.module_io.get_working_directory()
     expdir = controller.module_io.get_new_experiment_directory()
     expdir.mkdir(exist_ok=True, parents=True)
 
     params = workdir / 'params.json'
     try:
-        params = json.load(open(params, 'r'))
+        params = json.load(open(params))
     except OSError:
         params = PARAMS
 
     params.update(kwargs)
     params['flatfield'] = controller.module_io.get_flatfield()
 
     scan_radius = kwargs['scan_radius']
```

### Comparing `instamatic-1.8.0/instamatic/gui/videostream_frame.py` & `instamatic-1.9.0/instamatic/gui/videostream_frame.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,300 +1,298 @@
-import threading
-import time
-from datetime import datetime
-from tkinter import *
-from tkinter.ttk import *
-
-import numpy as np
-from PIL import Image
-from PIL import ImageEnhance
-from PIL import ImageTk
-
-from .base_module import BaseModule
-from instamatic.formats import read_tiff
-from instamatic.formats import write_tiff
-from instamatic.processing.flatfield import apply_flatfield_correction
-from instamatic.utils.spinbox import Spinbox
-
-
-class VideoStreamFrame(LabelFrame):
-    """GUI panel to continuously display the last frame streamed from the
-    camera."""
-
-    def __init__(self, parent, stream, app=None):
-        LabelFrame.__init__(self, parent, text='Stream')
-
-        self.parent = parent
-
-        self.stream = stream
-        self.app = app
-
-        self.panel = None
-
-        self.frame_delay = 50
-
-        self.frametime = 0.05
-        self.brightness = 1.0
-        self.display_range = self.display_range_default = self.stream.cam.dynamic_range
-        # Maximum number from image readout
-
-        self.auto_contrast = True
-
-        self.resize_image = False
-
-        self.last = time.perf_counter()
-        self.nframes = 1
-        self.update_frequency = 0.25
-        self.last_interval = self.frametime
-
-        self._atexit_funcs = []
-
-        #######################
-
-        self.parent = parent
-
-        self.init_vars()
-        self.buttonbox(self)
-        self.header(self)
-        self.makepanel(self)
-
-        try:
-            self.parent.wm_title('Video stream')
-            self.parent.wm_protocol('WM_DELETE_WINDOW', self.close)
-        except AttributeError:
-            pass
-
-        self.parent.bind('<Escape>', self.close)
-
-        self.start_stream()
-
-    def init_vars(self):
-        self.var_fps = DoubleVar()
-        self.var_interval = DoubleVar()
-        # self.var_overhead = DoubleVar()
-
-        self.var_frametime = DoubleVar()
-        self.var_frametime.set(self.frametime)
-        self.var_frametime.trace_add('write', self.update_frametime)
-
-        self.var_brightness = DoubleVar(value=self.brightness)
-        self.var_brightness.trace_add('write', self.update_brightness)
-
-        self.var_display_range = DoubleVar(value=self.display_range_default)
-        self.var_display_range.trace_add('write', self.update_display_range)
-
-        self.var_resize_image = BooleanVar(value=self.resize_image)
-        self.var_resize_image.trace_add('write', self.update_resize_image)
-
-        self.var_auto_contrast = BooleanVar(value=self.auto_contrast)
-        self.var_auto_contrast.trace_add('write', self.update_auto_contrast)
-
-    def buttonbox(self, master):
-        btn = Button(master, text='Save image',
-                     command=self.saveImage)
-        btn.pack(side='bottom', fill='both', padx=10, pady=10)
-
-    def header(self, master):
-        ewidth = 8
-        lwidth = 12
-
-        frame = Frame(master)
-
-        self.cb_resize = Checkbutton(frame, text='Increase size', variable=self.var_resize_image)
-        self.cb_resize.grid(row=1, column=4)
-
-        self.cb_contrast = Checkbutton(frame, text='Auto contrast', variable=self.var_auto_contrast)
-        self.cb_contrast.grid(row=1, column=5)
-
-        self.e_fps = Entry(frame, width=lwidth, textvariable=self.var_fps, state=DISABLED)
-        self.e_interval = Entry(frame, width=lwidth, textvariable=self.var_interval, state=DISABLED)
-        # self.e_overhead    = Entry(frame, bd=0, width=ewidth, textvariable=self.var_overhead, state=DISABLED)
-
-        Label(frame, width=lwidth, text='fps:').grid(row=1, column=0)
-        self.e_fps.grid(row=1, column=1, sticky='we')
-        Label(frame, width=lwidth, text='interval (ms):').grid(row=1, column=2)
-        self.e_interval.grid(row=1, column=3, sticky='we')
-        # Label(frame, width=lwidth, text="overhead (ms):").grid(row=1, column=4)
-        # self.e_overhead.grid(row=1, column=5)
-
-        frame.pack()
-
-        frame = Frame(master)
-
-        self.e_frametime = Spinbox(frame, width=ewidth, textvariable=self.var_frametime, from_=0.0, to=1.0, increment=0.01)
-
-        Label(frame, width=lwidth, text='exposure (s)').grid(row=1, column=0)
-        self.e_frametime.grid(row=1, column=1)
-
-        self.e_brightness = Spinbox(frame, width=ewidth, textvariable=self.var_brightness, from_=0.0, to=10.0, increment=0.1)
-
-        Label(frame, width=lwidth, text='Brightness').grid(row=1, column=2)
-        self.e_brightness.grid(row=1, column=3)
-
-        Label(frame, width=lwidth, text='DisplayRange').grid(row=1, column=4)
-        self.e_display_range = Spinbox(frame, width=ewidth, textvariable=self.var_display_range, from_=1, to=self.display_range_default, increment=1000)
-        self.e_display_range.grid(row=1, column=5)
-
-        frame.pack()
-
-    def makepanel(self, master, resolution=(512, 512)):
-        if self.panel is None:
-            image = Image.fromarray(np.zeros(resolution))
-            image = ImageTk.PhotoImage(image)
-
-            self.panel = Label(master, image=image)
-            self.panel.image = image
-            self.panel.pack(side='left', padx=10, pady=10)
-
-    def setup_stream(self):
-        pass
-
-    def update_resize_image(self, name, index, mode):
-        # print name, index, mode
-        try:
-            self.resize_image = self.var_resize_image.get()
-        except BaseException:
-            pass
-
-    def update_auto_contrast(self, name, index, mode):
-        # print name, index, mode
-        try:
-            self.auto_contrast = self.var_auto_contrast.get()
-        except BaseException:
-            pass
-
-    def update_frametime(self, name, index, mode):
-        # print name, index, mode
-        try:
-            self.frametime = self.var_frametime.get()
-        except BaseException:
-            pass
-        else:
-            self.stream.update_frametime(self.frametime)
-
-    def update_brightness(self, name, index, mode):
-        # print name, index, mode
-        try:
-            self.brightness = self.var_brightness.get()
-        except BaseException:
-            pass
-
-    def update_display_range(self, name, index, mode):
-        try:
-            val = self.var_display_range.get()
-            self.display_range = max(1, val)
-        except BaseException:
-            pass
-
-    def saveImage(self):
-        """Dump the current frame to a file."""
-        self.q.put(('save_image', {'frame': self.frame}))
-        self.triggerEvent.set()
-
-    def set_trigger(self, trigger=None, q=None):
-        self.triggerEvent = trigger
-        self.q = q
-
-    def close(self):
-        self.stream.close()
-        self.parent.quit()
-        # for func in self._atexit_funcs:
-        # func()
-
-    def start_stream(self):
-        self.stream.update_frametime(self.frametime)
-        self.after(500, self.on_frame)
-
-    def on_frame(self, event=None):
-        self.stream.lock.acquire(True)
-        self.frame = frame = self.stream.frame
-        self.stream.lock.release()
-
-        if frame is not None:
-            # the display range in ImageTk is from 0 to 256
-            if self.auto_contrast:
-                frame = frame * (256.0 / (1 + np.percentile(frame[::4, ::4], 99.5)))  # use 128x128 array for faster calculation
-
-                image = Image.fromarray(frame)
-            elif self.display_range != self.display_range_default:
-                image = np.clip(frame, 0, self.display_range)
-                image = (256.0 / self.display_range) * image
-                image = Image.fromarray(image)
-            else:
-                image = Image.fromarray(frame)
-
-            if self.brightness != 1:
-                image = ImageEnhance.Brightness(image.convert('L')).enhance(self.brightness)
-                # Can also use ImageEnhance.Sharpness or ImageEnhance.Contrast if needed
-
-            if self.resize_image:
-                image = image.resize((950, 950))
-
-            image = ImageTk.PhotoImage(image=image)
-
-            self.panel.configure(image=image)
-            # keep a reference to avoid premature garbage collection
-            self.panel.image = image
-
-        self.update_frametimes()
-        # self.parent.update_idletasks()
-
-        self.after(self.frame_delay, self.on_frame)
-
-    def update_frametimes(self):
-        self.current = time.perf_counter()
-        delta = self.current - self.last
-
-        if delta > self.update_frequency:
-            interval = delta / self.nframes
-
-            interval = (interval * 0.5) + (self.last_interval * 0.5)
-
-            fps = 1.0 / interval
-            # overhead = interval - self.stream.frametime
-
-            self.var_fps.set(round(fps, 2))
-            self.var_interval.set(round(interval * 1000, 2))
-            # self.var_overhead.set(round(overhead*1000, 2))
-            self.last = self.current
-            self.nframes = 1
-
-            self.last_interval = interval
-        else:
-            self.nframes += 1
-
-
-module = BaseModule(name='stream', display_name='Stream', tk_frame=VideoStreamFrame, location='left')
-commands = {}
-
-
-def start_gui(stream):
-    """Pass a camera stream object, and open a simple live-view window This is
-    meant to be used in an interactive python shell."""
-    root = Tk()
-    vsframe = VideoStreamFrame(root, stream=stream)
-    vsframe.pack(side='top', fill='both', expand=True)
-    root.mainloop()
-    root.destroy()
-
-
-def ipy_embed(*args, **kwargs):
-    """Embed an ipython terminal."""
-    import IPython
-    IPython.embed(*args, **kwargs)
-
-
-if __name__ == '__main__':
-    from instamatic import config
-    from instamatic.camera import VideoStream
-
-    stream = VideoStream(cam=config.camera.name)
-
-    if False:
-        threading.Thread(target=ipy_embed).start()
-        start_gui()
-    else:
-        t = threading.Thread(target=start_gui, args=(stream,))
-        t.start()
-
-        import IPython
-        IPython.embed()
+import threading
+import time
+from datetime import datetime
+from tkinter import *
+from tkinter.ttk import *
+
+import numpy as np
+from PIL import Image, ImageEnhance, ImageTk
+
+from instamatic.formats import read_tiff, write_tiff
+from instamatic.processing.flatfield import apply_flatfield_correction
+from instamatic.utils.spinbox import Spinbox
+
+from .base_module import BaseModule
+
+
+class VideoStreamFrame(LabelFrame):
+    """GUI panel to continuously display the last frame streamed from the
+    camera."""
+
+    def __init__(self, parent, stream, app=None):
+        LabelFrame.__init__(self, parent, text='Stream')
+
+        self.parent = parent
+
+        self.stream = stream
+        self.app = app
+
+        self.panel = None
+
+        self.frame_delay = 50
+
+        self.frametime = 0.05
+        self.brightness = 1.0
+        self.display_range = self.display_range_default = self.stream.cam.dynamic_range
+        # Maximum number from image readout
+
+        self.auto_contrast = True
+
+        self.resize_image = False
+
+        self.last = time.perf_counter()
+        self.nframes = 1
+        self.update_frequency = 0.25
+        self.last_interval = self.frametime
+
+        self._atexit_funcs = []
+
+        #######################
+
+        self.parent = parent
+
+        self.init_vars()
+        self.buttonbox(self)
+        self.header(self)
+        self.makepanel(self)
+
+        try:
+            self.parent.wm_title('Video stream')
+            self.parent.wm_protocol('WM_DELETE_WINDOW', self.close)
+        except AttributeError:
+            pass
+
+        self.parent.bind('<Escape>', self.close)
+
+        self.start_stream()
+
+    def init_vars(self):
+        self.var_fps = DoubleVar()
+        self.var_interval = DoubleVar()
+        # self.var_overhead = DoubleVar()
+
+        self.var_frametime = DoubleVar()
+        self.var_frametime.set(self.frametime)
+        self.var_frametime.trace_add('write', self.update_frametime)
+
+        self.var_brightness = DoubleVar(value=self.brightness)
+        self.var_brightness.trace_add('write', self.update_brightness)
+
+        self.var_display_range = DoubleVar(value=self.display_range_default)
+        self.var_display_range.trace_add('write', self.update_display_range)
+
+        self.var_resize_image = BooleanVar(value=self.resize_image)
+        self.var_resize_image.trace_add('write', self.update_resize_image)
+
+        self.var_auto_contrast = BooleanVar(value=self.auto_contrast)
+        self.var_auto_contrast.trace_add('write', self.update_auto_contrast)
+
+    def buttonbox(self, master):
+        btn = Button(master, text='Save image',
+                     command=self.saveImage)
+        btn.pack(side='bottom', fill='both', padx=10, pady=10)
+
+    def header(self, master):
+        ewidth = 8
+        lwidth = 12
+
+        frame = Frame(master)
+
+        self.cb_resize = Checkbutton(frame, text='Increase size', variable=self.var_resize_image)
+        self.cb_resize.grid(row=1, column=4)
+
+        self.cb_contrast = Checkbutton(frame, text='Auto contrast', variable=self.var_auto_contrast)
+        self.cb_contrast.grid(row=1, column=5)
+
+        self.e_fps = Entry(frame, width=lwidth, textvariable=self.var_fps, state=DISABLED)
+        self.e_interval = Entry(frame, width=lwidth, textvariable=self.var_interval, state=DISABLED)
+        # self.e_overhead    = Entry(frame, bd=0, width=ewidth, textvariable=self.var_overhead, state=DISABLED)
+
+        Label(frame, width=lwidth, text='fps:').grid(row=1, column=0)
+        self.e_fps.grid(row=1, column=1, sticky='we')
+        Label(frame, width=lwidth, text='interval (ms):').grid(row=1, column=2)
+        self.e_interval.grid(row=1, column=3, sticky='we')
+        # Label(frame, width=lwidth, text="overhead (ms):").grid(row=1, column=4)
+        # self.e_overhead.grid(row=1, column=5)
+
+        frame.pack()
+
+        frame = Frame(master)
+
+        self.e_frametime = Spinbox(frame, width=ewidth, textvariable=self.var_frametime, from_=0.0, to=1.0, increment=0.01)
+
+        Label(frame, width=lwidth, text='exposure (s)').grid(row=1, column=0)
+        self.e_frametime.grid(row=1, column=1)
+
+        self.e_brightness = Spinbox(frame, width=ewidth, textvariable=self.var_brightness, from_=0.0, to=10.0, increment=0.1)
+
+        Label(frame, width=lwidth, text='Brightness').grid(row=1, column=2)
+        self.e_brightness.grid(row=1, column=3)
+
+        Label(frame, width=lwidth, text='DisplayRange').grid(row=1, column=4)
+        self.e_display_range = Spinbox(frame, width=ewidth, textvariable=self.var_display_range, from_=1, to=self.display_range_default, increment=1000)
+        self.e_display_range.grid(row=1, column=5)
+
+        frame.pack()
+
+    def makepanel(self, master, resolution=(512, 512)):
+        if self.panel is None:
+            image = Image.fromarray(np.zeros(resolution))
+            image = ImageTk.PhotoImage(image)
+
+            self.panel = Label(master, image=image)
+            self.panel.image = image
+            self.panel.pack(side='left', padx=10, pady=10)
+
+    def setup_stream(self):
+        pass
+
+    def update_resize_image(self, name, index, mode):
+        # print name, index, mode
+        try:
+            self.resize_image = self.var_resize_image.get()
+        except BaseException:
+            pass
+
+    def update_auto_contrast(self, name, index, mode):
+        # print name, index, mode
+        try:
+            self.auto_contrast = self.var_auto_contrast.get()
+        except BaseException:
+            pass
+
+    def update_frametime(self, name, index, mode):
+        # print name, index, mode
+        try:
+            self.frametime = self.var_frametime.get()
+        except BaseException:
+            pass
+        else:
+            self.stream.update_frametime(self.frametime)
+
+    def update_brightness(self, name, index, mode):
+        # print name, index, mode
+        try:
+            self.brightness = self.var_brightness.get()
+        except BaseException:
+            pass
+
+    def update_display_range(self, name, index, mode):
+        try:
+            val = self.var_display_range.get()
+            self.display_range = max(1, val)
+        except BaseException:
+            pass
+
+    def saveImage(self):
+        """Dump the current frame to a file."""
+        self.q.put(('save_image', {'frame': self.frame}))
+        self.triggerEvent.set()
+
+    def set_trigger(self, trigger=None, q=None):
+        self.triggerEvent = trigger
+        self.q = q
+
+    def close(self):
+        self.stream.close()
+        self.parent.quit()
+        # for func in self._atexit_funcs:
+        # func()
+
+    def start_stream(self):
+        self.stream.update_frametime(self.frametime)
+        self.after(500, self.on_frame)
+
+    def on_frame(self, event=None):
+        self.stream.lock.acquire(True)
+        self.frame = frame = self.stream.frame
+        self.stream.lock.release()
+
+        if frame is not None:
+            # the display range in ImageTk is from 0 to 256
+            if self.auto_contrast:
+                frame = frame * (256.0 / (1 + np.percentile(frame[::4, ::4], 99.5)))  # use 128x128 array for faster calculation
+
+                image = Image.fromarray(frame)
+            elif self.display_range != self.display_range_default:
+                image = np.clip(frame, 0, self.display_range)
+                image = (256.0 / self.display_range) * image
+                image = Image.fromarray(image)
+            else:
+                image = Image.fromarray(frame)
+
+            if self.brightness != 1:
+                image = ImageEnhance.Brightness(image.convert('L')).enhance(self.brightness)
+                # Can also use ImageEnhance.Sharpness or ImageEnhance.Contrast if needed
+
+            if self.resize_image:
+                image = image.resize((950, 950))
+
+            image = ImageTk.PhotoImage(image=image)
+
+            self.panel.configure(image=image)
+            # keep a reference to avoid premature garbage collection
+            self.panel.image = image
+
+        self.update_frametimes()
+        # self.parent.update_idletasks()
+
+        self.after(self.frame_delay, self.on_frame)
+
+    def update_frametimes(self):
+        self.current = time.perf_counter()
+        delta = self.current - self.last
+
+        if delta > self.update_frequency:
+            interval = delta / self.nframes
+
+            interval = (interval * 0.5) + (self.last_interval * 0.5)
+
+            fps = 1.0 / interval
+            # overhead = interval - self.stream.frametime
+
+            self.var_fps.set(round(fps, 2))
+            self.var_interval.set(round(interval * 1000, 2))
+            # self.var_overhead.set(round(overhead*1000, 2))
+            self.last = self.current
+            self.nframes = 1
+
+            self.last_interval = interval
+        else:
+            self.nframes += 1
+
+
+module = BaseModule(name='stream', display_name='Stream', tk_frame=VideoStreamFrame, location='left')
+commands = {}
+
+
+def start_gui(stream):
+    """Pass a camera stream object, and open a simple live-view window This is
+    meant to be used in an interactive python shell."""
+    root = Tk()
+    vsframe = VideoStreamFrame(root, stream=stream)
+    vsframe.pack(side='top', fill='both', expand=True)
+    root.mainloop()
+    root.destroy()
+
+
+def ipy_embed(*args, **kwargs):
+    """Embed an ipython terminal."""
+    import IPython
+    IPython.embed(*args, **kwargs)
+
+
+if __name__ == '__main__':
+    from instamatic import config
+    from instamatic.camera import VideoStream
+
+    stream = VideoStream(cam=config.camera.name)
+
+    if False:
+        threading.Thread(target=ipy_embed).start()
+        start_gui()
+    else:
+        t = threading.Thread(target=start_gui, args=(stream,))
+        t.start()
+
+        import IPython
+        IPython.embed()
```

### Comparing `instamatic-1.8.0/instamatic/image_utils.py` & `instamatic-1.9.0/instamatic/image_utils.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/imreg.py` & `instamatic-1.9.0/instamatic/imreg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
-from numpy.fft import fft2
-from numpy.fft import ifft2
+from numpy.fft import fft2, ifft2
 
 
 def translation(im0,
                 im1,
                 limit_shift: bool = False,
                 return_fft: bool = False,
                 ):
```

### Comparing `instamatic-1.8.0/instamatic/io.py` & `instamatic-1.9.0/instamatic/io.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/main.py` & `instamatic-1.9.0/instamatic/main.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/montage.py` & `instamatic-1.9.0/instamatic/montage.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,21 @@
         self.mode = mode
         self.magnification = magnification
 
     @classmethod
     def from_montage_yaml(cls, filename: str = 'montage.yaml'):
         """Load montage from a series of tiff files + `montage.yaml`"""
         import yaml
+
         from instamatic.formats import read_tiff
 
         p = Path(filename)
         drc = p.parent
 
-        d = yaml.safe_load(open(p, 'r'))
+        d = yaml.safe_load(open(p))
         fns = (drc / fn for fn in d['filenames'])
 
         d['stagecoords'] = np.array(d['stagecoords'])
         d['stagematrix'] = np.array(d['stagematrix'])
 
         images = [read_tiff(fn)[0] for fn in fns]
```

### Comparing `instamatic-1.8.0/instamatic/neural_network/neural_network.py` & `instamatic-1.9.0/instamatic/neural_network/neural_network.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/neural_network/preprocess.py` & `instamatic-1.9.0/instamatic/neural_network/preprocess.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/neural_network/preprocess_SerialRED.py` & `instamatic-1.9.0/instamatic/neural_network/preprocess_SerialRED.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/processing/ImgConversion.py` & `instamatic-1.9.0/instamatic/processing/ImgConversion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,702 +1,703 @@
-import collections
-import logging
-import time
-from datetime import datetime
-from math import cos
-
-import numpy as np
-
-from instamatic import config
-from instamatic.formats import read_tiff
-from instamatic.formats import write_adsc
-from instamatic.formats import write_mrc
-from instamatic.formats import write_tiff
-from instamatic.processing.flatfield import apply_flatfield_correction
-from instamatic.processing.stretch_correction import affine_transform_ellipse_to_circle
-from instamatic.tools import find_beam_center
-from instamatic.tools import find_beam_center_with_beamstop
-from instamatic.tools import find_subranges
-from instamatic.tools import to_xds_untrusted_area
-
-logger = logging.getLogger(__name__)
-
-
-def rotation_axis_to_xyz(rotation_axis, invert=False, setting='xds'):
-    """Convert rotation axis angle to XYZ vector compatible with 'xds', or
-    'dials' Set invert to 'True' for anti-clockwise rotation."""
-    if invert:
-        rotation_axis += np.pi
-
-    rot_x = np.cos(rotation_axis)
-    rot_y = np.sin(rotation_axis)
-    rot_z = 0
-
-    if setting == 'dials':
-        return rot_x, rot_y, rot_z
-    elif setting == 'xds':
-        return rot_x, -rot_y, rot_z
-    else:
-        raise ValueError("Must be one of {'dials', 'xds'}")
-
-
-def export_dials_variables(path, *, sequence=(), missing=(), rotation_xyz=None):
-    """Export variables for DIALS to account for missing frames writes
-    dials_variables.sh (bash) and dials_variables.bat (cmd)
-
-    `sequence` is a tuple of sequence numbers of the data frames
-    `missing `is a tuple of sequence numbers of the missing frames
-    """
-    scanranges = find_subranges(sequence)
-
-    scanrange = ' '.join(f'scan_range={i},{j}' for i, j in scanranges)
-    excludeimages = ','.join(str(n) for n in missing)
-
-    if rotation_xyz:
-        rot_x, rot_y, rot_z = rotation_xyz
-
-    # newline='\n' to have unix line endings
-    with open(path / 'dials_variables.sh', 'w', newline='\n') as f:
-        print('#!/usr/bin/env bash', file=f)
-        print(f"scan_range='{scanrange}'", file=f)
-        print(f"exclude_images='exclude_images={excludeimages}'", file=f)
-        if rotation_xyz:
-            print(f"rotation_axis='geometry.goniometer.axes={rot_x:.4f},{rot_y:.4f},{rot_z:.4f}'", file=f)
-        print('#', file=f)
-        print('# To run:', file=f)
-        print('#     source dials_variables.sh', file=f)
-        print('#', file=f)
-        print('# and:', file=f)
-        print('#     dials.import directory=data $rotation_axis', file=f)
-        print('#     dials.find_spots datablock.json $scan_range', file=f)
-        print('#     dials.integrate $exclude_images refined.pickle refined.json', file=f)
-        print('#', file=f)
-
-    with open(path / 'dials_variables.bat', 'w', newline='\n') as f:
-        print('@echo off', file=f)
-        print('', file=f)
-        print(f'set scan_range={scanrange}', file=f)
-        print(f'set exclude_images=exclude_images={excludeimages}', file=f)
-        if rotation_xyz:
-            print(f'set rotation_axis=geometry.goniometer.axes={rot_x:.4f},{rot_y:.4f},{rot_z:.4f}', file=f)
-        print('', file=f)
-        print(':: To run:', file=f)
-        print('::     call dials_variables.bat', file=f)
-        print('::', file=f)
-        print('::     dials.import directory=data %rotation_axis%', file=f)
-        print('::     dials.find_spots datablock.json %scan_range%', file=f)
-        print('::     dials.integrate %exclude_images% refined.pickle refined.json', file=f)
-
-
-def get_calibrated_rotation_speed(val):
-    """Correct for the overestimation of the oscillation angle if the rotation
-    was stopped before interrupting the data collection.
-
-    It uses calibrated values for the rotation speeds of the microscope,
-    and matches them to the observed one
-    """
-
-    rotation_speeds = set(config.microscope.rotation_speeds['coarse'] + config.microscope.rotation_speeds['fine'])
-    calibrated_value = min(rotation_speeds, key=lambda x: abs(x - val))
-    logger.info(f'Correcting oscillation angle from {val:.3f} to calibrated value {calibrated_value:.3f}')
-    return calibrated_value
-
-
-class ImgConversion:
-    """This class is for post RED/cRED data collection image conversion. Files
-    can be generated for REDp, DIALS, XDS, and PETS.
-
-    The image buffer is passed as a list of tuples, where each tuple
-    contains the index (int), image data (2D numpy array),
-    metadata/header (dict). The buffer index must start at 1.
-    """
-
-    def __init__(self,
-                 buffer: list,                   # image buffer, list of (index [int], image data [2D numpy array], header [dict])
-                 camera_length: float,           # virtual camera length read from the microscope
-                 osc_angle: float,               # degrees, oscillation angle of the rotation
-                 start_angle: float,             # degrees, start angle of the rotation
-                 end_angle: float,               # degrees, end angle of the rotation
-                 rotation_axis: float,           # radians, specifies the position of the rotation axis
-                 acquisition_time: float,        # seconds, acquisition time (exposure time + overhead)
-                 flatfield: str = 'flatfield.tiff',
-                 ):
-        if flatfield is not None:
-            flatfield, h = read_tiff(flatfield)
-        self.flatfield = flatfield
-
-        self.headers = {}
-        self.data = {}
-
-        self.smv_subdrc = 'data'
-
-        while len(buffer) != 0:
-            i, img, h = buffer.pop(0)
-
-            self.headers[i] = h
-
-            if self.flatfield is not None:
-                self.data[i] = apply_flatfield_correction(img, self.flatfield)
-            else:
-                self.data[i] = img
-
-        self.untrusted_areas = []
-
-        self.observed_range = set(self.data.keys())
-        self.complete_range = set(range(min(self.observed_range), max(self.observed_range) + 1))
-        self.missing_range = self.observed_range ^ self.complete_range
-
-        self.data_shape = img.shape
-        try:
-            self.pixelsize = config.calibration['diff']['pixelsize'][camera_length]  # px / Angstrom
-        except KeyError:
-            self.pixelsize = 1
-            print(f'No calibrated pixelsize for camera length={camera_length}. Setting pixelsize to 1.')
-            logger.warning(f'No calibrated pixelsize for camera length={camera_length}. Setting pixelsize to 1.')
-
-        self.physical_pixelsize = config.camera.physical_pixelsize  # mm
-        self.wavelength = config.microscope.wavelength  # angstrom
-        # NOTE: Stretch correction - not sure if the azimuth and amplitude are correct anymore.
-        self.do_stretch_correction = True
-        self.stretch_azimuth = config.camera.stretch_azimuth
-        self.stretch_amplitude = config.camera.stretch_amplitude
-
-        self.distance = (1 / self.wavelength) * (self.physical_pixelsize / self.pixelsize)
-        self.osc_angle = osc_angle
-        self.start_angle = start_angle
-        self.end_angle = end_angle
-        self.rotation_axis = rotation_axis
-
-        self.acquisition_time = acquisition_time
-        # self.rotation_speed = get_calibrated_rotation_speed(osc_angle / self.acquisition_time)
-
-        self.name = 'Instamatic'
-
-        from .XDS_template import XDS_template  # hook XDS_template here, because it is difficult to override as a global
-        self.XDS_template = XDS_template
-
-        self.check_settings()  # check if all required parameters are present, and fill default values if needed
-
-        self.mean_beam_center, self.beam_center_std = self.get_beam_centers()
-        logger.debug(f'Primary beam at: {self.mean_beam_center}')
-
-    def check_settings(self) -> None:
-        """Check for the presence of all required attributes.
-
-        If possible, optional missing attributes are set to their
-        defaults.
-        """
-
-        kw_attrs = {
-            'name': 'instamatic',
-            'use_beamstop': False,
-            'untrusted_areas': [],
-            'smv_subdrc': 'data',
-            'do_stretch_correction': False,
-        }
-
-        for attr, default in kw_attrs.items():
-            if not hasattr(self, attr):
-                print(f'self.{attr} = {default}')
-                setattr(self, attr, default)
-
-        attrs = [
-            # "rotation_speed",
-            'acquisition_time',
-            'start_angle',
-            'end_angle',
-            'osc_angle',
-            'distance',
-            'mean_beam_center',
-            'wavelength',
-            'physical_pixelsize',
-            'pixelsize',
-            'data_shape',
-            'missing_range',
-            'complete_range',
-            'observed_range',
-            'headers',
-            'data',
-            'XDS_template',
-        ]
-
-        for attr in attrs:
-            if not hasattr(self, attr):
-                raise AttributeError(f'`{self.__class__.__name__}` has no attribute `{attr}`')
-
-        if self.do_stretch_correction:
-            stretch_attrs = ('stretch_amplitude', 'stretch_azimuth')
-            if not all(hasattr(self, attr) for attr in stretch_attrs):
-                raise AttributeError(f'`{self.__class__.__name__}` is missing stretch attrs `{stretch_attrs[0]}/{stretch_attrs[1]}`')
-
-    def get_beam_centers(self, invert_x: bool = False, invert_y: bool = False) -> (float, float):
-        """Obtain beam centers from the diffraction data Returns a tuple with
-        the median beam center and its standard deviation."""
-        shape_x, shape_y = self.data_shape
-        centers = []
-        for i, h in self.headers.items():
-            if self.use_beamstop:
-                cx, cy = find_beam_center_with_beamstop(self.data[i], z=99)
-            else:
-                cx, cy = find_beam_center(self.data[i], sigma=10)
-
-            if invert_x:
-                cx = shape_x - cx
-            if invert_y:
-                cy = shape_y - cy
-
-            h['beam_center'] = (cx, cy)
-            centers.append((cx, cy))
-
-        self._beam_centers = beam_centers = np.array(centers)
-
-        # avg_center = np.mean(centers, axis=0)
-        median_center = np.median(beam_centers, axis=0)
-        std_center = np.std(beam_centers, axis=0)
-
-        return median_center, std_center
-
-    def write_geometric_correction_files(self, path) -> None:
-        """Make geometric correction images for XDS Writes files XCORR.cbf and
-        YCORR.cbf to `path`
-
-        To use:
-            DETECTOR= PILATUS     ! fake being a PILATUS detector
-            X-GEO_CORR= XCORR.cbf
-            Y-GEO_CORR= YCORR.cbf
-
-        Reads the stretch amplitude/azimuth from the config file
-        """
-        from instamatic.formats import write_cbf
-
-        center = np.array(self.mean_beam_center)
-
-        amplitude_pc = self.stretch_amplitude / (2 * 100)
-
-        # To create the correct corrections the azimuth is mirrored
-        azimuth_rad = np.radians(180 - self.stretch_azimuth)
-
-        shape = self.data_shape
-
-        xi, yi = np.mgrid[0:shape[0], 0:shape[1]]
-        coords = np.stack([xi.flatten(), yi.flatten()], axis=1) - center
-
-        s = affine_transform_ellipse_to_circle(azimuth_rad, amplitude_pc)
-
-        new = np.dot(coords, s)
-
-        xcorr = (new[:, 0].reshape(shape) + center[0]) - xi
-        ycorr = (new[:, 1].reshape(shape) + center[1]) - yi
-
-        # reverse XY coordinates for XDS
-        xcorr, ycorr = ycorr, xcorr
-
-        # In XDS, the geometrically corrected coordinates of a pixel at IX,IY
-        # are found by adding the table_value(IX,IY)/100.0 for the X- and Y-tables, respectively.
-        write_cbf(path / 'XCORR.cbf', np.int32(xcorr * 100))
-        write_cbf(path / 'YCORR.cbf', np.int32(ycorr * 100))
-
-    def tiff_writer(self, path: str) -> None:
-        """Write all data as tiff files to given `path`"""
-        print('\033[k', 'Writing TIFF files......', end='\r')
-
-        path.mkdir(exist_ok=True)
-
-        for i in self.observed_range:
-            self.write_tiff(path, i)
-
-        logger.debug(f'Tiff files saved in folder: {path}')
-
-    def smv_writer(self, path: str) -> None:
-        """Write all data as SMV files compatible with XDS/DIALS to `path`"""
-        print('\033[k', 'Writing SMV files......', end='\r')
-
-        path = path / self.smv_subdrc
-        path.mkdir(exist_ok=True)
-
-        for i in self.observed_range:
-            self.write_smv(path, i)
-
-        logger.debug(f'SMV files saved in folder: {path}')
-
-    def mrc_writer(self, path: str) -> None:
-        """Write all data as mrc files to `path`"""
-        print('\033[k', 'Writing MRC files......', end='\r')
-
-        path.mkdir(exist_ok=True)
-
-        for i in self.observed_range:
-            self.write_mrc(path, i)
-
-        logger.debug(f'MRC files created in folder: {path}')
-
-    def threadpoolwriter(self, tiff_path: str = None, smv_path: str = None, mrc_path: str = None, workers: int = 8) -> None:
-        """Efficiently write all data to the specified formats using a
-        threadpool.
-
-        If a path is given, write data in the corresponding format, i.e.
-        if `tiff_path` is specified TIFF files are written to that path.
-        """
-        write_tiff = tiff_path is not None
-        write_smv = smv_path is not None
-        write_mrc = mrc_path is not None
-
-        if write_smv:
-            smv_path = smv_path / self.smv_subdrc
-            smv_path.mkdir(exist_ok=True, parents=True)
-            logger.debug(f'SMV files saved in folder: {smv_path}')
-
-        if write_tiff:
-            tiff_path.mkdir(exist_ok=True, parents=True)
-            logger.debug(f'Tiff files saved in folder: {tiff_path}')
-
-        if write_mrc:
-            mrc_path.mkdir(exist_ok=True, parents=True)
-            logger.debug(f'MRC files saved in folder: {mrc_path}')
-
-        import concurrent.futures
-        with concurrent.futures.ThreadPoolExecutor(max_workers=workers) as executor:
-            futures = []
-            for i in self.observed_range:
-
-                if write_tiff:
-                    futures.append(executor.submit(self.write_tiff, tiff_path, i))
-                if write_mrc:
-                    futures.append(executor.submit(self.write_mrc, mrc_path, i))
-                if write_smv:
-                    futures.append(executor.submit(self.write_smv, smv_path, i))
-
-            for future in futures:
-                ret = future.result()
-
-    def to_dials(self, smv_path: str) -> None:
-        """Convert the buffer to output compatible with DIALS.
-
-        Files are written to the path given by `smv_path`.
-        """
-        observed_range = self.observed_range
-        self.missing_range = self.missing_range
-
-        invert_rotation_axis = self.start_angle > self.end_angle
-        rotation_xyz = rotation_axis_to_xyz(self.rotation_axis, invert=invert_rotation_axis, setting='dials')
-
-        export_dials_variables(smv_path, sequence=observed_range, missing=self.missing_range, rotation_xyz=rotation_xyz)
-
-        path = smv_path / self.smv_subdrc
-
-        i = min(observed_range)
-        empty = np.zeros_like(self.data[i])
-        # copy header from first frame
-        h = self.headers[i].copy()
-        h['ImageGetTime'] = time.time()
-
-        # add data to self.data/self.headers so that existing functions can be used
-        # make sure to remove them afterwards, not to interfere with other data writing
-        logger.debug(f'Writing missing files for DIALS: {self.missing_range}')
-
-        for n in self.missing_range:
-            self.data[n] = empty
-            self.headers[n] = h
-
-            self.write_smv(path, n)
-
-            del self.data[n]
-            del self.headers[n]
-
-    def write_tiff(self, path: str, i: int) -> str:
-        """Write the image+header with sequence number `i` to the directory
-        `path` in TIFF format.
-
-        Returns the path to the written image.
-        """
-        img = self.data[i]
-        h = self.headers[i]
-
-        # PETS reads only 16bit unsignt integer TIFF
-        img = np.round(img, 0).astype(np.uint16)
-
-        fn = path / f'{i:05d}.tiff'
-        write_tiff(fn, img, header=h)
-        return fn
-
-    def write_smv(self, path: str, i: int) -> str:
-        """Write the image+header with sequence number `i` to the directory
-        `path` in SMV format.
-
-        Returns the path to the written image.
-        """
-        img = self.data[i]
-        h = self.headers[i]
-
-        img = np.ushort(img)
-        shape_x, shape_y = img.shape
-
-        phi = self.start_angle + self.osc_angle * (i - 1)
-
-        # TODO: Dials reads the beam_center from the first image and uses that for the whole range
-        # For now, use the average beam center and consider it stationary, remove this line later
-        mean_beam_center = self.mean_beam_center
-
-        try:
-            date = str(datetime.fromtimestamp(h['ImageGetTime']))
-        except BaseException:
-            date = '0'
-
-        header = collections.OrderedDict()
-        header['HEADER_BYTES'] = 512
-        header['DIM'] = 2
-        header['BYTE_ORDER'] = 'little_endian'
-        header['TYPE'] = 'unsigned_short'
-        header['SIZE1'] = shape_x
-        header['SIZE2'] = shape_y
-        header['PIXEL_SIZE'] = self.physical_pixelsize
-        header['BIN'] = '1x1'
-        header['BIN_TYPE'] = 'HW'
-        header['ADC'] = 'fast'
-        header['CREV'] = 1
-        header['BEAMLINE'] = self.name      # special ID for DIALS
-        header['DETECTOR_SN'] = 901         # special ID for DIALS
-        header['DATE'] = date
-        header['TIME'] = str(h['ImageExposureTime'])
-        header['DISTANCE'] = f'{self.distance:.4f}'
-        header['TWOTHETA'] = 0.00
-        header['PHI'] = '{phi:.4f}'
-        header['OSC_START'] = f'{phi:.4f}'
-        header['OSC_RANGE'] = f'{self.osc_angle:.4f}'
-        header['WAVELENGTH'] = f'{self.wavelength:.4f}'
-        # reverse XY coordinates for XDS
-        header['BEAM_CENTER_X'] = f'{mean_beam_center[1]:.4f}'
-        header['BEAM_CENTER_Y'] = f'{mean_beam_center[0]:.4f}'
-        header['DENZO_X_BEAM'] = f'{mean_beam_center[0]*self.physical_pixelsize:.4f}'
-        header['DENZO_Y_BEAM'] = f'{mean_beam_center[1]*self.physical_pixelsize:.4f}'
-        fn = path / f'{i:05d}.img'
-        write_adsc(fn, img, header=header)
-        return fn
-
-    def write_mrc(self, path: str, i: int) -> str:
-        """Write the image+header with sequence number `i` to the directory
-        `path` in TIFF format.
-
-        Returns the path to the written image.
-        """
-        img = self.data[i]
-
-        fn = path / f'{i:05d}.mrc'
-
-        # for RED these need to be as integers
-        dtype = np.uint16
-        if False:
-            # Use maximum range available in data type for extra precision when converting from FLOAT to INT
-            dynamic_range = 11900  # a little bit higher just in case
-            maxval = np.iinfo(dtype).max
-            img = (img / dynamic_range) * maxval
-
-        img = np.round(img, 0).astype(dtype)
-
-        # flip up/down because RED reads images from the bottom left corner
-        img = np.flipud(img)
-
-        write_mrc(fn, img)
-
-        return fn
-
-    def write_ed3d(self, path: str) -> None:
-        """Write .ed3d input file for REDp in directory `path`"""
-        path.mkdir(exist_ok=True)
-
-        omega = np.degrees(self.rotation_axis)
-
-        # for red, -180 <= omega <= 180
-        if omega < -180:
-            omega += 360
-        elif omega > 180:
-            omega -= 360
-
-        if self.start_angle > self.end_angle:
-            sign = -1
-        else:
-            sign = 1
-
-        with open(path / '1.ed3d', 'w') as f:
-            print(f'WAVELENGTH    {self.wavelength}', file=f)
-            print(f'ROTATIONAXIS    {omega:5f}', file=f)
-            print(f'CCDPIXELSIZE    {self.pixelsize:5f}', file=f)
-            print(f'GONIOTILTSTEP    {self.osc_angle:5f}', file=f)
-            print('BEAMTILTSTEP    0', file=f)
-            print('BEAMTILTRANGE    0.000', file=f)
-            print('STRETCHINGMP    0.0', file=f)
-            print('STRETCHINGAZIMUTH    0.0', file=f)
-            print('', file=f)
-            print('FILELIST', file=f)
-
-            for i in self.observed_range:
-                fn = f'{i:05d}.mrc'
-                angle = self.start_angle + sign * self.osc_angle * i
-                print(f'FILE {fn}    {angle: 12.4f}    0    {angle: 12.4f}', file=f)
-
-            print('ENDFILELIST', file=f)
-
-        logger.debug(f'ED3D file created in path: {path}')
-
-    def write_xds_inp(self, path: str) -> None:
-        """Write XDS.INP input file for XDS in directory `path`"""
-
-        path.mkdir(exist_ok=True)
-
-        nframes = max(self.complete_range)
-
-        invert_rotation_axis = self.start_angle > self.end_angle
-        rot_x, rot_y, rot_z = rotation_axis_to_xyz(self.rotation_axis, invert=invert_rotation_axis)
-
-        shape_x, shape_y = self.data_shape
-
-        if self.do_stretch_correction:
-            self.write_geometric_correction_files(path)
-            stretch_correction = 'DETECTOR= PILATUS      ! Pretend to be PILATUS detector to enable geometric corrections\nX-GEO_CORR= XCORR.cbf  ! X stretch correction\nY-GEO_CORR= YCORR.cbf  ! Y stretch correction\n'
-        else:
-            stretch_correction = ''
-
-        if self.missing_range:
-            exclude = '\n'.join([f'EXCLUDE_DATA_RANGE={i} {j}' for i, j in find_subranges(self.missing_range)])
-        else:
-            exclude = '!EXCLUDE_DATA_RANGE='
-
-        untrusted_areas = ''
-
-        for kind, coords in self.untrusted_areas:
-            untrusted_areas += to_xds_untrusted_area(kind, coords) + '\n'
-
-        s = self.XDS_template.format(
-            date=str(time.ctime()),
-            data_drc=self.smv_subdrc,
-            data_begin=1,
-            data_end=nframes,
-            exclude=exclude,
-            stretch_correction=stretch_correction,
-            starting_angle=self.start_angle,
-            wavelength=self.wavelength,
-            # reverse XY coordinates for XDS
-            origin_x=self.mean_beam_center[1],
-            origin_y=self.mean_beam_center[0],
-            untrusted_areas=untrusted_areas,
-            NX=shape_y,
-            NY=shape_x,
-            sign='+',
-            detector_distance=self.distance,
-            QX=self.physical_pixelsize,
-            QY=self.physical_pixelsize,
-            osc_angle=self.osc_angle,
-            rot_x=rot_x,
-            rot_y=rot_y,
-            rot_z=rot_z,
-        )
-
-        with open(path / 'XDS.INP', 'w') as f:
-            print(s, file=f)
-
-        logger.info('XDS INP file created.')
-
-    def write_beam_centers(self, path: str) -> None:
-        """Write list of beam centers to file `beam_centers.txt` in `path`"""
-        centers = np.zeros((max(self.observed_range), 2), dtype=float)
-        for i, h in self.headers.items():
-            centers[i - 1] = h['beam_center']
-        for i in self.missing_range:
-            centers[i - 1] = [np.NaN, np.NaN]
-
-        np.savetxt(path / 'beam_centers.txt', centers, fmt='%10.4f')
-
-    def write_pets_inp(self, path: str, tiff_path: str = 'tiff') -> None:
-        """Write PETS input file `pets.pts` in directory `path`"""
-        if self.start_angle > self.end_angle:
-            sign = -1
-        else:
-            sign = 1
-
-        omega = np.degrees(self.rotation_axis)
-
-        # for pets, 0 <= omega <= 360
-        if omega < 0:
-            omega += 360
-        elif omega > 360:
-            omega -= 360
-
-        with open(path / 'pets.pts', 'w') as f:
-            date = str(time.ctime())
-            print('# PETS input file for Rotation Electron Diffraction generated by `instamatic`', file=f)
-            print(f'# {date}', file=f)
-            print('# For definitions of input parameters, see:', file=f)
-            print('# http://pets.fzu.cz/ ', file=f)
-            print('', file=f)
-            print(f'lambda {self.wavelength}', file=f)
-            print(f'Aperpixel {self.pixelsize}', file=f)
-            print('phi 0.0', file=f)
-            print(f'omega {omega}', file=f)
-            print('bin 1', file=f)
-            print('reflectionsize 20', file=f)
-            print('noiseparameters 3.5 38', file=f)
-            print('', file=f)
-            # print("reconstructions", file=f)
-            # print("endreconstructions", file=f)
-            # print("", file=f)
-            # print("distortions", file=f)
-            # print("enddistortions", file=f)
-            # print("", file=f)
-            print('imagelist', file=f)
-            for i in self.observed_range:
-                fn = f'{i:05d}.tiff'
-                angle = self.start_angle + sign * self.osc_angle * i
-                print(f'{tiff_path}/{fn} {angle:10.4f} 0.00', file=f)
-            print('endimagelist', file=f)
-    
-    def write_pets2_inp(self, path: str, tiff_path: str = 'tiff') -> None:
-        """Write PETS 2 input file `pets.pts2` in directory `path`"""
-        path.mkdir(exist_ok=True, parents=True)
-
-        if self.start_angle > self.end_angle:
-            sign = -1
-        else:
-            sign = 1
-
-        omega = np.degrees(self.rotation_axis)
-
-        with open(path / 'pets.pts2', 'w') as f:
-            date = str(time.ctime())
-            print('# PETS 2 input file for Rotation Electron Diffraction generated by `instamatic`', file=f)
-            print(f'# {date}', file=f)
-            print('# For definitions of input parameters, see:', file=f)
-            print('# http://pets.fzu.cz/ ', file=f)
-            print('', file=f)
-            print('geometry continuous', file=f)
-            print(f'lambda {self.wavelength}', file=f)
-            print(f'Aperpixel {self.pixelsize}', file=f)
-            print(f'phi {float(self.osc_angle)/2}', file=f)
-            print(f'omega {omega}', file=f)
-            print('bin 1', file=f)
-            print('reflectionsize 15', file=f)
-            print('noiseparameters 25 10', file=f)
-            print('i/sigma    5.00   10.00', file=f)
-            print('', file=f)
-            print('imagelist', file=f)
-            tiff_set = set([0])
-            last_img = len(self.observed_range)
-            tiff_set.update(self.observed_range)
-            tiff_set.remove(last_img)
-            for i in tiff_set:
-                fn = f'{i:04d}.tiff'
-                angle = self.start_angle + sign * self.osc_angle * i
-                print(f'{tiff_path}/{fn} {angle:10.4f} 0.00', file=f)
-            print('endimagelist', file=f)
-
-    def write_REDp_shiftcorrection(self, path: str) -> None:
-        """Write .sc (shift correction) file for REDp in directory `path`"""
-        path.mkdir(exist_ok=True)
-
-        cx, cy = self.mean_beam_center
-        with open(path / 'shifts.sc', 'w') as f:
-            print(f' {cy:.2f} {cx:.2f}', file=f)  # cx/cy must be switched around, y first
-            for i in self.observed_range:
-                print(f'{i:4d}{0:8.2f}{0:8.2f}', file=f)
-
-    def add_beamstop(self, rect):
-        """rect must be a 2x4 coordinate array."""
-        self.untrusted_areas.append(('quadrilateral', rect))
+import collections
+import logging
+import time
+from datetime import datetime
+from math import cos
+
+import numpy as np
+
+from instamatic import config
+from instamatic.formats import read_tiff, write_adsc, write_mrc, write_tiff
+from instamatic.processing.flatfield import apply_flatfield_correction
+from instamatic.processing.stretch_correction import affine_transform_ellipse_to_circle
+from instamatic.tools import (
+    find_beam_center,
+    find_beam_center_with_beamstop,
+    find_subranges,
+    to_xds_untrusted_area,
+)
+
+logger = logging.getLogger(__name__)
+
+
+def rotation_axis_to_xyz(rotation_axis, invert=False, setting='xds'):
+    """Convert rotation axis angle to XYZ vector compatible with 'xds', or
+    'dials' Set invert to 'True' for anti-clockwise rotation."""
+    if invert:
+        rotation_axis += np.pi
+
+    rot_x = np.cos(rotation_axis)
+    rot_y = np.sin(rotation_axis)
+    rot_z = 0
+
+    if setting == 'dials':
+        return rot_x, rot_y, rot_z
+    elif setting == 'xds':
+        return rot_x, -rot_y, rot_z
+    else:
+        raise ValueError("Must be one of {'dials', 'xds'}")
+
+
+def export_dials_variables(path, *, sequence=(), missing=(), rotation_xyz=None):
+    """Export variables for DIALS to account for missing frames writes
+    dials_variables.sh (bash) and dials_variables.bat (cmd)
+
+    `sequence` is a tuple of sequence numbers of the data frames
+    `missing `is a tuple of sequence numbers of the missing frames
+    """
+    scanranges = find_subranges(sequence)
+
+    scanrange = ' '.join(f'scan_range={i},{j}' for i, j in scanranges)
+    excludeimages = ','.join(str(n) for n in missing)
+
+    if rotation_xyz:
+        rot_x, rot_y, rot_z = rotation_xyz
+
+    # newline='\n' to have unix line endings
+    with open(path / 'dials_variables.sh', 'w', newline='\n') as f:
+        print('#!/usr/bin/env bash', file=f)
+        print(f"scan_range='{scanrange}'", file=f)
+        print(f"exclude_images='exclude_images={excludeimages}'", file=f)
+        if rotation_xyz:
+            print(f"rotation_axis='geometry.goniometer.axes={rot_x:.4f},{rot_y:.4f},{rot_z:.4f}'", file=f)
+        print('#', file=f)
+        print('# To run:', file=f)
+        print('#     source dials_variables.sh', file=f)
+        print('#', file=f)
+        print('# and:', file=f)
+        print('#     dials.import directory=data $rotation_axis', file=f)
+        print('#     dials.find_spots datablock.json $scan_range', file=f)
+        print('#     dials.integrate $exclude_images refined.pickle refined.json', file=f)
+        print('#', file=f)
+
+    with open(path / 'dials_variables.bat', 'w', newline='\n') as f:
+        print('@echo off', file=f)
+        print('', file=f)
+        print(f'set scan_range={scanrange}', file=f)
+        print(f'set exclude_images=exclude_images={excludeimages}', file=f)
+        if rotation_xyz:
+            print(f'set rotation_axis=geometry.goniometer.axes={rot_x:.4f},{rot_y:.4f},{rot_z:.4f}', file=f)
+        print('', file=f)
+        print(':: To run:', file=f)
+        print('::     call dials_variables.bat', file=f)
+        print('::', file=f)
+        print('::     dials.import directory=data %rotation_axis%', file=f)
+        print('::     dials.find_spots datablock.json %scan_range%', file=f)
+        print('::     dials.integrate %exclude_images% refined.pickle refined.json', file=f)
+
+
+def get_calibrated_rotation_speed(val):
+    """Correct for the overestimation of the oscillation angle if the rotation
+    was stopped before interrupting the data collection.
+
+    It uses calibrated values for the rotation speeds of the microscope,
+    and matches them to the observed one
+    """
+
+    rotation_speeds = set(config.microscope.rotation_speeds['coarse'] + config.microscope.rotation_speeds['fine'])
+    calibrated_value = min(rotation_speeds, key=lambda x: abs(x - val))
+    logger.info(f'Correcting oscillation angle from {val:.3f} to calibrated value {calibrated_value:.3f}')
+    return calibrated_value
+
+
+class ImgConversion:
+    """This class is for post RED/cRED data collection image conversion. Files
+    can be generated for REDp, DIALS, XDS, and PETS.
+
+    The image buffer is passed as a list of tuples, where each tuple
+    contains the index (int), image data (2D numpy array),
+    metadata/header (dict). The buffer index must start at 1.
+    """
+
+    def __init__(self,
+                 buffer: list,                   # image buffer, list of (index [int], image data [2D numpy array], header [dict])
+                 camera_length: float,           # virtual camera length read from the microscope
+                 osc_angle: float,               # degrees, oscillation angle of the rotation
+                 start_angle: float,             # degrees, start angle of the rotation
+                 end_angle: float,               # degrees, end angle of the rotation
+                 rotation_axis: float,           # radians, specifies the position of the rotation axis
+                 acquisition_time: float,        # seconds, acquisition time (exposure time + overhead)
+                 flatfield: str = 'flatfield.tiff',
+                 ):
+        if flatfield is not None:
+            flatfield, h = read_tiff(flatfield)
+        self.flatfield = flatfield
+
+        self.headers = {}
+        self.data = {}
+
+        self.smv_subdrc = 'data'
+
+        while len(buffer) != 0:
+            i, img, h = buffer.pop(0)
+
+            self.headers[i] = h
+
+            if self.flatfield is not None:
+                self.data[i] = apply_flatfield_correction(img, self.flatfield)
+            else:
+                self.data[i] = img
+
+        self.untrusted_areas = []
+
+        self.observed_range = set(self.data.keys())
+        self.complete_range = set(range(min(self.observed_range), max(self.observed_range) + 1))
+        self.missing_range = self.observed_range ^ self.complete_range
+
+        self.data_shape = img.shape
+        try:
+            self.pixelsize = config.calibration['diff']['pixelsize'][camera_length]  # px / Angstrom
+        except KeyError:
+            self.pixelsize = 1
+            print(f'No calibrated pixelsize for camera length={camera_length}. Setting pixelsize to 1.')
+            logger.warning(f'No calibrated pixelsize for camera length={camera_length}. Setting pixelsize to 1.')
+
+        self.physical_pixelsize = config.camera.physical_pixelsize  # mm
+        self.wavelength = config.microscope.wavelength  # angstrom
+        # NOTE: Stretch correction - not sure if the azimuth and amplitude are correct anymore.
+        self.do_stretch_correction = True
+        self.stretch_azimuth = config.camera.stretch_azimuth
+        self.stretch_amplitude = config.camera.stretch_amplitude
+
+        self.distance = (1 / self.wavelength) * (self.physical_pixelsize / self.pixelsize)
+        self.osc_angle = osc_angle
+        self.start_angle = start_angle
+        self.end_angle = end_angle
+        self.rotation_axis = rotation_axis
+
+        self.acquisition_time = acquisition_time
+        # self.rotation_speed = get_calibrated_rotation_speed(osc_angle / self.acquisition_time)
+
+        self.name = 'Instamatic'
+
+        from .XDS_template import (
+            XDS_template,  # hook XDS_template here, because it is difficult to override as a global
+        )
+        self.XDS_template = XDS_template
+
+        self.check_settings()  # check if all required parameters are present, and fill default values if needed
+
+        self.mean_beam_center, self.beam_center_std = self.get_beam_centers()
+        logger.debug(f'Primary beam at: {self.mean_beam_center}')
+
+    def check_settings(self) -> None:
+        """Check for the presence of all required attributes.
+
+        If possible, optional missing attributes are set to their
+        defaults.
+        """
+
+        kw_attrs = {
+            'name': 'instamatic',
+            'use_beamstop': False,
+            'untrusted_areas': [],
+            'smv_subdrc': 'data',
+            'do_stretch_correction': False,
+        }
+
+        for attr, default in kw_attrs.items():
+            if not hasattr(self, attr):
+                print(f'self.{attr} = {default}')
+                setattr(self, attr, default)
+
+        attrs = [
+            # "rotation_speed",
+            'acquisition_time',
+            'start_angle',
+            'end_angle',
+            'osc_angle',
+            'distance',
+            'mean_beam_center',
+            'wavelength',
+            'physical_pixelsize',
+            'pixelsize',
+            'data_shape',
+            'missing_range',
+            'complete_range',
+            'observed_range',
+            'headers',
+            'data',
+            'XDS_template',
+        ]
+
+        for attr in attrs:
+            if not hasattr(self, attr):
+                raise AttributeError(f'`{self.__class__.__name__}` has no attribute `{attr}`')
+
+        if self.do_stretch_correction:
+            stretch_attrs = ('stretch_amplitude', 'stretch_azimuth')
+            if not all(hasattr(self, attr) for attr in stretch_attrs):
+                raise AttributeError(f'`{self.__class__.__name__}` is missing stretch attrs `{stretch_attrs[0]}/{stretch_attrs[1]}`')
+
+    def get_beam_centers(self, invert_x: bool = False, invert_y: bool = False) -> (float, float):
+        """Obtain beam centers from the diffraction data Returns a tuple with
+        the median beam center and its standard deviation."""
+        shape_x, shape_y = self.data_shape
+        centers = []
+        for i, h in self.headers.items():
+            if self.use_beamstop:
+                cx, cy = find_beam_center_with_beamstop(self.data[i], z=99)
+            else:
+                cx, cy = find_beam_center(self.data[i], sigma=10)
+
+            if invert_x:
+                cx = shape_x - cx
+            if invert_y:
+                cy = shape_y - cy
+
+            h['beam_center'] = (cx, cy)
+            centers.append((cx, cy))
+
+        self._beam_centers = beam_centers = np.array(centers)
+
+        # avg_center = np.mean(centers, axis=0)
+        median_center = np.median(beam_centers, axis=0)
+        std_center = np.std(beam_centers, axis=0)
+
+        return median_center, std_center
+
+    def write_geometric_correction_files(self, path) -> None:
+        """Make geometric correction images for XDS Writes files XCORR.cbf and
+        YCORR.cbf to `path`
+
+        To use:
+            DETECTOR= PILATUS     ! fake being a PILATUS detector
+            X-GEO_CORR= XCORR.cbf
+            Y-GEO_CORR= YCORR.cbf
+
+        Reads the stretch amplitude/azimuth from the config file
+        """
+        from instamatic.formats import write_cbf
+
+        center = np.array(self.mean_beam_center)
+
+        amplitude_pc = self.stretch_amplitude / (2 * 100)
+
+        # To create the correct corrections the azimuth is mirrored
+        azimuth_rad = np.radians(180 - self.stretch_azimuth)
+
+        shape = self.data_shape
+
+        xi, yi = np.mgrid[0:shape[0], 0:shape[1]]
+        coords = np.stack([xi.flatten(), yi.flatten()], axis=1) - center
+
+        s = affine_transform_ellipse_to_circle(azimuth_rad, amplitude_pc)
+
+        new = np.dot(coords, s)
+
+        xcorr = (new[:, 0].reshape(shape) + center[0]) - xi
+        ycorr = (new[:, 1].reshape(shape) + center[1]) - yi
+
+        # reverse XY coordinates for XDS
+        xcorr, ycorr = ycorr, xcorr
+
+        # In XDS, the geometrically corrected coordinates of a pixel at IX,IY
+        # are found by adding the table_value(IX,IY)/100.0 for the X- and Y-tables, respectively.
+        write_cbf(path / 'XCORR.cbf', np.int32(xcorr * 100))
+        write_cbf(path / 'YCORR.cbf', np.int32(ycorr * 100))
+
+    def tiff_writer(self, path: str) -> None:
+        """Write all data as tiff files to given `path`"""
+        print('\033[k', 'Writing TIFF files......', end='\r')
+
+        path.mkdir(exist_ok=True)
+
+        for i in self.observed_range:
+            self.write_tiff(path, i)
+
+        logger.debug(f'Tiff files saved in folder: {path}')
+
+    def smv_writer(self, path: str) -> None:
+        """Write all data as SMV files compatible with XDS/DIALS to `path`"""
+        print('\033[k', 'Writing SMV files......', end='\r')
+
+        path = path / self.smv_subdrc
+        path.mkdir(exist_ok=True)
+
+        for i in self.observed_range:
+            self.write_smv(path, i)
+
+        logger.debug(f'SMV files saved in folder: {path}')
+
+    def mrc_writer(self, path: str) -> None:
+        """Write all data as mrc files to `path`"""
+        print('\033[k', 'Writing MRC files......', end='\r')
+
+        path.mkdir(exist_ok=True)
+
+        for i in self.observed_range:
+            self.write_mrc(path, i)
+
+        logger.debug(f'MRC files created in folder: {path}')
+
+    def threadpoolwriter(self, tiff_path: str = None, smv_path: str = None, mrc_path: str = None, workers: int = 8) -> None:
+        """Efficiently write all data to the specified formats using a
+        threadpool.
+
+        If a path is given, write data in the corresponding format, i.e.
+        if `tiff_path` is specified TIFF files are written to that path.
+        """
+        write_tiff = tiff_path is not None
+        write_smv = smv_path is not None
+        write_mrc = mrc_path is not None
+
+        if write_smv:
+            smv_path = smv_path / self.smv_subdrc
+            smv_path.mkdir(exist_ok=True, parents=True)
+            logger.debug(f'SMV files saved in folder: {smv_path}')
+
+        if write_tiff:
+            tiff_path.mkdir(exist_ok=True, parents=True)
+            logger.debug(f'Tiff files saved in folder: {tiff_path}')
+
+        if write_mrc:
+            mrc_path.mkdir(exist_ok=True, parents=True)
+            logger.debug(f'MRC files saved in folder: {mrc_path}')
+
+        import concurrent.futures
+        with concurrent.futures.ThreadPoolExecutor(max_workers=workers) as executor:
+            futures = []
+            for i in self.observed_range:
+
+                if write_tiff:
+                    futures.append(executor.submit(self.write_tiff, tiff_path, i))
+                if write_mrc:
+                    futures.append(executor.submit(self.write_mrc, mrc_path, i))
+                if write_smv:
+                    futures.append(executor.submit(self.write_smv, smv_path, i))
+
+            for future in futures:
+                ret = future.result()
+
+    def to_dials(self, smv_path: str) -> None:
+        """Convert the buffer to output compatible with DIALS.
+
+        Files are written to the path given by `smv_path`.
+        """
+        observed_range = self.observed_range
+        self.missing_range = self.missing_range
+
+        invert_rotation_axis = self.start_angle > self.end_angle
+        rotation_xyz = rotation_axis_to_xyz(self.rotation_axis, invert=invert_rotation_axis, setting='dials')
+
+        export_dials_variables(smv_path, sequence=observed_range, missing=self.missing_range, rotation_xyz=rotation_xyz)
+
+        path = smv_path / self.smv_subdrc
+
+        i = min(observed_range)
+        empty = np.zeros_like(self.data[i])
+        # copy header from first frame
+        h = self.headers[i].copy()
+        h['ImageGetTime'] = time.time()
+
+        # add data to self.data/self.headers so that existing functions can be used
+        # make sure to remove them afterwards, not to interfere with other data writing
+        logger.debug(f'Writing missing files for DIALS: {self.missing_range}')
+
+        for n in self.missing_range:
+            self.data[n] = empty
+            self.headers[n] = h
+
+            self.write_smv(path, n)
+
+            del self.data[n]
+            del self.headers[n]
+
+    def write_tiff(self, path: str, i: int) -> str:
+        """Write the image+header with sequence number `i` to the directory
+        `path` in TIFF format.
+
+        Returns the path to the written image.
+        """
+        img = self.data[i]
+        h = self.headers[i]
+
+        # PETS reads only 16bit unsignt integer TIFF
+        img = np.round(img, 0).astype(np.uint16)
+
+        fn = path / f'{i:05d}.tiff'
+        write_tiff(fn, img, header=h)
+        return fn
+
+    def write_smv(self, path: str, i: int) -> str:
+        """Write the image+header with sequence number `i` to the directory
+        `path` in SMV format.
+
+        Returns the path to the written image.
+        """
+        img = self.data[i]
+        h = self.headers[i]
+
+        img = np.ushort(img)
+        shape_x, shape_y = img.shape
+
+        phi = self.start_angle + self.osc_angle * (i - 1)
+
+        # TODO: Dials reads the beam_center from the first image and uses that for the whole range
+        # For now, use the average beam center and consider it stationary, remove this line later
+        mean_beam_center = self.mean_beam_center
+
+        try:
+            date = str(datetime.fromtimestamp(h['ImageGetTime']))
+        except BaseException:
+            date = '0'
+
+        header = collections.OrderedDict()
+        header['HEADER_BYTES'] = 512
+        header['DIM'] = 2
+        header['BYTE_ORDER'] = 'little_endian'
+        header['TYPE'] = 'unsigned_short'
+        header['SIZE1'] = shape_x
+        header['SIZE2'] = shape_y
+        header['PIXEL_SIZE'] = self.physical_pixelsize
+        header['BIN'] = '1x1'
+        header['BIN_TYPE'] = 'HW'
+        header['ADC'] = 'fast'
+        header['CREV'] = 1
+        header['BEAMLINE'] = self.name      # special ID for DIALS
+        header['DETECTOR_SN'] = 901         # special ID for DIALS
+        header['DATE'] = date
+        header['TIME'] = str(h['ImageExposureTime'])
+        header['DISTANCE'] = f'{self.distance:.4f}'
+        header['TWOTHETA'] = 0.00
+        header['PHI'] = '{phi:.4f}'
+        header['OSC_START'] = f'{phi:.4f}'
+        header['OSC_RANGE'] = f'{self.osc_angle:.4f}'
+        header['WAVELENGTH'] = f'{self.wavelength:.4f}'
+        # reverse XY coordinates for XDS
+        header['BEAM_CENTER_X'] = f'{mean_beam_center[1]:.4f}'
+        header['BEAM_CENTER_Y'] = f'{mean_beam_center[0]:.4f}'
+        header['DENZO_X_BEAM'] = f'{mean_beam_center[0]*self.physical_pixelsize:.4f}'
+        header['DENZO_Y_BEAM'] = f'{mean_beam_center[1]*self.physical_pixelsize:.4f}'
+        fn = path / f'{i:05d}.img'
+        write_adsc(fn, img, header=header)
+        return fn
+
+    def write_mrc(self, path: str, i: int) -> str:
+        """Write the image+header with sequence number `i` to the directory
+        `path` in TIFF format.
+
+        Returns the path to the written image.
+        """
+        img = self.data[i]
+
+        fn = path / f'{i:05d}.mrc'
+
+        # for RED these need to be as integers
+        dtype = np.uint16
+        if False:
+            # Use maximum range available in data type for extra precision when converting from FLOAT to INT
+            dynamic_range = 11900  # a little bit higher just in case
+            maxval = np.iinfo(dtype).max
+            img = (img / dynamic_range) * maxval
+
+        img = np.round(img, 0).astype(dtype)
+
+        # flip up/down because RED reads images from the bottom left corner
+        img = np.flipud(img)
+
+        write_mrc(fn, img)
+
+        return fn
+
+    def write_ed3d(self, path: str) -> None:
+        """Write .ed3d input file for REDp in directory `path`"""
+        path.mkdir(exist_ok=True)
+
+        omega = np.degrees(self.rotation_axis)
+
+        # for red, -180 <= omega <= 180
+        if omega < -180:
+            omega += 360
+        elif omega > 180:
+            omega -= 360
+
+        if self.start_angle > self.end_angle:
+            sign = -1
+        else:
+            sign = 1
+
+        with open(path / '1.ed3d', 'w') as f:
+            print(f'WAVELENGTH    {self.wavelength}', file=f)
+            print(f'ROTATIONAXIS    {omega:5f}', file=f)
+            print(f'CCDPIXELSIZE    {self.pixelsize:5f}', file=f)
+            print(f'GONIOTILTSTEP    {self.osc_angle:5f}', file=f)
+            print('BEAMTILTSTEP    0', file=f)
+            print('BEAMTILTRANGE    0.000', file=f)
+            print('STRETCHINGMP    0.0', file=f)
+            print('STRETCHINGAZIMUTH    0.0', file=f)
+            print('', file=f)
+            print('FILELIST', file=f)
+
+            for i in self.observed_range:
+                fn = f'{i:05d}.mrc'
+                angle = self.start_angle + sign * self.osc_angle * i
+                print(f'FILE {fn}    {angle: 12.4f}    0    {angle: 12.4f}', file=f)
+
+            print('ENDFILELIST', file=f)
+
+        logger.debug(f'ED3D file created in path: {path}')
+
+    def write_xds_inp(self, path: str) -> None:
+        """Write XDS.INP input file for XDS in directory `path`"""
+
+        path.mkdir(exist_ok=True)
+
+        nframes = max(self.complete_range)
+
+        invert_rotation_axis = self.start_angle > self.end_angle
+        rot_x, rot_y, rot_z = rotation_axis_to_xyz(self.rotation_axis, invert=invert_rotation_axis)
+
+        shape_x, shape_y = self.data_shape
+
+        if self.do_stretch_correction:
+            self.write_geometric_correction_files(path)
+            stretch_correction = 'DETECTOR= PILATUS      ! Pretend to be PILATUS detector to enable geometric corrections\nX-GEO_CORR= XCORR.cbf  ! X stretch correction\nY-GEO_CORR= YCORR.cbf  ! Y stretch correction\n'
+        else:
+            stretch_correction = ''
+
+        if self.missing_range:
+            exclude = '\n'.join([f'EXCLUDE_DATA_RANGE={i} {j}' for i, j in find_subranges(self.missing_range)])
+        else:
+            exclude = '!EXCLUDE_DATA_RANGE='
+
+        untrusted_areas = ''
+
+        for kind, coords in self.untrusted_areas:
+            untrusted_areas += to_xds_untrusted_area(kind, coords) + '\n'
+
+        s = self.XDS_template.format(
+            date=str(time.ctime()),
+            data_drc=self.smv_subdrc,
+            data_begin=1,
+            data_end=nframes,
+            exclude=exclude,
+            stretch_correction=stretch_correction,
+            starting_angle=self.start_angle,
+            wavelength=self.wavelength,
+            # reverse XY coordinates for XDS
+            origin_x=self.mean_beam_center[1],
+            origin_y=self.mean_beam_center[0],
+            untrusted_areas=untrusted_areas,
+            NX=shape_y,
+            NY=shape_x,
+            sign='+',
+            detector_distance=self.distance,
+            QX=self.physical_pixelsize,
+            QY=self.physical_pixelsize,
+            osc_angle=self.osc_angle,
+            rot_x=rot_x,
+            rot_y=rot_y,
+            rot_z=rot_z,
+        )
+
+        with open(path / 'XDS.INP', 'w') as f:
+            print(s, file=f)
+
+        logger.info('XDS INP file created.')
+
+    def write_beam_centers(self, path: str) -> None:
+        """Write list of beam centers to file `beam_centers.txt` in `path`"""
+        centers = np.zeros((max(self.observed_range), 2), dtype=float)
+        for i, h in self.headers.items():
+            centers[i - 1] = h['beam_center']
+        for i in self.missing_range:
+            centers[i - 1] = [np.NaN, np.NaN]
+
+        np.savetxt(path / 'beam_centers.txt', centers, fmt='%10.4f')
+
+    def write_pets_inp(self, path: str, tiff_path: str = 'tiff') -> None:
+        """Write PETS input file `pets.pts` in directory `path`"""
+        if self.start_angle > self.end_angle:
+            sign = -1
+        else:
+            sign = 1
+
+        omega = np.degrees(self.rotation_axis)
+
+        # for pets, 0 <= omega <= 360
+        if omega < 0:
+            omega += 360
+        elif omega > 360:
+            omega -= 360
+
+        with open(path / 'pets.pts', 'w') as f:
+            date = str(time.ctime())
+            print('# PETS input file for Rotation Electron Diffraction generated by `instamatic`', file=f)
+            print(f'# {date}', file=f)
+            print('# For definitions of input parameters, see:', file=f)
+            print('# http://pets.fzu.cz/ ', file=f)
+            print('', file=f)
+            print(f'lambda {self.wavelength}', file=f)
+            print(f'Aperpixel {self.pixelsize}', file=f)
+            print('phi 0.0', file=f)
+            print(f'omega {omega}', file=f)
+            print('bin 1', file=f)
+            print('reflectionsize 20', file=f)
+            print('noiseparameters 3.5 38', file=f)
+            print('', file=f)
+            # print("reconstructions", file=f)
+            # print("endreconstructions", file=f)
+            # print("", file=f)
+            # print("distortions", file=f)
+            # print("enddistortions", file=f)
+            # print("", file=f)
+            print('imagelist', file=f)
+            for i in self.observed_range:
+                fn = f'{i:05d}.tiff'
+                angle = self.start_angle + sign * self.osc_angle * i
+                print(f'{tiff_path}/{fn} {angle:10.4f} 0.00', file=f)
+            print('endimagelist', file=f)
+
+    def write_pets2_inp(self, path: str, tiff_path: str = 'tiff') -> None:
+        """Write PETS 2 input file `pets.pts2` in directory `path`"""
+        path.mkdir(exist_ok=True, parents=True)
+
+        if self.start_angle > self.end_angle:
+            sign = -1
+        else:
+            sign = 1
+
+        omega = np.degrees(self.rotation_axis)
+
+        with open(path / 'pets.pts2', 'w') as f:
+            date = str(time.ctime())
+            print('# PETS 2 input file for Rotation Electron Diffraction generated by `instamatic`', file=f)
+            print(f'# {date}', file=f)
+            print('# For definitions of input parameters, see:', file=f)
+            print('# http://pets.fzu.cz/ ', file=f)
+            print('', file=f)
+            print('geometry continuous', file=f)
+            print(f'lambda {self.wavelength}', file=f)
+            print(f'Aperpixel {self.pixelsize}', file=f)
+            print(f'phi {float(self.osc_angle)/2}', file=f)
+            print(f'omega {omega}', file=f)
+            print('bin 1', file=f)
+            print('reflectionsize 15', file=f)
+            print('noiseparameters 25 10', file=f)
+            print('i/sigma    5.00   10.00', file=f)
+            print('', file=f)
+            print('imagelist', file=f)
+            tiff_set = {0}
+            last_img = len(self.observed_range)
+            tiff_set.update(self.observed_range)
+            tiff_set.remove(last_img)
+            for i in tiff_set:
+                fn = f'{i:04d}.tiff'
+                angle = self.start_angle + sign * self.osc_angle * i
+                print(f'{tiff_path}/{fn} {angle:10.4f} 0.00', file=f)
+            print('endimagelist', file=f)
+
+    def write_REDp_shiftcorrection(self, path: str) -> None:
+        """Write .sc (shift correction) file for REDp in directory `path`"""
+        path.mkdir(exist_ok=True)
+
+        cx, cy = self.mean_beam_center
+        with open(path / 'shifts.sc', 'w') as f:
+            print(f' {cy:.2f} {cx:.2f}', file=f)  # cx/cy must be switched around, y first
+            for i in self.observed_range:
+                print(f'{i:4d}{0:8.2f}{0:8.2f}', file=f)
+
+    def add_beamstop(self, rect):
+        """rect must be a 2x4 coordinate array."""
+        self.untrusted_areas.append(('quadrilateral', rect))
```

### Comparing `instamatic-1.8.0/instamatic/processing/ImgConversionDM.py` & `instamatic-1.9.0/instamatic/processing/ImgConversionDM.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/processing/ImgConversionTPX.py` & `instamatic-1.9.0/instamatic/processing/ImgConversionTPX.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/processing/ImgConversionTVIPS.py` & `instamatic-1.9.0/instamatic/processing/ImgConversionTVIPS.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/processing/XDS_template.py` & `instamatic-1.9.0/instamatic/processing/XDS_template.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/processing/XDS_templateDM.py` & `instamatic-1.9.0/instamatic/processing/XDS_templateDM.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/processing/XDS_templateTPX.py` & `instamatic-1.9.0/instamatic/processing/XDS_templateTPX.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/processing/XDS_templateTVIPS.py` & `instamatic-1.9.0/instamatic/processing/XDS_templateTVIPS.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/processing/find_crystals.py` & `instamatic-1.9.0/instamatic/processing/find_crystals.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,19 @@
 from collections import namedtuple
 
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy import ndimage
 from scipy._lib._util import _asarray_validated
 from scipy.cluster.vq import kmeans2
-from skimage import filters
-from skimage import measure
-from skimage import morphology
-from skimage import segmentation
+from skimage import filters, measure, morphology, segmentation
 
 from instamatic.config import calibration
 from instamatic.image_utils import autoscale
 
-
 CrystalPosition = namedtuple('CrystalPosition', ['x', 'y', 'isolated', 'n_clusters', 'area_micrometer', 'area_pixel'])
 
 
 def isedge(prop):
     """Simple edge detection routine.
 
     Checks if the bbox of the prop matches the shape of the array. Uses
@@ -203,16 +199,17 @@
     parser.add_argument('args',
                         type=str, nargs='*', metavar='IMG',
                         help='Images to find crystals in.')
 
     options = parser.parse_args()
     args = options.args
 
-    from instamatic.formats import read_image
     import warnings
+
+    from instamatic.formats import read_image
     warnings.simplefilter('ignore')
 
     for fn in args:
         img, h = read_image(fn)
 
         crystals = find_crystals_timepix(img, h['exp_magnification'], plot=True)
```

### Comparing `instamatic-1.8.0/instamatic/processing/find_crystals_ilastik.py` & `instamatic-1.9.0/instamatic/processing/find_crystals_ilastik.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,14 +122,15 @@
             if action.dest == arg:
                 group._group_actions.remove(action)
                 return
 
 
 def main_entry():
     import argparse
+
     from predicrystal import parsers
 
     # Re-use parsers from `predicrystal`
     parents = (
         parsers.test_data_parser(add_help=False),
         # parsers.project_file_parser(add_help=False),
         parsers.output_parser(add_help=False),
```

### Comparing `instamatic-1.8.0/instamatic/processing/find_holes.py` & `instamatic-1.9.0/instamatic/processing/find_holes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import sys
 
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy import ndimage
-from skimage import color
-from skimage import filters
-from skimage import measure
-from skimage import morphology
-from skimage import segmentation
+from skimage import color, filters, measure, morphology, segmentation
 
 from instamatic.config import calibration
 from instamatic.image_utils import autoscale
 
 plt.rcParams['image.cmap'] = 'gray'
 
 
@@ -45,15 +41,15 @@
     from matplotlib.patches import Rectangle
 
     fig = plt.figure(figsize=(15, 10))
     ax = fig.add_subplot(111)
     plt.imshow(img, interpolation='none')
 
     for i, prop in enumerate(props):
-        y1, x1, y2, x2 = [x * scale for x in prop.bbox]
+        y1, x1, y2, x2 = (x * scale for x in prop.bbox)
 
         color = 'red'
 
         rect = Rectangle((x1 - 1, y1 - 1), x2 - x1 + 1,
                          y2 - y1 + 1, fc='none', ec=color, lw=2)
         ax.add_patch(rect)
 
@@ -112,15 +108,14 @@
     binsize: int,
         binning used for the data collection (1, 2, or 4)
 
     Returns:
         area: float,
             apprximate feature size in pixels
     """
-
     px = py = calibration['lowmag']['pixelsize'][magnification] / 1000  # nm -> um
     px *= (binsize / img_scale)
     py *= (binsize / img_scale)
     hole_area = (np.pi * (diameter / 2.0)**2) / (px * py)
     return hole_area
```

### Comparing `instamatic-1.8.0/instamatic/processing/flatfield.py` & `instamatic-1.9.0/instamatic/processing/flatfield.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import time
 import warnings
 from pathlib import Path
 
 import numpy as np
 from tqdm.auto import tqdm
 
-from instamatic import config
-from instamatic import TEMController
+from instamatic import TEMController, config
 from instamatic.formats import *
 
 
 def apply_corrections(img, deadpixels=None):
     """Apply image corrections."""
     if deadpixels is None:
         deadpixels = get_deadpixels(img)
@@ -56,15 +55,14 @@
 
 
 def apply_flatfield_correction(img, flatfield, darkfield=None):
     """Apply flatfield correction to image.
 
     https://en.wikipedia.org/wiki/Flat-field_correction
     """
-
     if flatfield.shape != img.shape:
         msg = f'Flatfield not applied: image {img.shape} and flatfield {flatfield.shape} do not match shapes.'
         warnings.warn(msg)
         return img
 
     if darkfield is None:
         ret = img * np.mean(flatfield) / flatfield
```

### Comparing `instamatic-1.8.0/instamatic/processing/stretch_correction.py` & `instamatic-1.9.0/instamatic/processing/stretch_correction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import math
 import sys
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.widgets import Slider
-from scipy.ndimage import interpolation
-from scipy.ndimage import morphology
+from scipy.ndimage import interpolation, morphology
 from skimage.feature import canny
-from skimage.measure import label
-from skimage.measure import regionprops
+from skimage.measure import label, regionprops
 
 from instamatic.formats import read_tiff
 from instamatic.image_utils import autoscale
 
 
 def apply_transform_to_image(img, transform, center=None):
     """Applies transformation matrix to image and recenters it
```

### Comparing `instamatic-1.8.0/instamatic/server/TEMServer_FEI.py` & `instamatic-1.9.0/instamatic/server/TEMServer_FEI.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 usage."""
 import datetime
 import logging
 import subprocess as sp
 import threading
 from socket import *
 
-from instamatic import config
-from instamatic import TEMController
-
+from instamatic import TEMController, config
 
 HOST = config.settings.fei_server_host
 PORT = config.settings.fei_server_port
 
 
 def handle(conn):
     while True:
```

### Comparing `instamatic-1.8.0/instamatic/server/cam_server.py` & `instamatic-1.9.0/instamatic/server/cam_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import queue
 import socket
 import threading
 import traceback
 
 import numpy as np
 
-from .serializer import dumper
-from .serializer import loader
 from instamatic import config
 from instamatic.camera import Camera
 from instamatic.utils import high_precision_timers
+
+from .serializer import dumper, loader
+
 high_precision_timers.enable()
 
 if config.settings.cam_use_shared_memory:
     from multiprocessing import shared_memory
 
 condition = threading.Condition()
 box = []
```

### Comparing `instamatic-1.8.0/instamatic/server/dials_server.py` & `instamatic-1.9.0/instamatic/server/dials_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import sys
 import threading
 from pathlib import Path
 from socket import *
 
 from instamatic import config
 
-
 try:
     EXE = Path(sys.argv[1])
 except BaseException:
     EXE = Path(config.settings.dials_script)
 
 CWD = EXE.parent
```

### Comparing `instamatic-1.8.0/instamatic/server/goniotool_server.py` & `instamatic-1.9.0/instamatic/server/goniotool_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import logging
 import pickle
 import queue
 import socket
 import threading
 import traceback
 
-from .serializer import dumper
-from .serializer import loader
 from instamatic import config
 from instamatic.goniotool import GonioToolWrapper
 
+from .serializer import dumper, loader
+
 barrier = threading.Barrier(2, timeout=60)
 
 condition = threading.Condition()
 box = []
 
 
 HOST = config.settings.goniotool_server_host
@@ -42,15 +42,15 @@
         self._name = name
 
         self.verbose = False
 
     def run(self):
         """Start the server thread."""
         self.goniotool = GonioToolWrapper(barrier=barrier)
-        print(f'Initialized connection to GonioTool')
+        print('Initialized connection to GonioTool')
 
         while True:
             now = datetime.datetime.now().strftime('%H:%M:%S.%f')
 
             cmd = self.q.get()
 
             with condition:
```

### Comparing `instamatic-1.8.0/instamatic/server/serializer.py` & `instamatic-1.9.0/instamatic/server/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import pickle
 
 import yaml
 
 from instamatic.config import settings
+
 PROTOCOL = settings.tem_communication_protocol
 
 # %timeit ctrl.stage.get()
 # - pickle:  287 µs ± 10.7 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
 # - json:    320 µs ± 55.8 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
 # - msgpack: 512 µs ± 27.2 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
 # - yaml:   4.43 ms ± 13.7 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
```

### Comparing `instamatic-1.8.0/instamatic/server/tem_server.py` & `instamatic-1.9.0/instamatic/server/tem_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import logging
 import pickle
 import queue
 import socket
 import threading
 import traceback
 
-from .serializer import dumper
-from .serializer import loader
 from instamatic import config
 from instamatic.TEMController import Microscope
 
+from .serializer import dumper, loader
+
 condition = threading.Condition()
 box = []
 
 HOST = config.settings.tem_server_host
 PORT = config.settings.tem_server_port
 BUFSIZE = 1024
```

### Comparing `instamatic-1.8.0/instamatic/server/vm_ubuntu_server.py` & `instamatic-1.9.0/instamatic/server/vm_ubuntu_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 PORT = config.settings.VM_server_port
 VM_ID = config.settings.VM_ID
 VM_USERNAME = config.settings.VM_USERNAME
 VM_PWD = config.settings.VM_PWD
 VM_DELAY1 = config.settings.VM_STARTUP_DELAY
 VM_DELAY2 = config.settings.VM_DESKTOP_DELAY
 VM_SF = config.settings.VM_SHARED_FOLDER
-#ENABLE_SHELXT = config.settings.ENABLE_SHELXT
+# ENABLE_SHELXT = config.settings.ENABLE_SHELXT
 BUFF = 1024
 
 
 def start_vm_process(vmname=VM_ID, vmachine_pwd=VM_PWD, time_delay=VM_DELAY1, mode='headless'):
     """mode can be either gui or headless."""
     try:
         vbox = virtualbox.VirtualBox()
@@ -71,15 +71,15 @@
     print(stdout)
 
 
 def vm_ubuntu_start_xds_AtFolder(session, conn, shelxt, unitcell, spgr, composition):
     """incoming conn should contain a path that is shared already between VBox
     and windows."""
 
-    #path = "/media/sf_SharedWithVM/test_vm_server"
+    # path = "/media/sf_SharedWithVM/test_vm_server"
 
     while True:
 
         try:
             data = conn.recv(BUFF).decode()
         except ConnectionResetError:
             print('cRED experiment ended and connection was forcely closed.')
@@ -143,25 +143,25 @@
 
 
 def generate_shelxt_input(unitcell, spgr, composition, path):
     from edtools.make_shelx import comp2dict, get_latt_symm_cards, get_sfac
     composition = comp2dict(composition)
 
     if unitcell is None:
-        with open(Path(path) / 'CORRECT.LP', 'r') as f:
+        with open(Path(path) / 'CORRECT.LP') as f:
             for line in f:
                 if line.startswith(' UNIT_CELL_CONSTANTS='):
                     cell = list(map(float, line.strip('\n').split()[1:7]))
                 elif line.startswith(' UNIT CELL PARAMETERS'):
                     cell = list(map(float, line.strip('\n').split()[3:9]))
     else:
         cell = [float(ucl) for ucl in unitcell]
 
     if spgr is None:
-        with open(Path(path) / 'CORRECT.LP', 'r') as f:
+        with open(Path(path) / 'CORRECT.LP') as f:
             for line in f:
                 if line.startswith(' SPACE GROUP NUMBER'):
                     spgr = int(line.strip('\n').split()[-1])
                 elif line.startswith(' SPACE_GROUP_NUMBER='):
                     spgr = int(line.strip('\n').split()[1])
     else:
         spgr = str(spgr)
@@ -171,15 +171,15 @@
     spgr = str(spgr)
     out = Path(path) / 'shelx.ins'
 
     f = open(out, 'w')
 
     print(f'TITL {spgr}', file=f)
     print(f'CELL {wavelength:.4f} {a:6.3f} {b:6.3f} {c:6.3f} {al:7.3f} {be:7.3f} {ga:7.3f}', file=f)
-    print(f'ZERR 1.00    0.000  0.000  0.000   0.000   0.000   0.000', file=f)
+    print('ZERR 1.00    0.000  0.000  0.000   0.000   0.000   0.000', file=f)
 
     LATT, SYMM = get_latt_symm_cards(spgr)
 
     print(LATT, file=f)
     for line in SYMM:
         print(line, file=f)
 
@@ -260,15 +260,15 @@
     options = parser.parse_args()
 
     shelxt = options.shelxt
     unitcell = options.unitcell
     spgr = options.spgr
     composition = options.composition
 
-    #print(shelxt, unitcell, spgr, composition)
+    # print(shelxt, unitcell, spgr, composition)
 
     total_wait_sec = VM_DELAY1 + VM_DELAY2 + 10
     print('Starting Ubuntu server installed in VirtualBox...')
     print(f'Please allow around {total_wait_sec} sec for VM to finish start-up process.')
     session = start_vm_process()
     time.sleep(VM_DELAY2)
     vm_ubuntu_start_terminal(session)
@@ -297,12 +297,12 @@
             threading.Thread(target=vm_ubuntu_start_xds_AtFolder, args=(session, conn, shelxt, unitcell, spgr, composition)).start()
 
     # time.sleep(5)
     # vm_ubuntu_start_xds_AtFolder(session)
     # time.sleep(5)
     # close_down_vm_process(session)
     # time.sleep(5)
-    #print("VM server closed down safely!")
+    # print("VM server closed down safely!")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `instamatic-1.8.0/instamatic/server/xds_server.py` & `instamatic-1.9.0/instamatic/server/xds_server.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/tools.py` & `instamatic-1.9.0/instamatic/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import glob
 import os
 import sys
 from pathlib import Path
 
 import numpy as np
-from scipy import interpolate
-from scipy import ndimage
+from scipy import interpolate, ndimage
 from skimage import exposure
 from skimage.measure import regionprops
 
 
 def prepare_grid_coordinates(nx: int, ny: int, stepsize: float = 1.0) -> 'np.array':
     """Prepare a list of grid coordinates nx by ny in size. The grid is
     centered at the center of the grid.
@@ -68,16 +67,16 @@
     else:
         raise ValueError('Only quadrilaterals are supported for now')
 
 
 def find_subranges(lst: list) -> (int, int):
     """Takes a range of sequential numbers (possibly with gaps) and splits them
     in sequential sub-ranges defined by the minimum and maximum value."""
-    from operator import itemgetter
     from itertools import groupby
+    from operator import itemgetter
 
     for key, group in groupby(enumerate(lst), lambda i: i[0] - i[1]):
         group = list(map(itemgetter(1), group))
         yield min(group), max(group)
 
 
 def find_peak_max(arr: np.ndarray, sigma: int, m: int = 50, w: int = 10, kind: int = 3) -> (float, float):
@@ -137,15 +136,14 @@
     `gauss` applies a gaussian filter with a very large standard deviation in an attempt
     to smooth out the beam stop. The position of the largest pixel corresponds to the
     beam center.
 
     z = thresh: percentile to segment the image at (99)
         gauss: standard deviation for the gaussian blurring (50)
     """
-
     if method == 'gauss':
         if not z:
             z = 50
         blurred = ndimage.filters.gaussian_filter(img, z)
         cx, cy = np.unravel_index(blurred.argmax(), blurred.shape)
 
     elif method == 'thresh':
@@ -158,16 +156,16 @@
         props.sort(key=lambda x: x.area, reverse=True)
         prop = props[0]
 
         dx = (prop.bbox[0] + prop.bbox[2]) / 2
         dy = (prop.bbox[1] + prop.bbox[3]) / 2
 
         if plot:
-            import matplotlib.pyplot as plt
             import matplotlib.patches as mpatches
+            import matplotlib.pyplot as plt
 
             fig, (ax1, ax2) = plt.subplots(ncols=2)
 
             ax1.imshow(labeled, vmax=5)
             ax2.imshow(img, vmax=np.percentile(img, z))
 
             ax1.scatter(dy, dx)
@@ -219,17 +217,17 @@
     drc : str
         Location where to store the image
 
     Returns
     -------
     Namespace with acquisition/exposure/overhead time in s
     """
+    from types import SimpleNamespace
 
     from scipy.stats import linregress
-    from types import SimpleNamespace
 
     timestamps = np.array(timestamps)
 
     x = np.arange(len(timestamps))
     res = linregress(x, timestamps)
 
     y = x * res.slope + res.intercept
@@ -256,15 +254,14 @@
 def relativistic_wavelength(voltage: float = 200_000) -> float:
     """Calculate the relativistic wavelength of electrons from the accelarating
     voltage.
 
     Input: Voltage in V
     Output: Wavelength in Angstrom
     """
-
     h = 6.626070150e-34  # planck constant J.s
     m = 9.10938356e-31   # electron rest mass kg
     e = 1.6021766208e-19  # elementary charge C
     c = 299792458        # speed of light m/s
 
     wl = h / (2 * m * voltage * e * (1 + (e * voltage) / (2 * m * c**2)))**0.5
```

### Comparing `instamatic-1.8.0/instamatic/utils/beamstop.py` & `instamatic-1.9.0/instamatic/utils/beamstop.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,213 +1,213 @@
-from pathlib import Path
-
-import numpy as np
-from skimage import morphology
-from skimage.measure import find_contours
-
-from instamatic.formats import read_tiff
-from instamatic.tools import find_beam_center_with_beamstop
-
-
-def minimum_bounding_rectangle(points):
-    """# From https://stackoverflow.com/a/33619018.
-
-    Find the smallest bounding rectangle for a set of points.
-    Returns a set of points representing the corners of the bounding box.
-
-    :param points: an nx2 matrix of coordinates
-    :rval: an nx2 matrix of coordinates
-    """
-    from scipy.spatial import ConvexHull
-
-    pi2 = np.pi / 2.0
-
-    # get the convex hull for the points
-    hull_points = points[ConvexHull(points).vertices]
-
-    # calculate edge angles
-    edges = np.zeros((len(hull_points) - 1, 2))
-    edges = hull_points[1:] - hull_points[:-1]
-
-    angles = np.zeros(len(edges))
-    angles = np.arctan2(edges[:, 1], edges[:, 0])
-
-    angles = np.abs(np.mod(angles, pi2))
-    angles = np.unique(angles)
-
-    # find rotation matrices
-    rotations = np.vstack([
-        np.cos(angles),
-        np.cos(angles - pi2),
-        np.cos(angles + pi2),
-        np.cos(angles)]).T
-
-    rotations = rotations.reshape((-1, 2, 2))
-
-    # apply rotations to the hull
-    rot_points = np.dot(rotations, hull_points.T)
-
-    # find the bounding points
-    min_x = np.nanmin(rot_points[:, 0], axis=1)
-    max_x = np.nanmax(rot_points[:, 0], axis=1)
-    min_y = np.nanmin(rot_points[:, 1], axis=1)
-    max_y = np.nanmax(rot_points[:, 1], axis=1)
-
-    # find the box with the best area
-    areas = (max_x - min_x) * (max_y - min_y)
-    best_idx = np.argmin(areas)
-
-    # return the best box
-    x1 = max_x[best_idx]
-    x2 = min_x[best_idx]
-    y1 = max_y[best_idx]
-    y2 = min_y[best_idx]
-    r = rotations[best_idx]
-
-    rval = np.zeros((4, 2))
-    rval[0] = np.dot([x1, y2], r)
-    rval[1] = np.dot([x2, y2], r)
-    rval[2] = np.dot([x2, y1], r)
-    rval[3] = np.dot([x1, y1], r)
-
-    return rval
-
-
-def radial_average(z, center, as_radial_map=False):
-    """Calculate the radial profile by azimuthal averaging about a specified
-    center.
-
-    Parameters
-    ----------
-    center : array
-        The array indices of the diffraction pattern center about which the
-        radial integration is performed.
-    as_radial_map : bool
-        Return the radial average mapped to the pixel positions of the 2D image
-
-    Returns
-    -------
-    radial_profile : array
-        Radial profile of the diffraction pattern.
-    """
-    y, x = np.indices(z.shape)
-    r = np.sqrt((x - center[1])**2 + (y - center[0])**2)
-    r = r.astype(int)
-
-    tbin = np.bincount(r.ravel(), z.ravel())
-    nr = np.bincount(r.ravel())
-    averaged = tbin / nr
-
-    if as_radial_map:
-        return averaged[r]
-    else:
-        return averaged
-
-
-def find_beamstop_rect(img, center=None, threshold=0.5, pad=1, minsize=500, savefig=False, drc='.'):
-    """Find rectangle fitting the beamstop.
-
-    1. Radially scale the image (divide each point in the image by the radial average)
-    2. Segment the image via thresholding. The beamstop is identified by the area where the image < radially scaled image
-    3. Contour the segmented image.
-    4. Find minimum bounding rectangle for points that define the contours
-    5. The contour closest to the beam center is then taken as beamstop
-
-    input:
-        image, nxn 2D np.array defining the image. The average of the image stack works well
-        center, 2x1 np.array defining the center of the image. If omitted, will be find automatically
-        threshold, float representing the threshold value for segmentation
-        pad, int defining the padding of the beamstop to make it seem a bit larger
-        minsize, int defining minimum size of the beamstop
-        savefig, boolean that defines whether the result should be saved
-        drc, location where to place the image is saved
-
-    output:
-        4x2 np.array defining the corners of the rectangle
-    """
-
-    if center is None:
-        center = find_beam_center_with_beamstop(img, z=99)
-
-    # get radially averaged image
-    r_map = radial_average(img, center=center, as_radial_map=True)
-
-    radial_scaled = img / r_map
-
-    # image segmentation
-    seg = radial_scaled < threshold
-
-    seg = morphology.remove_small_objects(seg, 64)
-    seg = morphology.remove_small_holes(seg, 64)
-
-    # pad the beamstop to make the outline a big bigger
-    if pad:
-        seg = morphology.binary_dilation(seg, selem=morphology.disk(pad))
-
-    arr = find_contours(seg, 0.5)
-
-    if len(arr) > 1:
-        rects = [minimum_bounding_rectangle(a) for a in arr if len(a) > minsize]
-
-        a = [np.mean(rect, axis=0) for rect in rects]
-        dists = [np.linalg.norm(b - center) for b in a]
-        i = np.argmin(dists)
-
-        rect = rects[i]
-    else:
-        a = arr[0]
-        rect = minimum_bounding_rectangle(a)
-
-    # This is not robust if there are other shaded areas
-    # rect = sorted(arr, key=lambda x: len(x), reverse=True)[0]
-    # rect = minimum_bounding_rectangle(beamstop)
-
-    if savefig:
-        import matplotlib
-        matplotlib.use('pdf')
-        import matplotlib.pyplot as plt
-
-        fig, (ax1, ax2, ax3) = plt.subplots(ncols=3, figsize=(16, 8))
-        for ax in ax1, ax2, ax3:
-            ax.axis('off')
-
-        ax1.imshow(radial_scaled, vmax=np.percentile(radial_scaled, 99))
-        ax1.set_title('Radially scaled image')
-
-        cx, cy = center
-        ax1.scatter(cy, cx, marker='+', color='red')
-
-        ax2.imshow(seg)
-        ax2.set_title('Segmented image')
-
-        ax3.imshow(img, vmax=np.percentile(img, 99))
-        ax3.set_title('Mean image showing beamstop')
-        ax3.scatter(cy, cx, marker='+')
-
-        bx, by = np.vstack((rect, rect[0])).T
-        ax3.plot(by, bx, 'r-o')
-
-        fn = Path(drc) / 'beamstop.png'
-        plt.savefig(fn, dpi=150, bbox_inches='tight', pad_inches=0.1)
-
-    return rect
-
-
-if __name__ == '__main__':
-    drc = '.'
-    fns = list(Path(drc).glob('raw/*.tif'))
-
-    print(len(fns))
-
-    imgs, hs = zip(*(read_tiff(fn) for fn in fns))
-
-    stack_mean = np.mean(imgs, axis=0)
-
-    center = find_beam_center_with_beamstop(stack_mean, z=99)
-
-    beamstop_rect = find_beamstop_rect(stack_mean, center, pad=1, plot=True)
-
-    from instamatic.tools import to_xds_untrusted_area
-
-    xds_quad = to_xds_untrusted_area('quadrilateral', beamstop_rect)
-
-    print(xds_quad)
+from pathlib import Path
+
+import numpy as np
+from skimage import morphology
+from skimage.measure import find_contours
+
+from instamatic.formats import read_tiff
+from instamatic.tools import find_beam_center_with_beamstop
+
+
+def minimum_bounding_rectangle(points):
+    """# From https://stackoverflow.com/a/33619018.
+
+    Find the smallest bounding rectangle for a set of points.
+    Returns a set of points representing the corners of the bounding box.
+
+    :param points: an nx2 matrix of coordinates
+    :rval: an nx2 matrix of coordinates
+    """
+    from scipy.spatial import ConvexHull
+
+    pi2 = np.pi / 2.0
+
+    # get the convex hull for the points
+    hull_points = points[ConvexHull(points).vertices]
+
+    # calculate edge angles
+    edges = np.zeros((len(hull_points) - 1, 2))
+    edges = hull_points[1:] - hull_points[:-1]
+
+    angles = np.zeros(len(edges))
+    angles = np.arctan2(edges[:, 1], edges[:, 0])
+
+    angles = np.abs(np.mod(angles, pi2))
+    angles = np.unique(angles)
+
+    # find rotation matrices
+    rotations = np.vstack([
+        np.cos(angles),
+        np.cos(angles - pi2),
+        np.cos(angles + pi2),
+        np.cos(angles)]).T
+
+    rotations = rotations.reshape((-1, 2, 2))
+
+    # apply rotations to the hull
+    rot_points = np.dot(rotations, hull_points.T)
+
+    # find the bounding points
+    min_x = np.nanmin(rot_points[:, 0], axis=1)
+    max_x = np.nanmax(rot_points[:, 0], axis=1)
+    min_y = np.nanmin(rot_points[:, 1], axis=1)
+    max_y = np.nanmax(rot_points[:, 1], axis=1)
+
+    # find the box with the best area
+    areas = (max_x - min_x) * (max_y - min_y)
+    best_idx = np.argmin(areas)
+
+    # return the best box
+    x1 = max_x[best_idx]
+    x2 = min_x[best_idx]
+    y1 = max_y[best_idx]
+    y2 = min_y[best_idx]
+    r = rotations[best_idx]
+
+    rval = np.zeros((4, 2))
+    rval[0] = np.dot([x1, y2], r)
+    rval[1] = np.dot([x2, y2], r)
+    rval[2] = np.dot([x2, y1], r)
+    rval[3] = np.dot([x1, y1], r)
+
+    return rval
+
+
+def radial_average(z, center, as_radial_map=False):
+    """Calculate the radial profile by azimuthal averaging about a specified
+    center.
+
+    Parameters
+    ----------
+    center : array
+        The array indices of the diffraction pattern center about which the
+        radial integration is performed.
+    as_radial_map : bool
+        Return the radial average mapped to the pixel positions of the 2D image
+
+    Returns
+    -------
+    radial_profile : array
+        Radial profile of the diffraction pattern.
+    """
+    y, x = np.indices(z.shape)
+    r = np.sqrt((x - center[1])**2 + (y - center[0])**2)
+    r = r.astype(int)
+
+    tbin = np.bincount(r.ravel(), z.ravel())
+    nr = np.bincount(r.ravel())
+    averaged = tbin / nr
+
+    if as_radial_map:
+        return averaged[r]
+    else:
+        return averaged
+
+
+def find_beamstop_rect(img, center=None, threshold=0.5, pad=1, minsize=500, savefig=False, drc='.'):
+    """Find rectangle fitting the beamstop.
+
+    1. Radially scale the image (divide each point in the image by the radial average)
+    2. Segment the image via thresholding. The beamstop is identified by the area where the image < radially scaled image
+    3. Contour the segmented image.
+    4. Find minimum bounding rectangle for points that define the contours
+    5. The contour closest to the beam center is then taken as beamstop
+
+    input:
+        image, nxn 2D np.array defining the image. The average of the image stack works well
+        center, 2x1 np.array defining the center of the image. If omitted, will be find automatically
+        threshold, float representing the threshold value for segmentation
+        pad, int defining the padding of the beamstop to make it seem a bit larger
+        minsize, int defining minimum size of the beamstop
+        savefig, boolean that defines whether the result should be saved
+        drc, location where to place the image is saved
+
+    output:
+        4x2 np.array defining the corners of the rectangle
+    """
+
+    if center is None:
+        center = find_beam_center_with_beamstop(img, z=99)
+
+    # get radially averaged image
+    r_map = radial_average(img, center=center, as_radial_map=True)
+
+    radial_scaled = img / r_map
+
+    # image segmentation
+    seg = radial_scaled < threshold
+
+    seg = morphology.remove_small_objects(seg, 64)
+    seg = morphology.remove_small_holes(seg, 64)
+
+    # pad the beamstop to make the outline a big bigger
+    if pad:
+        seg = morphology.binary_dilation(seg, selem=morphology.disk(pad))
+
+    arr = find_contours(seg, 0.5)
+
+    if len(arr) > 1:
+        rects = [minimum_bounding_rectangle(a) for a in arr if len(a) > minsize]
+
+        a = [np.mean(rect, axis=0) for rect in rects]
+        dists = [np.linalg.norm(b - center) for b in a]
+        i = np.argmin(dists)
+
+        rect = rects[i]
+    else:
+        a = arr[0]
+        rect = minimum_bounding_rectangle(a)
+
+    # This is not robust if there are other shaded areas
+    # rect = sorted(arr, key=lambda x: len(x), reverse=True)[0]
+    # rect = minimum_bounding_rectangle(beamstop)
+
+    if savefig:
+        import matplotlib
+        matplotlib.use('pdf')
+        import matplotlib.pyplot as plt
+
+        fig, (ax1, ax2, ax3) = plt.subplots(ncols=3, figsize=(16, 8))
+        for ax in ax1, ax2, ax3:
+            ax.axis('off')
+
+        ax1.imshow(radial_scaled, vmax=np.percentile(radial_scaled, 99))
+        ax1.set_title('Radially scaled image')
+
+        cx, cy = center
+        ax1.scatter(cy, cx, marker='+', color='red')
+
+        ax2.imshow(seg)
+        ax2.set_title('Segmented image')
+
+        ax3.imshow(img, vmax=np.percentile(img, 99))
+        ax3.set_title('Mean image showing beamstop')
+        ax3.scatter(cy, cx, marker='+')
+
+        bx, by = np.vstack((rect, rect[0])).T
+        ax3.plot(by, bx, 'r-o')
+
+        fn = Path(drc) / 'beamstop.png'
+        plt.savefig(fn, dpi=150, bbox_inches='tight', pad_inches=0.1)
+
+    return rect
+
+
+if __name__ == '__main__':
+    drc = '.'
+    fns = list(Path(drc).glob('raw/*.tif'))
+
+    print(len(fns))
+
+    imgs, hs = zip(*(read_tiff(fn) for fn in fns))
+
+    stack_mean = np.mean(imgs, axis=0)
+
+    center = find_beam_center_with_beamstop(stack_mean, z=99)
+
+    beamstop_rect = find_beamstop_rect(stack_mean, center, pad=1, plot=True)
+
+    from instamatic.tools import to_xds_untrusted_area
+
+    xds_quad = to_xds_untrusted_area('quadrilateral', beamstop_rect)
+
+    print(xds_quad)
```

### Comparing `instamatic-1.8.0/instamatic/utils/high_precision_timers.py` & `instamatic-1.9.0/instamatic/utils/high_precision_timers.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/utils/progress.py` & `instamatic-1.9.0/instamatic/utils/progress.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/instamatic/utils/spinbox.py` & `instamatic-1.9.0/instamatic/utils/spinbox.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     def __init__(self, master=None, **kw):
         """Construct a Ttk Spinbox widget with the parent master.
 
         STANDARD OPTIONS: class, cursor, style, takefocus, validate,
         validatecommand, xscrollcommand, invalidcommand
 
-        WIDGET-SPECIFIC OPTIONS: to, from_, increment, values, wrap, format, command
+        WIDGET-SPECIFIC OPTIONS: to, from_, increment, values, wrap,
+        format, command
         """
         Entry.__init__(self, master, 'ttk::spinbox', **kw)
 
     def set(self, value):
         """Sets the value of the Spinbox to value."""
         self.tk.call(self._w, 'set', value)
```

### Comparing `instamatic-1.8.0/instamatic/utils/xds_parser.py` & `instamatic-1.9.0/instamatic/utils/xds_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import shutil
 import sys
 import time
-from math import cos
-from math import radians
+from math import cos, radians
 from pathlib import Path
 
 
 def volume(cell):
     """Returns volume for the general case from cell parameters."""
     a, b, c, al, be, ga = cell
     al = radians(al)
@@ -30,15 +29,15 @@
         self.d = self.parse()
 
     def parse(self):
         ios_threshold = self.ios_threshold
 
         fn = self.filename
 
-        f = open(fn, 'r')
+        f = open(fn)
 
         in_block = False
         block = []
 
         d = {}
 
         for line in f:
```

### Comparing `instamatic-1.8.0/instamatic.egg-info/SOURCES.txt` & `instamatic-1.9.0/instamatic.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -68,20 +68,22 @@
 instamatic/camera/EMCameraObj.dll
 instamatic/camera/__init__.py
 instamatic/camera/camera.py
 instamatic/camera/camera_client.py
 instamatic/camera/camera_emmenu.py
 instamatic/camera/camera_gatan.py
 instamatic/camera/camera_gatan2.py
+instamatic/camera/camera_merlin.py
 instamatic/camera/camera_serval.py
 instamatic/camera/camera_simu.py
 instamatic/camera/camera_timepix.py
 instamatic/camera/fakevideostream.py
 instamatic/camera/gatansocket3.md
 instamatic/camera/gatansocket3.py
+instamatic/camera/merlin_io.py
 instamatic/camera/mpxhwrelaxd.dll
 instamatic/camera/timepix.lockfile
 instamatic/camera/videostream.py
 instamatic/camera/tpx/171207_with_flatfield.bpc
 instamatic/camera/tpx/171207_with_flatfield.bpc.dacs
 instamatic/camera/tpx/HW.dacs
 instamatic/camera/tpx/config.txt
@@ -92,14 +94,15 @@
 instamatic/config/settings.yaml
 instamatic/config/utils.py
 instamatic/config/alignments/neutral.yaml
 instamatic/config/calibration/orius.yaml
 instamatic/config/calibration/simulate.yaml
 instamatic/config/calibration/timepix.yaml
 instamatic/config/calibration/tvips-f416.yaml
+instamatic/config/camera/merlin.yaml
 instamatic/config/camera/orius.yaml
 instamatic/config/camera/serval.yaml
 instamatic/config/camera/simulate.yaml
 instamatic/config/camera/simulateDLL.yaml
 instamatic/config/camera/timepix.yaml
 instamatic/config/camera/tvips-f416.yaml
 instamatic/config/camera/tvips-xf416.yaml
@@ -148,16 +151,14 @@
 instamatic/gui/red_frame.py
 instamatic/gui/sed_frame.py
 instamatic/gui/videostream_frame.py
 instamatic/neural_network/__init__.py
 instamatic/neural_network/neural_network.py
 instamatic/neural_network/preprocess.py
 instamatic/neural_network/preprocess_SerialRED.py
-instamatic/neural_network/weights-py2.p
-instamatic/neural_network/weights-py3.p
 instamatic/processing/ImgConversion.py
 instamatic/processing/ImgConversionDM.py
 instamatic/processing/ImgConversionTPX.py
 instamatic/processing/ImgConversionTVIPS.py
 instamatic/processing/XDS_template.py
 instamatic/processing/XDS_templateDM.py
 instamatic/processing/XDS_templateTPX.py
@@ -204,12 +205,13 @@
 scripts/viewer.py
 tests/conftest.py
 tests/test_camera.py
 tests/test_ctrl.py
 tests/test_experiments.py
 tests/test_formats.py
 tests/test_grid_mapping.py
+tests/test_merlin_io.py
 tests/config/defaults.yaml
 tests/config/settings.yaml
 tests/config/calibration/test.yaml
 tests/config/camera/test.yaml
 tests/config/microscope/test.yaml
```

### Comparing `instamatic-1.8.0/instamatic.egg-info/entry_points.txt` & `instamatic-1.9.0/instamatic.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/notebooks/montage_processing.ipynb` & `instamatic-1.9.0/notebooks/montage_processing.ipynb`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 21% similar despite different names*

```diff
@@ -1,848 +1,822 @@
-00000000: 7b0d 0a20 2263 656c 6c73 223a 205b 0d0a  {.. "cells": [..
-00000010: 2020 7b0d 0a20 2020 2263 656c 6c5f 7479    {..   "cell_ty
-00000020: 7065 223a 2022 636f 6465 222c 0d0a 2020  pe": "code",..  
-00000030: 2022 6578 6563 7574 696f 6e5f 636f 756e   "execution_coun
-00000040: 7422 3a20 6e75 6c6c 2c0d 0a20 2020 226d  t": null,..   "m
-00000050: 6574 6164 6174 6122 3a20 7b7d 2c0d 0a20  etadata": {},.. 
-00000060: 2020 226f 7574 7075 7473 223a 205b 5d2c    "outputs": [],
-00000070: 0d0a 2020 2022 736f 7572 6365 223a 205b  ..   "source": [
-00000080: 0d0a 2020 2020 2225 6c6f 6164 5f65 7874  ..    "%load_ext
-00000090: 2061 7574 6f72 656c 6f61 645c 6e22 2c0d   autoreload\n",.
-000000a0: 0a20 2020 2022 2561 7574 6f72 656c 6f61  .    "%autoreloa
-000000b0: 6420 3222 0d0a 2020 205d 0d0a 2020 7d2c  d 2"..   ]..  },
-000000c0: 0d0a 2020 7b0d 0a20 2020 2263 656c 6c5f  ..  {..   "cell_
-000000d0: 7479 7065 223a 2022 6d61 726b 646f 776e  type": "markdown
-000000e0: 222c 0d0a 2020 2022 6d65 7461 6461 7461  ",..   "metadata
-000000f0: 223a 207b 7d2c 0d0a 2020 2022 736f 7572  ": {},..   "sour
-00000100: 6365 223a 205b 0d0a 2020 2020 2223 2049  ce": [..    "# I
-00000110: 6e73 7461 6d61 7469 6320 2d20 6d6f 6e74  nstamatic - mont
-00000120: 6167 696e 675c 6e22 2c0d 0a20 2020 2022  aging\n",..    "
-00000130: 5c6e 222c 0d0a 2020 2020 2249 6e73 7461  \n",..    "Insta
-00000140: 6d61 7469 6320 6973 2061 2074 6f6f 6c20  matic is a tool 
-00000150: 666f 7220 6175 746f 6d61 7465 6420 656c  for automated el
-00000160: 6563 7472 6f6e 2064 6966 6672 6163 7469  ectron diffracti
-00000170: 6f6e 2064 6174 6120 636f 6c6c 6563 7469  on data collecti
-00000180: 6f6e 2e20 4974 2068 6173 2069 6e74 6572  on. It has inter
-00000190: 6661 6365 7320 666f 7220 696e 7465 7266  faces for interf
-000001a0: 6163 696e 6720 7769 7468 2074 6865 2054  acing with the T
-000001b0: 454d 2028 4a45 4f4c 2f54 4653 2920 616e  EM (JEOL/TFS) an
-000001c0: 6420 7365 7665 7261 6c20 6361 6d65 7261  d several camera
-000001d0: 7320 2847 6174 616e 2f41 5349 2054 696d  s (Gatan/ASI Tim
-000001e0: 6570 6978 2f54 5649 5053 292e 5c6e 222c  epix/TVIPS).\n",
-000001f0: 0d0a 2020 2020 225c 6e22 2c0d 0a20 2020  ..    "\n",..   
-00000200: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
-00000210: 2e63 6f6d 2f69 6e73 7461 6d61 7469 632d  .com/instamatic-
-00000220: 6465 762f 696e 7374 616d 6174 6963 5c6e  dev/instamatic\n
-00000230: 222c 0d0a 2020 2020 225c 6e22 2c0d 0a20  ",..    "\n",.. 
-00000240: 2020 2022 5468 6973 206e 6f74 6562 6f6f     "This noteboo
-00000250: 6b20 7368 6f77 7320 686f 7720 746f 2070  k shows how to p
-00000260: 726f 6365 7373 2061 2067 7269 6420 6d6f  rocess a grid mo
-00000270: 6e74 6167 6520 7573 696e 6720 6069 6e73  ntage using `ins
-00000280: 7461 6d61 7469 6360 2c20 7069 636b 2067  tamatic`, pick g
-00000290: 7269 6420 7371 7561 7265 732c 2061 6e64  rid squares, and
-000002a0: 2073 6574 2075 7020 616e 2061 6371 7569   set up an acqui
-000002b0: 7369 7469 6f6e 2028 6061 6371 7569 7265  sition (`acquire
-000002c0: 5f61 745f 6974 656d 7360 292e 2054 6865  _at_items`). The
-000002d0: 2064 6174 6120 7765 7265 2063 6f6c 6c65   data were colle
-000002e0: 6374 6564 206f 6e20 6120 7a65 6f6c 6974  cted on a zeolit
-000002f0: 6520 7361 6d70 6c65 2028 3230 3230 2d30  e sample (2020-0
-00000300: 322d 3132 292c 2075 7369 6e67 2061 204a  2-12), using a J
-00000310: 454f 4c20 4a45 4d2d 3134 3030 2040 2031  EOL JEM-1400 @ 1
-00000320: 3230 206b 5620 696e 2063 6f6d 6269 6e61  20 kV in combina
-00000330: 7469 6f6e 2077 6974 6820 6120 5456 4950  tion with a TVIP
-00000340: 5320 462d 3431 3620 6361 6d65 7261 2e5c  S F-416 camera.\
-00000350: 6e22 2c0d 0a20 2020 2022 5c6e 222c 0d0a  n",..    "\n",..
-00000360: 2020 2020 2254 6865 2064 6174 6120 666f      "The data fo
-00000370: 7220 7468 6973 2064 656d 6f20 6172 6520  r this demo are 
-00000380: 6176 6169 6c61 626c 6520 6672 6f6d 207a  available from z
-00000390: 656e 6f64 6f3a 2068 7474 7073 3a2f 2f64  enodo: https://d
-000003a0: 6f69 2e6f 7267 2f31 302e 3532 3831 2f7a  oi.org/10.5281/z
-000003b0: 656e 6f64 6f2e 3339 3234 3038 395c 6e22  enodo.3924089\n"
-000003c0: 2c0d 0a20 2020 2022 5c6e 222c 0d0a 2020  ,..    "\n",..  
-000003d0: 2020 224d 616b 6520 7375 7265 2074 6f20    "Make sure to 
-000003e0: 6368 616e 6765 2074 6865 2077 6f72 6b20  change the work 
-000003f0: 6469 7265 6374 6f72 7920 6265 6c6f 7720  directory below 
-00000400: 746f 2070 6f69 6e74 2061 7420 7468 6520  to point at the 
-00000410: 7269 6768 7420 6c6f 6361 7469 6f6e 2e22  right location."
-00000420: 0d0a 2020 205d 0d0a 2020 7d2c 0d0a 2020  ..   ]..  },..  
-00000430: 7b0d 0a20 2020 2263 656c 6c5f 7479 7065  {..   "cell_type
-00000440: 223a 2022 636f 6465 222c 0d0a 2020 2022  ": "code",..   "
-00000450: 6578 6563 7574 696f 6e5f 636f 756e 7422  execution_count"
-00000460: 3a20 6e75 6c6c 2c0d 0a20 2020 226d 6574  : null,..   "met
-00000470: 6164 6174 6122 3a20 7b7d 2c0d 0a20 2020  adata": {},..   
-00000480: 226f 7574 7075 7473 223a 205b 5d2c 0d0a  "outputs": [],..
-00000490: 2020 2022 736f 7572 6365 223a 205b 0d0a     "source": [..
-000004a0: 2020 2020 2266 726f 6d20 696e 7374 616d      "from instam
-000004b0: 6174 6963 2e6d 6f6e 7461 6765 2069 6d70  atic.montage imp
-000004c0: 6f72 7420 2a5c 6e22 2c0d 0a20 2020 2022  ort *\n",..    "
-000004d0: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-000004e0: 6e70 5c6e 222c 0d0a 2020 2020 2266 726f  np\n",..    "fro
-000004f0: 6d20 7061 7468 6c69 6220 696d 706f 7274  m pathlib import
-00000500: 2050 6174 685c 6e22 2c0d 0a20 2020 2022   Path\n",..    "
-00000510: 6e70 2e73 6574 5f70 7269 6e74 6f70 7469  np.set_printopti
-00000520: 6f6e 7328 7375 7070 7265 7373 3d54 7275  ons(suppress=Tru
-00000530: 6529 5c6e 222c 0d0a 2020 2020 225c 6e22  e)\n",..    "\n"
-00000540: 2c0d 0a20 2020 2022 2320 776f 726b 2064  ,..    "# work d
-00000550: 6972 6563 746f 7279 5c6e 222c 0d0a 2020  irectory\n",..  
-00000560: 2020 2277 6f72 6b20 3d20 5061 7468 2872    "work = Path(r
-00000570: 5c22 433a 2f73 2f64 6174 612f 6d6f 6e74  \"C:/s/data/mont
-00000580: 6167 655f 315c 2229 220d 0a20 2020 5d0d  age_1\")"..   ].
-00000590: 0a20 207d 2c0d 0a20 207b 0d0a 2020 2022  .  },..  {..   "
-000005a0: 6365 6c6c 5f74 7970 6522 3a20 226d 6172  cell_type": "mar
-000005b0: 6b64 6f77 6e22 2c0d 0a20 2020 226d 6574  kdown",..   "met
-000005c0: 6164 6174 6122 3a20 7b7d 2c0d 0a20 2020  adata": {},..   
-000005d0: 2273 6f75 7263 6522 3a20 5b0d 0a20 2020  "source": [..   
-000005e0: 2022 2323 2053 6574 7469 6e67 2075 7020   "## Setting up 
-000005f0: 7468 6520 6d6f 6e74 6167 655c 6e22 2c0d  the montage\n",.
-00000600: 0a20 2020 2022 5c6e 222c 0d0a 2020 2020  .    "\n",..    
-00000610: 224c 6f61 6420 7468 6520 606d 6f6e 7461  "Load the `monta
-00000620: 6765 2e79 616d 6c60 2066 696c 6520 616e  ge.yaml` file an
-00000630: 6420 7468 6520 6173 736f 6369 6174 6564  d the associated
-00000640: 2069 6d61 6765 732e 220d 0a20 2020 5d0d   images."..   ].
-00000650: 0a20 207d 2c0d 0a20 207b 0d0a 2020 2022  .  },..  {..   "
-00000660: 6365 6c6c 5f74 7970 6522 3a20 2263 6f64  cell_type": "cod
-00000670: 6522 2c0d 0a20 2020 2265 7865 6375 7469  e",..   "executi
-00000680: 6f6e 5f63 6f75 6e74 223a 206e 756c 6c2c  on_count": null,
-00000690: 0d0a 2020 2022 6d65 7461 6461 7461 223a  ..   "metadata":
-000006a0: 207b 7d2c 0d0a 2020 2022 6f75 7470 7574   {},..   "output
-000006b0: 7322 3a20 5b5d 2c0d 0a20 2020 2273 6f75  s": [],..   "sou
-000006c0: 7263 6522 3a20 5b0d 0a20 2020 2022 6d20  rce": [..    "m 
-000006d0: 3d20 496e 7374 616d 6174 6963 4d6f 6e74  = InstamaticMont
-000006e0: 6167 652e 6672 6f6d 5f6d 6f6e 7461 6765  age.from_montage
-000006f0: 5f79 616d 6c28 776f 726b 202f 2027 6d6f  _yaml(work / 'mo
-00000700: 6e74 6167 652e 7961 6d6c 2729 5c6e 222c  ntage.yaml')\n",
-00000710: 0d0a 2020 2020 226d 2e67 7269 6473 7065  ..    "m.gridspe
-00000720: 6322 0d0a 2020 205d 0d0a 2020 7d2c 0d0a  c"..   ]..  },..
-00000730: 2020 7b0d 0a20 2020 2263 656c 6c5f 7479    {..   "cell_ty
-00000740: 7065 223a 2022 6d61 726b 646f 776e 222c  pe": "markdown",
-00000750: 0d0a 2020 2022 6d65 7461 6461 7461 223a  ..   "metadata":
-00000760: 207b 7d2c 0d0a 2020 2022 736f 7572 6365   {},..   "source
-00000770: 223a 205b 0d0a 2020 2020 2246 6972 7374  ": [..    "First
-00000780: 2c20 7765 2063 616e 2063 6865 636b 2077  , we can check w
-00000790: 6861 7420 7468 6520 6461 7461 2061 6374  hat the data act
-000007a0: 7561 6c6c 7920 6c6f 6f6b 206c 696b 652e  ually look like.
-000007b0: 2054 6f20 646f 2073 6f2c 2077 6520 6361   To do so, we ca
-000007c0: 6e20 7369 6d70 6c79 2060 7374 6974 6368  n simply `stitch
-000007d0: 6020 616e 6420 6070 6c6f 7460 2074 6865  ` and `plot` the
-000007e0: 2064 6174 6120 7573 696e 6720 6120 6062   data using a `b
-000007f0: 696e 6e69 6e67 3d34 6020 746f 2063 6f6e  inning=4` to con
-00000800: 7365 7276 6520 6120 6269 7420 6f66 206d  serve a bit of m
-00000810: 656d 6f72 792e 2054 6869 7320 6e61 6976  emory. This naiv
-00000820: 656c 7920 706c 6f74 7320 7468 6520 6461  ely plots the da
-00000830: 7461 2061 7420 7468 6520 6578 7065 6374  ta at the expect
-00000840: 6564 2070 6f73 6974 696f 6e73 2e20 416c  ed positions. Al
-00000850: 7468 6f75 6768 2074 6865 2073 7469 7463  though the stitc
-00000860: 6869 6e67 2069 7320 6e6f 7420 7468 6174  hing is not that
-00000870: 2067 7265 6174 2c20 6974 2773 2065 6e6f   great, it's eno
-00000880: 7567 6820 746f 2067 6574 2061 2066 6565  ugh to get a fee
-00000890: 6c69 6e67 2066 6f72 2074 6865 2064 6174  ling for the dat
-000008a0: 612e 220d 0a20 2020 5d0d 0a20 207d 2c0d  a."..   ]..  },.
-000008b0: 0a20 207b 0d0a 2020 2022 6365 6c6c 5f74  .  {..   "cell_t
-000008c0: 7970 6522 3a20 2263 6f64 6522 2c0d 0a20  ype": "code",.. 
-000008d0: 2020 2265 7865 6375 7469 6f6e 5f63 6f75    "execution_cou
-000008e0: 6e74 223a 206e 756c 6c2c 0d0a 2020 2022  nt": null,..   "
-000008f0: 6d65 7461 6461 7461 223a 207b 7d2c 0d0a  metadata": {},..
-00000900: 2020 2022 6f75 7470 7574 7322 3a20 5b5d     "outputs": []
-00000910: 2c0d 0a20 2020 2273 6f75 7263 6522 3a20  ,..   "source": 
-00000920: 5b0d 0a20 2020 2022 6d2e 6361 6c63 756c  [..    "m.calcul
-00000930: 6174 655f 6d6f 6e74 6167 655f 636f 6f72  ate_montage_coor
-00000940: 6473 2829 5c6e 222c 0d0a 2020 2020 226d  ds()\n",..    "m
-00000950: 2e73 7469 7463 6828 6269 6e6e 696e 673d  .stitch(binning=
-00000960: 3429 5c6e 222c 0d0a 2020 2020 226d 2e70  4)\n",..    "m.p
-00000970: 6c6f 7428 2922 0d0a 2020 205d 0d0a 2020  lot()"..   ]..  
-00000980: 7d2c 0d0a 2020 7b0d 0a20 2020 2263 656c  },..  {..   "cel
-00000990: 6c5f 7479 7065 223a 2022 6d61 726b 646f  l_type": "markdo
-000009a0: 776e 222c 0d0a 2020 2022 6d65 7461 6461  wn",..   "metada
-000009b0: 7461 223a 207b 7d2c 0d0a 2020 2022 736f  ta": {},..   "so
-000009c0: 7572 6365 223a 205b 0d0a 2020 2020 2254  urce": [..    "T
-000009d0: 6f20 6765 7420 6265 7474 6572 2073 7469  o get better sti
-000009e0: 7463 6869 6e67 2c20 7765 206e 6565 6420  tching, we need 
-000009f0: 746f 3a5c 6e22 2c0d 0a20 2020 2022 5c6e  to:\n",..    "\n
-00000a00: 222c 0d0a 2020 2020 2220 312e 2042 6574  ",..    " 1. Bet
-00000a10: 7465 7220 6573 7469 6d61 7465 2074 6865  ter estimate the
-00000a20: 2064 6966 6665 7265 6e63 6520 7665 6374   difference vect
-00000a30: 6f72 7320 6265 7477 6565 6e20 6561 6368  ors between each
-00000a40: 2074 696c 6520 7573 696e 6720 6372 6f73   tile using cros
-00000a50: 7320 636f 7272 656c 6174 696f 6e5c 6e22  s correlation\n"
-00000a60: 2c0d 0a20 2020 2022 2032 2e20 4f70 7469  ,..    " 2. Opti
-00000a70: 6d69 7a65 2074 6865 2063 6f6f 7264 696e  mize the coordin
-00000a80: 6174 6573 206f 6620 7468 6520 6469 6666  ates of the diff
-00000a90: 6572 656e 6365 2076 6563 746f 7273 2075  erence vectors u
-00000aa0: 7369 6e67 206c 6561 7374 2d73 7175 6172  sing least-squar
-00000ab0: 6573 206d 696e 696d 697a 6174 696f 6e5c  es minimization\
-00000ac0: 6e22 2c0d 0a20 2020 2022 5c6e 222c 0d0a  n",..    "\n",..
-00000ad0: 2020 2020 2254 6869 7320 6170 7072 6f61      "This approa
-00000ae0: 6368 2069 7320 6261 7365 6420 6f6e 202a  ch is based on *
-00000af0: 476c 6f62 616c 6c79 206f 7074 696d 616c  Globally optimal
-00000b00: 2073 7469 7463 6869 6e67 206f 6620 7469   stitching of ti
-00000b10: 6c65 6420 3344 206d 6963 726f 7363 6f70  led 3D microscop
-00000b20: 6963 2069 6d61 6765 2061 6371 7569 7369  ic image acquisi
-00000b30: 7469 6f6e 732a 2062 7920 5072 6569 6269  tions* by Preibi
-00000b40: 7368 2065 7420 616c 2e2c 2042 696f 696e  sh et al., Bioin
-00000b50: 666f 726d 6174 6963 7320 3235 2028 3230  formatics 25 (20
-00000b60: 3039 292c 2031 3436 33e2 8093 3134 3635  09), 1463...1465
-00000b70: 2028 6874 7470 733a 2f2f 646f 692e 6f72   (https://doi.or
-00000b80: 672f 3130 2e31 3039 332f 6269 6f69 6e66  g/10.1093/bioinf
-00000b90: 6f72 6d61 7469 6373 2f62 7470 3138 3429  ormatics/btp184)
-00000ba0: 2e5c 6e22 2c0d 0a20 2020 2022 5c6e 222c  .\n",..    "\n",
-00000bb0: 0d0a 2020 2020 2253 6f6d 6520 6d65 7472  ..    "Some metr
-00000bc0: 6963 732c 2073 7563 6820 6173 2074 6865  ics, such as the
-00000bd0: 206f 6274 6169 6e65 6420 7368 6966 7473   obtained shifts
-00000be0: 2061 6e64 2046 4654 2073 636f 7265 7320   and FFT scores 
-00000bf0: 6172 6520 706c 6f74 7465 6420 746f 2065  are plotted to e
-00000c00: 7661 6c75 6174 6520 7468 6520 7374 6974  valuate the stit
-00000c10: 6368 696e 672e 220d 0a20 2020 5d0d 0a20  ching."..   ].. 
-00000c20: 207d 2c0d 0a20 207b 0d0a 2020 2022 6365   },..  {..   "ce
-00000c30: 6c6c 5f74 7970 6522 3a20 2263 6f64 6522  ll_type": "code"
-00000c40: 2c0d 0a20 2020 2265 7865 6375 7469 6f6e  ,..   "execution
-00000c50: 5f63 6f75 6e74 223a 206e 756c 6c2c 0d0a  _count": null,..
-00000c60: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-00000c70: 7d2c 0d0a 2020 2022 6f75 7470 7574 7322  },..   "outputs"
-00000c80: 3a20 5b5d 2c0d 0a20 2020 2273 6f75 7263  : [],..   "sourc
-00000c90: 6522 3a20 5b0d 0a20 2020 2022 2320 5573  e": [..    "# Us
-00000ca0: 6520 6372 6f73 7320 636f 7272 656c 6174  e cross correlat
-00000cb0: 696f 6e20 746f 2067 6574 2064 6966 6665  ion to get diffe
-00000cc0: 7265 6e63 6520 7665 6374 6f72 735c 6e22  rence vectors\n"
-00000cd0: 2c0d 0a20 2020 2022 6d2e 6361 6c63 756c  ,..    "m.calcul
-00000ce0: 6174 655f 6469 6666 6572 656e 6365 5f76  ate_difference_v
-00000cf0: 6563 746f 7273 2874 6872 6573 686f 6c64  ectors(threshold
-00000d00: 3d27 6175 746f 272c 205c 6e22 2c0d 0a20  ='auto', \n",.. 
-00000d10: 2020 2022 2020 2020 2020 2020 2020 2020     "            
-00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d30: 2020 206d 6574 686f 643d 2773 6b69 6d61     method='skima
-00000d40: 6765 272c 205c 6e22 2c0d 0a20 2020 2022  ge', \n",..    "
-00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d60: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00000d70: 6c6f 743d 4661 6c73 6529 5c6e 222c 0d0a  lot=False)\n",..
-00000d80: 2020 2020 225c 6e22 2c0d 0a20 2020 2022      "\n",..    "
-00000d90: 2320 706c 6f74 2074 6865 2066 6674 5f73  # plot the fft_s
-00000da0: 636f 7265 735c 6e22 2c0d 0a20 2020 2022  cores\n",..    "
-00000db0: 6d2e 706c 6f74 5f66 6674 5f73 636f 7265  m.plot_fft_score
-00000dc0: 7328 295c 6e22 2c0d 0a20 2020 2022 5c6e  s()\n",..    "\n
-00000dd0: 222c 0d0a 2020 2020 2223 2070 6c6f 7420  ",..    "# plot 
-00000de0: 7468 6520 7069 7865 6c20 7368 6966 7473  the pixel shifts
-00000df0: 5c6e 222c 0d0a 2020 2020 226d 2e70 6c6f  \n",..    "m.plo
-00000e00: 745f 7368 6966 7473 2829 5c6e 222c 0d0a  t_shifts()\n",..
-00000e10: 2020 2020 225c 6e22 2c0d 0a20 2020 2022      "\n",..    "
-00000e20: 2320 6765 7420 636f 6f72 6473 206f 7074  # get coords opt
-00000e30: 696d 697a 6564 2075 7369 6e67 2063 726f  imized using cro
-00000e40: 7373 2063 6f72 7265 6c61 7469 6f6e 5c6e  ss correlation\n
-00000e50: 222c 0d0a 2020 2020 226d 2e6f 7074 696d  ",..    "m.optim
-00000e60: 697a 655f 6d6f 6e74 6167 655f 636f 6f72  ize_montage_coor
-00000e70: 6473 2870 6c6f 743d 5472 7565 295c 6e22  ds(plot=True)\n"
-00000e80: 2c0d 0a20 2020 2022 5c6e 222c 0d0a 2020  ,..    "\n",..  
-00000e90: 2020 2223 2073 7469 7463 6820 696d 6167    "# stitch imag
-00000ea0: 652c 2075 7365 2062 696e 6e69 6e67 2034  e, use binning 4
-00000eb0: 2066 6f72 2073 7065 6564 2d75 7020 616e   for speed-up an
-00000ec0: 6420 6d65 6d6f 7279 2063 6f6e 7365 7276  d memory conserv
-00000ed0: 6174 696f 6e5c 6e22 2c0d 0a20 2020 2022  ation\n",..    "
-00000ee0: 6d2e 7374 6974 6368 2862 696e 6e69 6e67  m.stitch(binning
-00000ef0: 3d34 295c 6e22 2c0d 0a20 2020 2022 5c6e  =4)\n",..    "\n
-00000f00: 222c 0d0a 2020 2020 2223 2070 6c6f 7420  ",..    "# plot 
-00000f10: 7468 6520 7374 6974 6368 6564 2069 6d61  the stitched ima
-00000f20: 6765 5c6e 222c 0d0a 2020 2020 226d 2e70  ge\n",..    "m.p
-00000f30: 6c6f 7428 2922 0d0a 2020 205d 0d0a 2020  lot()"..   ]..  
-00000f40: 7d2c 0d0a 2020 7b0d 0a20 2020 2263 656c  },..  {..   "cel
-00000f50: 6c5f 7479 7065 223a 2022 6d61 726b 646f  l_type": "markdo
-00000f60: 776e 222c 0d0a 2020 2022 6d65 7461 6461  wn",..   "metada
-00000f70: 7461 223a 207b 7d2c 0d0a 2020 2022 736f  ta": {},..   "so
-00000f80: 7572 6365 223a 205b 0d0a 2020 2020 2257  urce": [..    "W
-00000f90: 6520 6361 6e20 7361 7665 2074 6865 2073  e can save the s
-00000fa0: 7469 7463 6865 6420 696d 6167 653a 220d  titched image:".
-00000fb0: 0a20 2020 5d0d 0a20 207d 2c0d 0a20 207b  .   ]..  },..  {
-00000fc0: 0d0a 2020 2022 6365 6c6c 5f74 7970 6522  ..   "cell_type"
-00000fd0: 3a20 2263 6f64 6522 2c0d 0a20 2020 2265  : "code",..   "e
-00000fe0: 7865 6375 7469 6f6e 5f63 6f75 6e74 223a  xecution_count":
-00000ff0: 206e 756c 6c2c 0d0a 2020 2022 6d65 7461   null,..   "meta
-00001000: 6461 7461 223a 207b 7d2c 0d0a 2020 2022  data": {},..   "
-00001010: 6f75 7470 7574 7322 3a20 5b5d 2c0d 0a20  outputs": [],.. 
-00001020: 2020 2273 6f75 7263 6522 3a20 5b0d 0a20    "source": [.. 
-00001030: 2020 2022 6d2e 6578 706f 7274 2877 6f72     "m.export(wor
-00001040: 6b20 2f20 5c22 7374 6974 6368 6564 2e74  k / \"stitched.t
-00001050: 6966 665c 2229 220d 0a20 2020 5d0d 0a20  iff\")"..   ].. 
-00001060: 207d 2c0d 0a20 207b 0d0a 2020 2022 6365   },..  {..   "ce
-00001070: 6c6c 5f74 7970 6522 3a20 226d 6172 6b64  ll_type": "markd
-00001080: 6f77 6e22 2c0d 0a20 2020 226d 6574 6164  own",..   "metad
-00001090: 6174 6122 3a20 7b7d 2c0d 0a20 2020 2273  ata": {},..   "s
-000010a0: 6f75 7263 6522 3a20 5b0d 0a20 2020 2022  ource": [..    "
-000010b0: 5768 656e 2074 6865 2069 6d61 6765 2068  When the image h
-000010c0: 6173 2062 6565 6e20 7374 6974 6368 6564  as been stitched
-000010d0: 2028 7769 7468 206f 7220 7769 7468 6f75   (with or withou
-000010e0: 7420 6f70 7469 6d69 7a61 7469 6f6e 292c  t optimization),
-000010f0: 2077 6520 6361 6e20 6c6f 6f6b 2066 6f72   we can look for
-00001100: 2074 6865 2070 6f73 6974 696f 6e73 206f   the positions o
-00001110: 6620 7468 6520 6772 6964 2073 7175 6172  f the grid squar
-00001120: 6573 2f73 7175 6972 636c 6573 2e20 546f  es/squircles. To
-00001130: 2064 6f20 736f 2c20 6361 6c6c 2074 6865   do so, call the
-00001140: 206d 6574 686f 6420 602e 6669 6e64 5f68   method `.find_h
-00001150: 6f6c 6573 602e 2054 6865 2067 7269 6420  oles`. The grid 
-00001160: 7371 7561 7265 7320 6172 6520 6964 656e  squares are iden
-00001170: 7469 6669 6564 2061 7320 6f62 6a65 6374  tified as object
-00001180: 7320 726f 7567 686c 7920 7369 7a65 6420  s roughly sized 
-00001190: 6064 6961 6d65 7465 7260 2077 6974 6820  `diameter` with 
-000011a0: 6120 746f 6c65 7261 6e63 6520 6f66 2031  a tolerance of 1
-000011b0: 3025 2e20 5468 6520 6d65 6469 616e 2061  0%. The median a
-000011c0: 7320 7765 6c6c 2061 7320 352f 3935 2070  s well as 5/95 p
-000011d0: 6572 6365 6e74 696c 6573 2061 7265 2070  ercentiles are p
-000011e0: 7269 6e74 6564 2074 6f20 6576 616c 7561  rinted to evalua
-000011f0: 7465 2074 6865 2068 6f6c 6520 7369 7a65  te the hole size
-00001200: 2064 6973 7472 6962 7574 696f 6e2e 220d   distribution.".
-00001210: 0a20 2020 5d0d 0a20 207d 2c0d 0a20 207b  .   ]..  },..  {
-00001220: 0d0a 2020 2022 6365 6c6c 5f74 7970 6522  ..   "cell_type"
-00001230: 3a20 2263 6f64 6522 2c0d 0a20 2020 2265  : "code",..   "e
-00001240: 7865 6375 7469 6f6e 5f63 6f75 6e74 223a  xecution_count":
-00001250: 206e 756c 6c2c 0d0a 2020 2022 6d65 7461   null,..   "meta
-00001260: 6461 7461 223a 207b 7d2c 0d0a 2020 2022  data": {},..   "
-00001270: 6f75 7470 7574 7322 3a20 5b5d 2c0d 0a20  outputs": [],.. 
-00001280: 2020 2273 6f75 7263 6522 3a20 5b0d 0a20    "source": [.. 
-00001290: 2020 2022 6469 616d 6574 6572 203d 2034     "diameter = 4
-000012a0: 355f 3030 3020 2023 206e 6d5c 6e22 2c0d  5_000  # nm\n",.
-000012b0: 0a20 2020 2022 7374 6167 6563 6f6f 7264  .    "stagecoord
-000012c0: 732c 2069 6d61 6765 636f 6f72 6473 203d  s, imagecoords =
-000012d0: 206d 2e66 696e 645f 686f 6c65 7328 706c   m.find_holes(pl
-000012e0: 6f74 3d54 7275 652c 2074 6f6c 6572 616e  ot=True, toleran
-000012f0: 6365 3d30 2e31 2922 0d0a 2020 205d 0d0a  ce=0.1)"..   ]..
-00001300: 2020 7d2c 0d0a 2020 7b0d 0a20 2020 2263    },..  {..   "c
-00001310: 656c 6c5f 7479 7065 223a 2022 6d61 726b  ell_type": "mark
-00001320: 646f 776e 222c 0d0a 2020 2022 6d65 7461  down",..   "meta
-00001330: 6461 7461 223a 207b 7d2c 0d0a 2020 2022  data": {},..   "
-00001340: 736f 7572 6365 223a 205b 0d0a 2020 2020  source": [..    
-00001350: 2249 7420 6973 2070 6f73 7369 626c 6520  "It is possible 
-00001360: 746f 206f 7074 696d 697a 6520 7468 6520  to optimize the 
-00001370: 7374 6167 6520 636f 6f72 6469 6e61 7465  stage coordinate
-00001380: 7320 666f 7220 6d6f 7265 2065 6666 6963  s for more effic
-00001390: 6965 6e74 206e 6176 6967 6174 696f 6e2e  ient navigation.
-000013a0: 2049 6e20 7468 6973 2065 7861 6d70 6c65   In this example
-000013b0: 2c20 7468 6520 746f 7461 6c20 7374 6167  , the total stag
-000013c0: 6520 6d6f 7665 6d65 6e74 2063 616e 2062  e movement can b
-000013d0: 6520 7265 6475 6365 6420 6279 2061 626f  e reduced by abo
-000013e0: 7574 2037 3525 2c20 7768 6963 6820 7769  ut 75%, which wi
-000013f0: 6c6c 2073 6176 6520 6120 6c6f 7420 6f66  ll save a lot of
-00001400: 2074 696d 652e 2054 6865 2066 756e 6374   time. The funct
-00001410: 696f 6e20 7573 6573 2074 6865 205f 7477  ion uses the _tw
-00001420: 6f2d 6f70 745f 2061 6c67 6f72 6974 686d  o-opt_ algorithm
-00001430: 2066 6f72 2066 696e 6469 6e67 2074 6865   for finding the
-00001440: 2073 686f 7274 6573 7420 7061 7468 3a20   shortest path: 
-00001450: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00001460: 6564 6961 2e6f 7267 2f77 696b 692f 322d  edia.org/wiki/2-
-00001470: 6f70 742e 220d 0a20 2020 5d0d 0a20 207d  opt."..   ]..  }
-00001480: 2c0d 0a20 207b 0d0a 2020 2022 6365 6c6c  ,..  {..   "cell
-00001490: 5f74 7970 6522 3a20 2263 6f64 6522 2c0d  _type": "code",.
-000014a0: 0a20 2020 2265 7865 6375 7469 6f6e 5f63  .   "execution_c
-000014b0: 6f75 6e74 223a 206e 756c 6c2c 0d0a 2020  ount": null,..  
-000014c0: 2022 6d65 7461 6461 7461 223a 207b 7d2c   "metadata": {},
-000014d0: 0d0a 2020 2022 6f75 7470 7574 7322 3a20  ..   "outputs": 
-000014e0: 5b5d 2c0d 0a20 2020 2273 6f75 7263 6522  [],..   "source"
-000014f0: 3a20 5b0d 0a20 2020 2022 6672 6f6d 2070  : [..    "from p
-00001500: 7973 6572 6961 6c65 6d2e 6e61 7669 6761  yserialem.naviga
-00001510: 7469 6f6e 2069 6d70 6f72 7420 736f 7274  tion import sort
-00001520: 5f6e 6176 5f69 7465 6d73 5f62 795f 7368  _nav_items_by_sh
-00001530: 6f72 7465 7374 5f70 6174 685c 6e22 2c0d  ortest_path\n",.
-00001540: 0a20 2020 2022 7374 6167 6563 6f6f 7264  .    "stagecoord
-00001550: 7320 3d20 736f 7274 5f6e 6176 5f69 7465  s = sort_nav_ite
-00001560: 6d73 5f62 795f 7368 6f72 7465 7374 5f70  ms_by_shortest_p
-00001570: 6174 6828 7374 6167 6563 6f6f 7264 732c  ath(stagecoords,
-00001580: 2070 6c6f 743d 5472 7565 293b 220d 0a20   plot=True);".. 
-00001590: 2020 5d0d 0a20 207d 2c0d 0a20 207b 0d0a    ]..  },..  {..
-000015a0: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
-000015b0: 226d 6172 6b64 6f77 6e22 2c0d 0a20 2020  "markdown",..   
-000015c0: 226d 6574 6164 6174 6122 3a20 7b7d 2c0d  "metadata": {},.
-000015d0: 0a20 2020 2273 6f75 7263 6522 3a20 5b0d  .   "source": [.
-000015e0: 0a20 2020 2022 5468 6520 6073 7461 6765  .    "The `stage
-000015f0: 636f 6f72 6473 6020 6361 6e20 6265 2075  coords` can be u
-00001600: 7365 6420 746f 2073 6574 2075 7020 616e  sed to set up an
-00001610: 2061 7574 6f6d 6174 6564 202a 2a61 6371   automated **acq
-00001620: 7569 7265 2061 7420 6974 656d 732a 2a2e  uire at items**.
-00001630: 2054 6869 7320 6973 2075 7365 6675 6c20   This is useful 
-00001640: 746f 2074 616b 6520 6d65 6469 756d 206d  to take medium m
-00001650: 6167 6e69 6669 6361 7469 6f6e 2069 6d61  agnification ima
-00001660: 6765 7320 6672 6f6d 2074 6865 2072 6567  ges from the reg
-00001670: 696f 6e73 206f 6620 696e 7465 7265 7374  ions of interest
-00001680: 2c20 696e 206f 7572 2063 6173 652c 2074  , in our case, t
-00001690: 6865 2067 7269 6420 7371 7561 7265 732e  he grid squares.
-000016a0: 2046 6972 7374 2c20 696e 6974 6961 6c69   First, initiali
-000016b0: 7a65 2061 2063 6f6e 6e65 6374 696f 6e20  ze a connection 
-000016c0: 746f 2074 6865 206d 6963 726f 7363 6f70  to the microscop
-000016d0: 652e 220d 0a20 2020 5d0d 0a20 207d 2c0d  e."..   ]..  },.
-000016e0: 0a20 207b 0d0a 2020 2022 6365 6c6c 5f74  .  {..   "cell_t
-000016f0: 7970 6522 3a20 2263 6f64 6522 2c0d 0a20  ype": "code",.. 
-00001700: 2020 2265 7865 6375 7469 6f6e 5f63 6f75    "execution_cou
-00001710: 6e74 223a 206e 756c 6c2c 0d0a 2020 2022  nt": null,..   "
-00001720: 6d65 7461 6461 7461 223a 207b 7d2c 0d0a  metadata": {},..
-00001730: 2020 2022 6f75 7470 7574 7322 3a20 5b5d     "outputs": []
-00001740: 2c0d 0a20 2020 2273 6f75 7263 6522 3a20  ,..   "source": 
-00001750: 5b0d 0a20 2020 2022 6672 6f6d 2069 6e73  [..    "from ins
-00001760: 7461 6d61 7469 6320 696d 706f 7274 2054  tamatic import T
-00001770: 454d 436f 6e74 726f 6c6c 6572 5c6e 222c  EMController\n",
-00001780: 0d0a 2020 2020 2263 7472 6c20 3d20 5445  ..    "ctrl = TE
-00001790: 4d43 6f6e 7472 6f6c 6c65 722e 696e 6974  MController.init
-000017a0: 6961 6c69 7a65 2829 220d 0a20 2020 5d0d  ialize()"..   ].
-000017b0: 0a20 207d 2c0d 0a20 207b 0d0a 2020 2022  .  },..  {..   "
-000017c0: 6365 6c6c 5f74 7970 6522 3a20 226d 6172  cell_type": "mar
-000017d0: 6b64 6f77 6e22 2c0d 0a20 2020 226d 6574  kdown",..   "met
-000017e0: 6164 6174 6122 3a20 7b7d 2c0d 0a20 2020  adata": {},..   
-000017f0: 2273 6f75 7263 6522 3a20 5b0d 0a20 2020  "source": [..   
-00001800: 2022 4e65 7874 2c20 7765 2073 686f 756c   "Next, we shoul
-00001810: 6420 7365 7420 7570 2061 6e20 6163 7175  d set up an acqu
-00001820: 6973 6974 696f 6e20 6675 6e63 7469 6f6e  isition function
-00001830: 2066 6f72 2065 6163 6820 7374 6167 6520   for each stage 
-00001840: 706f 7369 7469 6f6e 2e20 5468 6973 2073  position. This s
-00001850: 686f 756c 643a 5c6e 222c 0d0a 2020 2020  hould:\n",..    
-00001860: 225c 6e22 2c0d 0a20 2020 2022 312e 2043  "\n",..    "1. C
-00001870: 656e 7465 7220 7468 6520 6772 6964 2073  enter the grid s
-00001880: 7175 6172 6520 6279 2061 6c69 676e 696e  quare by alignin
-00001890: 6720 6974 2077 6974 6820 6120 7265 6665  g it with a refe
-000018a0: 7265 6e63 6520 696d 6167 655c 6e22 2c0d  rence image\n",.
-000018b0: 0a20 2020 2022 322e 2054 616b 6520 616e  .    "2. Take an
-000018c0: 2069 6d61 6765 2061 7420 6869 6768 206d   image at high m
-000018d0: 6167 5c6e 222c 0d0a 2020 2020 2233 2e20  ag\n",..    "3. 
-000018e0: 5374 6f72 6520 7468 6520 696d 6167 6520  Store the image 
-000018f0: 616e 6420 7468 6520 636f 7272 6573 706f  and the correspo
-00001900: 6e64 696e 6720 7374 6167 6520 706f 7369  nding stage posi
-00001910: 7469 6f6e 2069 6e20 6120 6275 6666 6572  tion in a buffer
-00001920: 5c6e 222c 0d0a 2020 2020 225c 6e22 2c0d  \n",..    "\n",.
-00001930: 0a20 2020 2022 496e 2074 6869 7320 7072  .    "In this pr
-00001940: 6570 6172 6174 696f 6e20 7374 6570 2c20  eparation step, 
-00001950: 7765 206d 7563 6820 6669 7273 7420 6f62  we much first ob
-00001960: 7461 696e 2061 2072 6566 6572 656e 6365  tain a reference
-00001970: 2069 6d61 6765 2066 726f 6d20 6120 6772   image from a gr
-00001980: 6964 2073 7175 6172 652e 2054 6865 206d  id square. The m
-00001990: 6167 6e69 6669 6361 7469 6f6e 2073 686f  agnification sho
-000019a0: 756c 6420 6265 2073 6f20 7468 6174 2074  uld be so that t
-000019b0: 6865 2067 7269 6420 7371 7561 7265 2066  he grid square f
-000019c0: 6974 7320 696e 2074 6865 2076 6965 7720  its in the view 
-000019d0: 6f66 2074 6865 2069 6d61 6765 2e20 496e  of the image. In
-000019e0: 2074 6869 7320 6578 616d 706c 652c 2077   this example, w
-000019f0: 6520 7573 6520 6033 3030 7860 2069 6e20  e use `300x` in 
-00001a00: 606c 6f77 6d61 6760 2e22 0d0a 2020 205d  `lowmag`."..   ]
-00001a10: 0d0a 2020 7d2c 0d0a 2020 7b0d 0a20 2020  ..  },..  {..   
-00001a20: 2263 656c 6c5f 7479 7065 223a 2022 636f  "cell_type": "co
-00001a30: 6465 222c 0d0a 2020 2022 6578 6563 7574  de",..   "execut
-00001a40: 696f 6e5f 636f 756e 7422 3a20 6e75 6c6c  ion_count": null
-00001a50: 2c0d 0a20 2020 226d 6574 6164 6174 6122  ,..   "metadata"
-00001a60: 3a20 7b7d 2c0d 0a20 2020 226f 7574 7075  : {},..   "outpu
-00001a70: 7473 223a 205b 5d2c 0d0a 2020 2022 736f  ts": [],..   "so
-00001a80: 7572 6365 223a 205b 0d0a 2020 2020 2269  urce": [..    "i
-00001a90: 6d70 6f72 7420 6d72 6366 696c 655c 6e22  mport mrcfile\n"
-00001aa0: 2c0d 0a20 2020 2022 5c6e 222c 0d0a 2020  ,..    "\n",..  
-00001ab0: 2020 2223 2073 6574 206d 6963 726f 7363    "# set microsc
-00001ac0: 6f70 6520 636f 6e64 6974 696f 6e73 5c6e  ope conditions\n
-00001ad0: 222c 0d0a 2020 2020 2263 7472 6c2e 6d6f  ",..    "ctrl.mo
-00001ae0: 6465 2e73 6574 2827 6c6f 776d 6167 2729  de.set('lowmag')
-00001af0: 5c6e 222c 0d0a 2020 2020 2263 7472 6c2e  \n",..    "ctrl.
-00001b00: 6d61 676e 6966 6963 6174 696f 6e2e 7661  magnification.va
-00001b10: 6c75 6520 3d20 3330 305c 6e22 2c0d 0a20  lue = 300\n",.. 
-00001b20: 2020 2022 6269 6e73 697a 6520 3d20 345c     "binsize = 4\
-00001b30: 6e22 2c0d 0a20 2020 2022 5c6e 222c 0d0a  n",..    "\n",..
-00001b40: 2020 2020 2223 2072 6566 6572 656e 6365      "# reference
-00001b50: 2069 6d61 6765 206f 6620 6120 6365 6e74   image of a cent
-00001b60: 6572 6564 2067 7269 6420 7371 7561 7265  ered grid square
-00001b70: 5c6e 222c 0d0a 2020 2020 2272 6566 5f69  \n",..    "ref_i
-00001b80: 6d67 203d 2063 7472 6c2e 6765 745f 7261  mg = ctrl.get_ra
-00001b90: 775f 696d 6167 6528 295c 6e22 2c0d 0a20  w_image()\n",.. 
-00001ba0: 2020 2022 5c6e 222c 0d0a 2020 2020 2266     "\n",..    "f
-00001bb0: 203d 206d 7263 6669 6c65 2e6e 6577 2877   = mrcfile.new(w
-00001bc0: 6f72 6b20 2f20 2774 656d 706c 6174 652e  ork / 'template.
-00001bd0: 6d72 6327 2c20 6461 7461 3d72 6566 5f69  mrc', data=ref_i
-00001be0: 6d67 2e61 7374 7970 6528 6e70 2e69 6e74  mg.astype(np.int
-00001bf0: 3136 292c 206f 7665 7277 7269 7465 3d54  16), overwrite=T
-00001c00: 7275 6529 5c6e 222c 0d0a 2020 2020 2266  rue)\n",..    "f
-00001c10: 2e63 6c6f 7365 2829 220d 0a20 2020 5d0d  .close()"..   ].
-00001c20: 0a20 207d 2c0d 0a20 207b 0d0a 2020 2022  .  },..  {..   "
-00001c30: 6365 6c6c 5f74 7970 6522 3a20 226d 6172  cell_type": "mar
-00001c40: 6b64 6f77 6e22 2c0d 0a20 2020 226d 6574  kdown",..   "met
-00001c50: 6164 6174 6122 3a20 7b7d 2c0d 0a20 2020  adata": {},..   
-00001c60: 2273 6f75 7263 6522 3a20 5b0d 0a20 2020  "source": [..   
-00001c70: 2022 5468 656e 2c20 7765 2063 616e 2064   "Then, we can d
-00001c80: 6566 696e 6520 6f75 7220 6163 7175 6973  efine our acquis
-00001c90: 6974 696f 6e20 6675 6e63 7469 6f6e 2e20  ition function. 
-00001ca0: 5765 2077 696c 6c20 616c 6967 6e20 7468  We will align th
-00001cb0: 6520 7374 6167 6520 746f 2074 6865 2072  e stage to the r
-00001cc0: 6566 6572 656e 6365 2069 6d61 6765 2075  eference image u
-00001cd0: 7369 6e67 2063 726f 7373 2063 6f72 7265  sing cross corre
-00001ce0: 6c61 7469 6f6e 2028 6063 7472 6c2e 616c  lation (`ctrl.al
-00001cf0: 6967 6e5f 746f 6029 2c20 616e 6420 7468  ign_to`), and th
-00001d00: 656e 2074 616b 656e 2061 6e20 696d 6167  en taken an imag
-00001d10: 6520 6f66 2074 6865 2063 656e 7465 7265  e of the centere
-00001d20: 6420 6772 6964 2073 7175 6172 652e 2041  d grid square. A
-00001d30: 6c74 686f 7567 6820 7468 6973 2073 7465  lthough this ste
-00001d40: 7020 6973 206f 7074 696f 6e61 6c2c 2069  p is optional, i
-00001d50: 7420 6d61 6b65 7320 7375 7265 2074 6861  t makes sure tha
-00001d60: 7420 7468 6520 6772 6964 2073 7175 6172  t the grid squar
-00001d70: 6520 6973 2063 656e 7465 7265 642e 2054  e is centered. T
-00001d80: 6869 7320 6865 6c70 7320 7768 656e 206c  his helps when l
-00001d90: 6f6f 6b69 6e67 2066 6f72 2070 6172 7469  ooking for parti
-00001da0: 636c 6573 2c20 616e 6420 7265 6475 6365  cles, and reduce
-00001db0: 7320 6572 726f 7273 2072 656c 6174 6564  s errors related
-00001dc0: 2074 6f20 7374 6167 6520 7472 616e 736c   to stage transl
-00001dd0: 6174 696f 6e20 616e 6420 6361 6c69 6272  ation and calibr
-00001de0: 6174 696f 6e2e 2057 6520 616c 736f 2061  ation. We also a
-00001df0: 6371 7569 7265 2061 6e20 696d 6167 6520  cquire an image 
-00001e00: 616e 6420 7374 6f72 6520 7468 6520 6e65  and store the ne
-00001e10: 7720 7374 6167 6520 706f 7369 7469 6f6e  w stage position
-00001e20: 2074 6f20 6120 6275 6666 6572 2e22 0d0a   to a buffer."..
-00001e30: 2020 205d 0d0a 2020 7d2c 0d0a 2020 7b0d     ]..  },..  {.
-00001e40: 0a20 2020 2263 656c 6c5f 7479 7065 223a  .   "cell_type":
-00001e50: 2022 636f 6465 222c 0d0a 2020 2022 6578   "code",..   "ex
-00001e60: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
-00001e70: 6e75 6c6c 2c0d 0a20 2020 226d 6574 6164  null,..   "metad
-00001e80: 6174 6122 3a20 7b7d 2c0d 0a20 2020 226f  ata": {},..   "o
-00001e90: 7574 7075 7473 223a 205b 5d2c 0d0a 2020  utputs": [],..  
-00001ea0: 2022 736f 7572 6365 223a 205b 0d0a 2020   "source": [..  
-00001eb0: 2020 2262 7566 6665 7220 3d20 5b5d 5c6e    "buffer = []\n
-00001ec0: 222c 0d0a 2020 2020 2273 7461 6765 706f  ",..    "stagepo
-00001ed0: 7320 3d20 5b5d 5c6e 222c 0d0a 2020 2020  s = []\n",..    
-00001ee0: 225c 6e22 2c0d 0a20 2020 2022 5c6e 222c  "\n",..    "\n",
-00001ef0: 0d0a 2020 2020 2264 6566 2061 6371 7569  ..    "def acqui
-00001f00: 7265 5f66 756e 6328 6374 726c 293a 5c6e  re_func(ctrl):\n
-00001f10: 222c 0d0a 2020 2020 2220 2020 2023 2041  ",..    "    # A
-00001f20: 6c69 676e 2074 6f20 7465 6d70 6c61 7465  lign to template
-00001f30: 5c6e 222c 0d0a 2020 2020 2223 2020 2020  \n",..    "#    
-00001f40: 2063 7472 6c2e 616c 6967 6e5f 746f 2872   ctrl.align_to(r
-00001f50: 6566 5f69 6d67 2c20 6170 706c 793d 5472  ef_img, apply=Tr
-00001f60: 7565 295c 6e22 2c0d 0a20 2020 2022 2020  ue)\n",..    "  
-00001f70: 2020 5c6e 222c 0d0a 2020 2020 2220 2020    \n",..    "   
-00001f80: 2023 206f 6274 6169 6e20 696d 6167 655c   # obtain image\
-00001f90: 6e22 2c0d 0a20 2020 2022 2020 2020 696d  n",..    "    im
-00001fa0: 672c 2068 203d 2063 7472 6c2e 6765 745f  g, h = ctrl.get_
-00001fb0: 696d 6167 6528 6269 6e73 697a 653d 6269  image(binsize=bi
-00001fc0: 6e73 697a 6529 2020 5c6e 222c 0d0a 2020  nsize)  \n",..  
-00001fd0: 2020 2220 2020 2062 7566 6665 722e 6170    "    buffer.ap
-00001fe0: 7065 6e64 2869 6d67 295c 6e22 2c0d 0a20  pend(img)\n",.. 
-00001ff0: 2020 2022 2020 2020 5c6e 222c 0d0a 2020     "    \n",..  
-00002000: 2020 2220 2020 2023 2073 746f 7265 2073    "    # store s
-00002010: 7461 6765 2070 6f73 6974 696f 6e20 616e  tage position an
-00002020: 6420 696d 6167 6520 736f 6d65 7768 6572  d image somewher
-00002030: 655c 6e22 2c0d 0a20 2020 2022 2020 2020  e\n",..    "    
-00002040: 706f 7320 3d20 6374 726c 2e73 7461 6765  pos = ctrl.stage
-00002050: 2e67 6574 2829 5c6e 222c 0d0a 2020 2020  .get()\n",..    
-00002060: 2220 2020 2073 7461 6765 706f 732e 6170  "    stagepos.ap
-00002070: 7065 6e64 2870 6f73 2922 0d0a 2020 205d  pend(pos)"..   ]
-00002080: 0d0a 2020 7d2c 0d0a 2020 7b0d 0a20 2020  ..  },..  {..   
-00002090: 2263 656c 6c5f 7479 7065 223a 2022 6d61  "cell_type": "ma
-000020a0: 726b 646f 776e 222c 0d0a 2020 2022 6d65  rkdown",..   "me
-000020b0: 7461 6461 7461 223a 207b 7d2c 0d0a 2020  tadata": {},..  
-000020c0: 2022 736f 7572 6365 223a 205b 0d0a 2020   "source": [..  
-000020d0: 2020 2257 6865 6e20 7468 6520 6675 6e63    "When the func
-000020e0: 7469 6f6e 2069 7320 6465 6669 6e65 642c  tion is defined,
-000020f0: 2077 6520 6361 6e20 7061 7373 2069 7420   we can pass it 
-00002100: 616e 6420 7468 6520 6c69 7374 206f 6620  and the list of 
-00002110: 6772 6964 2073 7175 6172 6520 7374 6167  grid square stag
-00002120: 6520 636f 6f72 6469 6e61 7465 7320 746f  e coordinates to
-00002130: 2074 6865 2066 756e 6374 696f 6e20 6063   the function `c
-00002140: 7472 6c2e 6163 7175 6972 655f 6174 5f69  trl.acquire_at_i
-00002150: 7465 6d73 602c 2077 6869 6368 2077 696c  tems`, which wil
-00002160: 6c20 6175 746f 6d61 7465 2074 6865 2066  l automate the f
-00002170: 756e 6374 696f 6e20 6174 2065 6163 6820  unction at each 
-00002180: 7374 6167 6520 706f 7369 7469 6f6e 2e22  stage position."
-00002190: 0d0a 2020 205d 0d0a 2020 7d2c 0d0a 2020  ..   ]..  },..  
-000021a0: 7b0d 0a20 2020 2263 656c 6c5f 7479 7065  {..   "cell_type
-000021b0: 223a 2022 636f 6465 222c 0d0a 2020 2022  ": "code",..   "
-000021c0: 6578 6563 7574 696f 6e5f 636f 756e 7422  execution_count"
-000021d0: 3a20 6e75 6c6c 2c0d 0a20 2020 226d 6574  : null,..   "met
-000021e0: 6164 6174 6122 3a20 7b7d 2c0d 0a20 2020  adata": {},..   
-000021f0: 226f 7574 7075 7473 223a 205b 5d2c 0d0a  "outputs": [],..
-00002200: 2020 2022 736f 7572 6365 223a 205b 0d0a     "source": [..
-00002210: 2020 2020 2273 656c 203d 2073 7461 6765      "sel = stage
-00002220: 636f 6f72 6473 5b30 3a31 305d 2020 2320  coords[0:10]  # 
-00002230: 4163 7175 6972 6520 6174 2074 6865 2066  Acquire at the f
-00002240: 6972 7374 2031 3020 6974 656d 735c 6e22  irst 10 items\n"
-00002250: 2c0d 0a20 2020 2022 6374 726c 2e61 6371  ,..    "ctrl.acq
-00002260: 7569 7265 5f61 745f 6974 656d 7328 7365  uire_at_items(se
-00002270: 6c2c 2061 6371 7569 7265 3d61 6371 7569  l, acquire=acqui
-00002280: 7265 5f66 756e 6329 220d 0a20 2020 5d0d  re_func)"..   ].
-00002290: 0a20 207d 2c0d 0a20 207b 0d0a 2020 2022  .  },..  {..   "
-000022a0: 6365 6c6c 5f74 7970 6522 3a20 226d 6172  cell_type": "mar
-000022b0: 6b64 6f77 6e22 2c0d 0a20 2020 226d 6574  kdown",..   "met
-000022c0: 6164 6174 6122 3a20 7b7d 2c0d 0a20 2020  adata": {},..   
-000022d0: 2273 6f75 7263 6522 3a20 5b0d 0a20 2020  "source": [..   
-000022e0: 2022 4865 7265 2069 7320 6120 6d69 6e69   "Here is a mini
-000022f0: 6d61 6c20 6578 616d 706c 6520 6f66 2068  mal example of h
-00002300: 6f77 2074 6865 2061 6371 7569 7265 2066  ow the acquire f
-00002310: 756e 6374 696f 6e73 2063 616e 2062 6520  unctions can be 
-00002320: 6368 616e 6765 6420 746f 2063 6f6c 6c65  changed to colle
-00002330: 6374 2064 6174 6120 6361 6e20 6265 2073  ct data can be s
-00002340: 6176 6564 2074 6f20 6120 602e 6e61 7660  aved to a `.nav`
-00002350: 2066 696c 6520 7768 6963 6820 6361 6e20   file which can 
-00002360: 6265 2072 6561 6420 6279 2060 5365 7269  be read by `Seri
-00002370: 616c 454d 602e 205c 6e22 2c0d 0a20 2020  alEM`. \n",..   
-00002380: 2022 5c6e 222c 0d0a 2020 2020 2254 6869   "\n",..    "Thi
-00002390: 7320 6d61 6b65 7320 7573 6520 6f66 2074  s makes use of t
-000023a0: 6865 2061 6269 6c69 7479 2074 6f20 7061  he ability to pa
-000023b0: 7373 2061 2060 706f 7374 5f61 6371 7569  ss a `post_acqui
-000023c0: 7265 6020 6675 6e63 7469 6f6e 2074 6f20  re` function to 
-000023d0: 602e 6163 7175 6972 655f 6174 5f69 7465  `.acquire_at_ite
-000023e0: 6d73 602e 2054 6865 2070 6f73 7420 6163  ms`. The post ac
-000023f0: 7175 6973 6974 696f 6e20 6361 6e20 6265  quisition can be
-00002400: 2075 7365 6420 746f 2073 6176 6520 7468   used to save th
-00002410: 6520 696d 6167 6573 2061 7320 7765 6c6c  e images as well
-00002420: 2061 7320 7468 6520 7265 7175 6972 6564   as the required
-00002430: 206d 6574 6164 6174 6120 746f 2060 5365   metadata to `Se
-00002440: 7269 616c 454d 6020 666f 726d 6174 2c20  rialEM` format, 
-00002450: 6d61 6b69 6e67 2075 7365 206f 6620 7468  making use of th
-00002460: 6520 6069 6e73 7461 6d61 7469 632e 7365  e `instamatic.se
-00002470: 7269 616c 656d 6020 6d6f 6475 6c65 2e5c  rialem` module.\
-00002480: 6e22 2c0d 0a20 2020 2022 5c6e 222c 0d0a  n",..    "\n",..
-00002490: 2020 2020 2254 6865 2060 706f 7374 5f61      "The `post_a
-000024a0: 6371 7569 7265 6020 6675 6e63 7469 6f6e  cquire` function
-000024b0: 2073 6176 6573 2074 6865 2064 6174 6120   saves the data 
-000024c0: 746f 2060 2e6d 7263 6020 666f 726d 6174  to `.mrc` format
-000024d0: 2c20 616e 6420 7772 6974 6573 2061 6e20  , and writes an 
-000024e0: 696e 7075 7420 6669 6c65 2066 6f72 2053  input file for S
-000024f0: 6572 6961 6c45 4d3a 2060 696e 7374 616d  erialEM: `instam
-00002500: 6174 6963 2e6e 6176 602e 220d 0a20 2020  atic.nav`."..   
-00002510: 5d0d 0a20 207d 2c0d 0a20 207b 0d0a 2020  ]..  },..  {..  
-00002520: 2022 6365 6c6c 5f74 7970 6522 3a20 2263   "cell_type": "c
-00002530: 6f64 6522 2c0d 0a20 2020 2265 7865 6375  ode",..   "execu
-00002540: 7469 6f6e 5f63 6f75 6e74 223a 206e 756c  tion_count": nul
-00002550: 6c2c 0d0a 2020 2022 6d65 7461 6461 7461  l,..   "metadata
-00002560: 223a 207b 7d2c 0d0a 2020 2022 6f75 7470  ": {},..   "outp
-00002570: 7574 7322 3a20 5b5d 2c0d 0a20 2020 2273  uts": [],..   "s
-00002580: 6f75 7263 6522 3a20 5b0d 0a20 2020 2022  ource": [..    "
-00002590: 6672 6f6d 2070 7973 6572 6961 6c65 6d20  from pyserialem 
-000025a0: 696d 706f 7274 204d 6170 4974 656d 2c20  import MapItem, 
-000025b0: 7772 6974 655f 6e61 765f 6669 6c65 5c6e  write_nav_file\n
-000025c0: 222c 0d0a 2020 2020 2266 726f 6d20 696e  ",..    "from in
-000025d0: 7374 616d 6174 6963 2069 6d70 6f72 7420  stamatic import 
-000025e0: 636f 6e66 6967 5c6e 222c 0d0a 2020 2020  config\n",..    
-000025f0: 225c 6e22 2c0d 0a20 2020 2022 2320 7265  "\n",..    "# re
-00002600: 6665 7265 6e63 6520 696d 6167 6520 6f66  ference image of
-00002610: 2061 2063 656e 7465 7265 6420 6772 6964   a centered grid
-00002620: 2073 7175 6172 655c 6e22 2c0d 0a20 2020   square\n",..   
-00002630: 2022 7265 665f 696d 6720 3d20 6374 726c   "ref_img = ctrl
-00002640: 2e67 6574 5f72 6177 5f69 6d61 6765 2829  .get_raw_image()
-00002650: 5c6e 222c 0d0a 2020 2020 225c 6e22 2c0d  \n",..    "\n",.
-00002660: 0a20 2020 2022 6620 3d20 6d72 6366 696c  .    "f = mrcfil
-00002670: 652e 6e65 7728 776f 726b 202f 205c 2274  e.new(work / \"t
-00002680: 656d 706c 6174 652e 6d72 635c 222c 2064  emplate.mrc\", d
-00002690: 6174 613d 7265 665f 696d 672e 6173 7479  ata=ref_img.asty
-000026a0: 7065 286e 702e 696e 7431 3629 2c20 6f76  pe(np.int16), ov
-000026b0: 6572 7772 6974 653d 5472 7565 295c 6e22  erwrite=True)\n"
-000026c0: 2c0d 0a20 2020 2022 662e 636c 6f73 6528  ,..    "f.close(
-000026d0: 295c 6e22 2c0d 0a20 2020 2022 5c6e 222c  )\n",..    "\n",
-000026e0: 0d0a 2020 2020 2223 2065 6d70 7479 2062  ..    "# empty b
-000026f0: 7566 6665 7273 5c6e 222c 0d0a 2020 2020  uffers\n",..    
-00002700: 2262 7566 6665 7220 3d20 5b5d 5c6e 222c  "buffer = []\n",
-00002710: 0d0a 2020 2020 2273 7461 6765 706f 7320  ..    "stagepos 
-00002720: 3d20 5b5d 5c6e 222c 0d0a 2020 2020 225c  = []\n",..    "\
-00002730: 6e22 2c0d 0a20 2020 2022 2020 205c 6e22  n",..    "   \n"
-00002740: 2c0d 0a20 2020 2022 6465 6620 7772 6974  ,..    "def writ
-00002750: 655f 6d72 635f 7374 6163 6b28 666e 3a73  e_mrc_stack(fn:s
-00002760: 7472 2c20 6461 7461 3a20 6c69 7374 2c20  tr, data: list, 
-00002770: 6f76 6572 7772 6974 653a 2062 6f6f 6c3d  overwrite: bool=
-00002780: 5472 7565 2c20 6d6d 6170 3a62 6f6f 6c20  True, mmap:bool 
-00002790: 3d20 5472 7565 293a 5c6e 222c 0d0a 2020  = True):\n",..  
-000027a0: 2020 2220 2020 205c 225c 225c 2257 7269    "    \"\"\"Wri
-000027b0: 7465 2061 2073 7461 636b 206f 6620 696d  te a stack of im
-000027c0: 6167 6573 2074 6f20 616e 206d 7263 2066  ages to an mrc f
-000027d0: 696c 652e 5c22 5c22 5c22 5c6e 222c 0d0a  ile.\"\"\"\n",..
-000027e0: 2020 2020 2220 2020 2069 6620 6d6d 6170      "    if mmap
-000027f0: 3a5c 6e22 2c0d 0a20 2020 2022 2020 2020  :\n",..    "    
-00002800: 2020 2020 7368 6170 6520 3d20 286c 656e      shape = (len
-00002810: 2862 7566 6665 7229 2c20 2a62 7566 6665  (buffer), *buffe
-00002820: 725b 305d 2e73 6861 7065 295c 6e22 2c0d  r[0].shape)\n",.
-00002830: 0a20 2020 2022 2020 2020 2020 2020 7769  .    "        wi
-00002840: 7468 206d 7263 6669 6c65 2e6e 6577 5f6d  th mrcfile.new_m
-00002850: 6d61 7028 666e 2c20 7368 6170 653d 7368  map(fn, shape=sh
-00002860: 6170 652c 206f 7665 7277 7269 7465 3d54  ape, overwrite=T
-00002870: 7275 652c 206d 7263 5f6d 6f64 653d 3129  rue, mrc_mode=1)
-00002880: 2061 7320 663a 5c6e 222c 0d0a 2020 2020   as f:\n",..    
-00002890: 2220 2020 2020 2020 2020 2020 2066 6f72  "            for
-000028a0: 2069 2c20 696d 2069 6e20 656e 756d 6572   i, im in enumer
-000028b0: 6174 6528 6275 6666 6572 293a 5c6e 222c  ate(buffer):\n",
-000028c0: 0d0a 2020 2020 2220 2020 2020 2020 2020  ..    "         
-000028d0: 2020 2020 2020 2066 2e64 6174 615b 695d         f.data[i]
-000028e0: 203d 2069 6d5c 6e22 2c0d 0a20 2020 2022   = im\n",..    "
-000028f0: 2020 2020 656c 7365 3a5c 6e22 2c0d 0a20      else:\n",.. 
-00002900: 2020 2022 2020 2020 2020 2020 6461 7461     "        data
-00002910: 203d 206e 702e 6172 7261 7928 6461 7461   = np.array(data
-00002920: 295c 6e22 2c0d 0a20 2020 2022 2020 2020  )\n",..    "    
-00002930: 2020 2020 2320 6d72 6320 6361 6e20 6f6e      # mrc can on
-00002940: 6c79 2062 6520 7361 7665 6420 6173 2061  ly be saved as a
-00002950: 2031 362d 6269 7420 696e 7465 6765 725c   16-bit integer\
-00002960: 6e22 2c0d 0a20 2020 2022 2020 2020 2020  n",..    "      
-00002970: 2020 6461 7461 203d 2064 6174 612e 6173    data = data.as
-00002980: 7479 7065 286e 702e 696e 7431 3629 5c6e  type(np.int16)\n
-00002990: 222c 0d0a 2020 2020 2220 2020 2020 2020  ",..    "       
-000029a0: 2074 7279 3a5c 6e22 2c0d 0a20 2020 2022   try:\n",..    "
-000029b0: 2020 2020 2020 2020 2020 2020 6620 3d20              f = 
-000029c0: 6d72 6366 696c 652e 6e65 7728 666e 2c20  mrcfile.new(fn, 
-000029d0: 6461 7461 3d64 6174 612c 206f 7665 7277  data=data, overw
-000029e0: 7269 7465 3d6f 7665 7277 7269 7465 295c  rite=overwrite)\
-000029f0: 6e22 2c0d 0a20 2020 2022 2020 2020 2020  n",..    "      
-00002a00: 2020 6578 6365 7074 204f 5345 7272 6f72    except OSError
-00002a10: 3a5c 6e22 2c0d 0a20 2020 2022 2020 2020  :\n",..    "    
-00002a20: 2020 2020 2020 2020 662e 636c 6f73 6528          f.close(
-00002a30: 295c 6e22 2c0d 0a20 2020 2022 2020 2020  )\n",..    "    
-00002a40: 5c6e 222c 0d0a 2020 2020 225c 6e22 2c0d  \n",..    "\n",.
-00002a50: 0a20 2020 2022 6465 6620 706f 7374 5f61  .    "def post_a
-00002a60: 6371 7569 7265 2863 7472 6c29 3a5c 6e22  cquire(ctrl):\n"
-00002a70: 2c0d 0a20 2020 2022 2020 2020 666e 5f6e  ,..    "    fn_n
-00002a80: 6176 203d 2077 6f72 6b20 2f20 2769 6e73  av = work / 'ins
-00002a90: 7461 6d61 7469 632e 6e61 7627 5c6e 222c  tamatic.nav'\n",
-00002aa0: 0d0a 2020 2020 2220 2020 2066 6e5f 6d72  ..    "    fn_mr
-00002ab0: 6320 3d20 776f 726b 202f 2027 6d6d 6d2e  c = work / 'mmm.
-00002ac0: 6d72 6327 5c6e 222c 0d0a 2020 2020 2220  mrc'\n",..    " 
-00002ad0: 2020 205c 6e22 2c0d 0a20 2020 2022 2020     \n",..    "  
-00002ae0: 2020 7772 6974 655f 6d72 635f 7374 6163    write_mrc_stac
-00002af0: 6b28 666e 5f6d 7263 2c20 6275 6666 6572  k(fn_mrc, buffer
-00002b00: 295c 6e22 2c0d 0a20 2020 2022 2020 2020  )\n",..    "    
-00002b10: 5c6e 222c 0d0a 2020 2020 2220 2020 2069  \n",..    "    i
-00002b20: 7465 6d73 203d 205b 5d5c 6e22 2c0d 0a20  tems = []\n",.. 
-00002b30: 2020 2022 2020 2020 5c6e 222c 0d0a 2020     "    \n",..  
-00002b40: 2020 2220 2020 206d 6167 6e69 6669 6361    "    magnifica
-00002b50: 7469 6f6e 203d 2063 7472 6c2e 6d61 676e  tion = ctrl.magn
-00002b60: 6966 6963 6174 696f 6e2e 7661 6c75 655c  ification.value\
-00002b70: 6e22 2c0d 0a20 2020 2022 2020 2020 6d6f  n",..    "    mo
-00002b80: 6465 203d 2063 7472 6c2e 6d6f 6465 2e67  de = ctrl.mode.g
-00002b90: 6574 2829 5c6e 222c 0d0a 2020 2020 2220  et()\n",..    " 
-00002ba0: 2020 206d 6170 7363 616c 656d 6174 203d     mapscalemat =
-00002bb0: 2063 6f6e 6669 672e 6361 6c69 6272 6174   config.calibrat
-00002bc0: 696f 6e5b 6d6f 6465 5d5b 2773 7461 6765  ion[mode]['stage
-00002bd0: 6d61 7472 6978 275d 5b6d 6167 6e69 6669  matrix'][magnifi
-00002be0: 6361 7469 6f6e 5d5c 6e22 2c0d 0a20 2020  cation]\n",..   
-00002bf0: 2022 2020 2020 6d61 7073 6361 6c65 6d61   "    mapscalema
-00002c00: 7420 3d20 5b69 7465 6d2f 6269 6e73 697a  t = [item/binsiz
-00002c10: 6520 666f 7220 6974 656d 2069 6e20 6d61  e for item in ma
-00002c20: 7073 6361 6c65 6d61 745d 5c6e 222c 0d0a  pscalemat]\n",..
-00002c30: 2020 2020 2220 2020 205c 6e22 2c0d 0a20      "    \n",.. 
-00002c40: 2020 2022 2020 2020 666f 7220 692c 2069     "    for i, i
-00002c50: 6d61 6765 2069 6e20 656e 756d 6572 6174  mage in enumerat
-00002c60: 6528 6275 6666 6572 293a 5c6e 222c 0d0a  e(buffer):\n",..
-00002c70: 2020 2020 2220 2020 2020 2020 2078 2c20      "        x, 
-00002c80: 792c 207a 2c20 5f2c 205f 203d 2073 7461  y, z, _, _ = sta
-00002c90: 6765 706f 735b 695d 5c6e 222c 0d0a 2020  gepos[i]\n",..  
-00002ca0: 2020 2220 2020 2020 2020 2073 6861 7065    "        shape
-00002cb0: 203d 2069 6d61 6765 2e73 6861 7065 5c6e   = image.shape\n
-00002cc0: 222c 0d0a 2020 2020 2220 2020 2020 2020  ",..    "       
-00002cd0: 2023 2062 696e 7369 7a65 203d 2063 7472   # binsize = ctr
-00002ce0: 6c2e 6361 6d2e 6765 7442 696e 6e69 6e67  l.cam.getBinning
-00002cf0: 2829 5c6e 222c 0d0a 2020 2020 225c 6e22  ()\n",..    "\n"
-00002d00: 2c0d 0a20 2020 2022 2020 2020 2020 2020  ,..    "        
-00002d10: 6420 3d20 7b7d 5c6e 222c 0d0a 2020 2020  d = {}\n",..    
-00002d20: 2220 2020 2020 2020 2064 5b27 5374 6167  "        d['Stag
-00002d30: 6558 595a 275d 203d 2078 202f 2031 3030  eXYZ'] = x / 100
-00002d40: 302c 2079 202f 2031 3030 302c 207a 202f  0, y / 1000, z /
-00002d50: 2031 3030 305c 6e22 2c0d 0a20 2020 2022   1000\n",..    "
-00002d60: 2020 2020 2020 2020 645b 274d 6170 4669          d['MapFi
-00002d70: 6c65 275d 203d 2066 6e5f 6d72 635c 6e22  le'] = fn_mrc\n"
-00002d80: 2c0d 0a20 2020 2022 2020 2020 2020 2020  ,..    "        
-00002d90: 645b 274d 6170 5365 6374 696f 6e27 5d20  d['MapSection'] 
-00002da0: 3d20 695c 6e22 2c0d 0a20 2020 2022 2020  = i\n",..    "  
-00002db0: 2020 2020 2020 645b 274d 6170 4269 6e6e        d['MapBinn
-00002dc0: 696e 6727 5d20 3d20 6269 6e73 697a 655c  ing'] = binsize\
-00002dd0: 6e22 2c0d 0a20 2020 2022 2020 2020 2020  n",..    "      
-00002de0: 2020 645b 274d 6170 4d61 6749 6e64 275d    d['MapMagInd']
-00002df0: 203d 2063 7472 6c2e 6d61 676e 6966 6963   = ctrl.magnific
-00002e00: 6174 696f 6e2e 6162 736f 6c75 7465 5f69  ation.absolute_i
-00002e10: 6e64 6578 202b 2031 2020 2320 5365 7269  ndex + 1  # Seri
-00002e20: 616c 454d 2069 7320 312d 6261 7365 645c  alEM is 1-based\
-00002e30: 6e22 2c0d 0a20 2020 2022 2020 2020 2020  n",..    "      
-00002e40: 2020 645b 274d 6170 5363 616c 654d 6174    d['MapScaleMat
-00002e50: 275d 203d 206d 6170 7363 616c 656d 6174  '] = mapscalemat
-00002e60: 5c6e 222c 0d0a 2020 2020 2220 2020 2020  \n",..    "     
-00002e70: 2020 2064 5b27 4d61 7057 6964 7468 4865     d['MapWidthHe
-00002e80: 6967 6874 275d 203d 2073 6861 7065 5c6e  ight'] = shape\n
-00002e90: 222c 0d0a 2020 2020 225c 6e22 2c0d 0a20  ",..    "\n",.. 
-00002ea0: 2020 2022 2020 2020 2020 2020 6d61 705f     "        map_
-00002eb0: 6974 656d 203d 204d 6170 4974 656d 2e66  item = MapItem.f
-00002ec0: 726f 6d5f 6469 6374 2864 295c 6e22 2c0d  rom_dict(d)\n",.
-00002ed0: 0a20 2020 2022 2020 2020 2020 2020 6974  .    "        it
-00002ee0: 656d 732e 6170 7065 6e64 286d 6170 5f69  ems.append(map_i
-00002ef0: 7465 6d29 5c6e 222c 0d0a 2020 2020 225c  tem)\n",..    "\
-00002f00: 6e22 2c0d 0a20 2020 2022 2020 2020 7772  n",..    "    wr
-00002f10: 6974 655f 6e61 765f 6669 6c65 2866 6e5f  ite_nav_file(fn_
-00002f20: 6e61 762c 202a 6974 656d 7329 5c6e 222c  nav, *items)\n",
-00002f30: 0d0a 2020 2020 2220 2020 205c 6e22 2c0d  ..    "    \n",.
-00002f40: 0a20 2020 2022 2020 2020 7072 696e 7428  .    "    print(
-00002f50: 665c 2244 6174 6120 7361 7665 6420 746f  f\"Data saved to
-00002f60: 2060 7b66 6e5f 6e61 767d 6020 616e 6420   `{fn_nav}` and 
-00002f70: 607b 666e 5f6d 7263 7d60 2028 7b6c 656e  `{fn_mrc}` ({len
-00002f80: 2862 7566 6665 7229 7d20 696d 6167 6573  (buffer)} images
-00002f90: 295c 2229 220d 0a20 2020 5d0d 0a20 207d  )\")"..   ]..  }
-00002fa0: 2c0d 0a20 207b 0d0a 2020 2022 6365 6c6c  ,..  {..   "cell
-00002fb0: 5f74 7970 6522 3a20 226d 6172 6b64 6f77  _type": "markdow
-00002fc0: 6e22 2c0d 0a20 2020 226d 6574 6164 6174  n",..   "metadat
-00002fd0: 6122 3a20 7b7d 2c0d 0a20 2020 2273 6f75  a": {},..   "sou
-00002fe0: 7263 6522 3a20 5b0d 0a20 2020 2022 4e65  rce": [..    "Ne
-00002ff0: 7874 2077 6520 6361 6c6c 2060 6374 726c  xt we call `ctrl
-00003000: 2e61 6371 7569 7265 5f61 745f 6974 656d  .acquire_at_item
-00003010: 7360 2061 7320 6265 666f 7265 2077 6974  s` as before wit
-00003020: 6820 7468 6520 6e65 7720 6070 6f73 745f  h the new `post_
-00003030: 6163 7175 6972 6560 2066 756e 6374 696f  acquire` functio
-00003040: 6e2e 220d 0a20 2020 5d0d 0a20 207d 2c0d  n."..   ]..  },.
-00003050: 0a20 207b 0d0a 2020 2022 6365 6c6c 5f74  .  {..   "cell_t
-00003060: 7970 6522 3a20 2263 6f64 6522 2c0d 0a20  ype": "code",.. 
-00003070: 2020 2265 7865 6375 7469 6f6e 5f63 6f75    "execution_cou
-00003080: 6e74 223a 206e 756c 6c2c 0d0a 2020 2022  nt": null,..   "
-00003090: 6d65 7461 6461 7461 223a 207b 7d2c 0d0a  metadata": {},..
-000030a0: 2020 2022 6f75 7470 7574 7322 3a20 5b5d     "outputs": []
-000030b0: 2c0d 0a20 2020 2273 6f75 7263 6522 3a20  ,..   "source": 
-000030c0: 5b0d 0a20 2020 2022 7365 6c20 3d20 7374  [..    "sel = st
-000030d0: 6167 6563 6f6f 7264 735b 303a 3130 5d20  agecoords[0:10] 
-000030e0: 2023 2041 6371 7569 7265 2061 7420 7468   # Acquire at th
-000030f0: 6520 6669 7273 7420 3130 2069 7465 6d73  e first 10 items
-00003100: 5c6e 222c 0d0a 2020 2020 2263 7472 6c2e  \n",..    "ctrl.
-00003110: 6163 7175 6972 655f 6174 5f69 7465 6d73  acquire_at_items
-00003120: 2873 656c 2c20 5c6e 222c 0d0a 2020 2020  (sel, \n",..    
-00003130: 2220 2020 2020 2020 2020 2020 2020 2020  "               
-00003140: 2020 2020 2020 2061 6371 7569 7265 3d61         acquire=a
-00003150: 6371 7569 7265 5f66 756e 632c 205c 6e22  cquire_func, \n"
-00003160: 2c0d 0a20 2020 2022 2020 2020 2020 2020  ,..    "        
-00003170: 2020 2020 2020 2020 2020 2020 2020 706f                po
-00003180: 7374 5f61 6371 7569 7265 3d70 6f73 745f  st_acquire=post_
-00003190: 6163 7175 6972 6529 220d 0a20 2020 5d0d  acquire)"..   ].
-000031a0: 0a20 207d 2c0d 0a20 207b 0d0a 2020 2022  .  },..  {..   "
-000031b0: 6365 6c6c 5f74 7970 6522 3a20 226d 6172  cell_type": "mar
-000031c0: 6b64 6f77 6e22 2c0d 0a20 2020 226d 6574  kdown",..   "met
-000031d0: 6164 6174 6122 3a20 7b7d 2c0d 0a20 2020  adata": {},..   
-000031e0: 2273 6f75 7263 6522 3a20 5b0d 0a20 2020  "source": [..   
-000031f0: 2022 4e6f 7720 6c6f 6164 2075 7020 7468   "Now load up th
-00003200: 6520 6069 6e73 7461 6d61 7469 632e 6e61  e `instamatic.na
-00003210: 7660 2066 696c 6520 696e 2060 5365 7269  v` file in `Seri
-00003220: 616c 454d 6020 746f 2073 6565 2074 6865  alEM` to see the
-00003230: 2072 6573 756c 7421 220d 0a20 2020 5d0d   result!"..   ].
-00003240: 0a20 207d 2c0d 0a20 207b 0d0a 2020 2022  .  },..  {..   "
-00003250: 6365 6c6c 5f74 7970 6522 3a20 2263 6f64  cell_type": "cod
-00003260: 6522 2c0d 0a20 2020 2265 7865 6375 7469  e",..   "executi
-00003270: 6f6e 5f63 6f75 6e74 223a 206e 756c 6c2c  on_count": null,
-00003280: 0d0a 2020 2022 6d65 7461 6461 7461 223a  ..   "metadata":
-00003290: 207b 7d2c 0d0a 2020 2022 6f75 7470 7574   {},..   "output
-000032a0: 7322 3a20 5b5d 2c0d 0a20 2020 2273 6f75  s": [],..   "sou
-000032b0: 7263 6522 3a20 5b5d 0d0a 2020 7d2c 0d0a  rce": []..  },..
-000032c0: 2020 7b0d 0a20 2020 2263 656c 6c5f 7479    {..   "cell_ty
-000032d0: 7065 223a 2022 636f 6465 222c 0d0a 2020  pe": "code",..  
-000032e0: 2022 6578 6563 7574 696f 6e5f 636f 756e   "execution_coun
-000032f0: 7422 3a20 6e75 6c6c 2c0d 0a20 2020 226d  t": null,..   "m
-00003300: 6574 6164 6174 6122 3a20 7b7d 2c0d 0a20  etadata": {},.. 
-00003310: 2020 226f 7574 7075 7473 223a 205b 5d2c    "outputs": [],
-00003320: 0d0a 2020 2022 736f 7572 6365 223a 205b  ..   "source": [
-00003330: 5d0d 0a20 207d 0d0a 205d 2c0d 0a20 226d  ]..  }.. ],.. "m
-00003340: 6574 6164 6174 6122 3a20 7b0d 0a20 2022  etadata": {..  "
-00003350: 6b65 726e 656c 7370 6563 223a 207b 0d0a  kernelspec": {..
-00003360: 2020 2022 6469 7370 6c61 795f 6e61 6d65     "display_name
-00003370: 223a 2022 5079 7468 6f6e 2033 222c 0d0a  ": "Python 3",..
-00003380: 2020 2022 6c61 6e67 7561 6765 223a 2022     "language": "
-00003390: 7079 7468 6f6e 222c 0d0a 2020 2022 6e61  python",..   "na
-000033a0: 6d65 223a 2022 7079 7468 6f6e 3322 0d0a  me": "python3"..
-000033b0: 2020 7d2c 0d0a 2020 226c 616e 6775 6167    },..  "languag
-000033c0: 655f 696e 666f 223a 207b 0d0a 2020 2022  e_info": {..   "
-000033d0: 636f 6465 6d69 7272 6f72 5f6d 6f64 6522  codemirror_mode"
-000033e0: 3a20 7b0d 0a20 2020 2022 6e61 6d65 223a  : {..    "name":
-000033f0: 2022 6970 7974 686f 6e22 2c0d 0a20 2020   "ipython",..   
-00003400: 2022 7665 7273 696f 6e22 3a20 330d 0a20   "version": 3.. 
-00003410: 2020 7d2c 0d0a 2020 2022 6669 6c65 5f65    },..   "file_e
-00003420: 7874 656e 7369 6f6e 223a 2022 2e70 7922  xtension": ".py"
-00003430: 2c0d 0a20 2020 226d 696d 6574 7970 6522  ,..   "mimetype"
-00003440: 3a20 2274 6578 742f 782d 7079 7468 6f6e  : "text/x-python
-00003450: 222c 0d0a 2020 2022 6e61 6d65 223a 2022  ",..   "name": "
-00003460: 7079 7468 6f6e 222c 0d0a 2020 2022 6e62  python",..   "nb
-00003470: 636f 6e76 6572 745f 6578 706f 7274 6572  convert_exporter
-00003480: 223a 2022 7079 7468 6f6e 222c 0d0a 2020  ": "python",..  
-00003490: 2022 7079 676d 656e 7473 5f6c 6578 6572   "pygments_lexer
-000034a0: 223a 2022 6970 7974 686f 6e33 222c 0d0a  ": "ipython3",..
-000034b0: 2020 2022 7665 7273 696f 6e22 3a20 2233     "version": "3
-000034c0: 2e38 2e33 220d 0a20 207d 0d0a 207d 2c0d  .8.3"..  }.. },.
-000034d0: 0a20 226e 6266 6f72 6d61 7422 3a20 342c  . "nbformat": 4,
-000034e0: 0d0a 2022 6e62 666f 726d 6174 5f6d 696e  .. "nbformat_min
-000034f0: 6f72 223a 2032 0d0a 7d0d 0a              or": 2..}..
+00000000: 7b0a 2022 6365 6c6c 7322 3a20 5b0a 2020  {. "cells": [.  
+00000010: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
+00000020: 3a20 2263 6f64 6522 2c0a 2020 2022 6578  : "code",.   "ex
+00000030: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
+00000040: 6e75 6c6c 2c0a 2020 2022 6d65 7461 6461  null,.   "metada
+00000050: 7461 223a 207b 7d2c 0a20 2020 226f 7574  ta": {},.   "out
+00000060: 7075 7473 223a 205b 5d2c 0a20 2020 2273  puts": [],.   "s
+00000070: 6f75 7263 6522 3a20 5b0a 2020 2020 2225  ource": [.    "%
+00000080: 6c6f 6164 5f65 7874 2061 7574 6f72 656c  load_ext autorel
+00000090: 6f61 645c 6e22 2c0a 2020 2020 2225 6175  oad\n",.    "%au
+000000a0: 746f 7265 6c6f 6164 2032 220a 2020 205d  toreload 2".   ]
+000000b0: 0a20 207d 2c0a 2020 7b0a 2020 2022 6365  .  },.  {.   "ce
+000000c0: 6c6c 5f74 7970 6522 3a20 226d 6172 6b64  ll_type": "markd
+000000d0: 6f77 6e22 2c0a 2020 2022 6d65 7461 6461  own",.   "metada
+000000e0: 7461 223a 207b 7d2c 0a20 2020 2273 6f75  ta": {},.   "sou
+000000f0: 7263 6522 3a20 5b0a 2020 2020 2223 2049  rce": [.    "# I
+00000100: 6e73 7461 6d61 7469 6320 2d20 6d6f 6e74  nstamatic - mont
+00000110: 6167 696e 675c 6e22 2c0a 2020 2020 225c  aging\n",.    "\
+00000120: 6e22 2c0a 2020 2020 2249 6e73 7461 6d61  n",.    "Instama
+00000130: 7469 6320 6973 2061 2074 6f6f 6c20 666f  tic is a tool fo
+00000140: 7220 6175 746f 6d61 7465 6420 656c 6563  r automated elec
+00000150: 7472 6f6e 2064 6966 6672 6163 7469 6f6e  tron diffraction
+00000160: 2064 6174 6120 636f 6c6c 6563 7469 6f6e   data collection
+00000170: 2e20 4974 2068 6173 2069 6e74 6572 6661  . It has interfa
+00000180: 6365 7320 666f 7220 696e 7465 7266 6163  ces for interfac
+00000190: 696e 6720 7769 7468 2074 6865 2054 454d  ing with the TEM
+000001a0: 2028 4a45 4f4c 2f54 4653 2920 616e 6420   (JEOL/TFS) and 
+000001b0: 7365 7665 7261 6c20 6361 6d65 7261 7320  several cameras 
+000001c0: 2847 6174 616e 2f41 5349 2054 696d 6570  (Gatan/ASI Timep
+000001d0: 6978 2f54 5649 5053 292e 5c6e 222c 0a20  ix/TVIPS).\n",. 
+000001e0: 2020 2022 5c6e 222c 0a20 2020 2022 6874     "\n",.    "ht
+000001f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000200: 2f69 6e73 7461 6d61 7469 632d 6465 762f  /instamatic-dev/
+00000210: 696e 7374 616d 6174 6963 5c6e 222c 0a20  instamatic\n",. 
+00000220: 2020 2022 5c6e 222c 0a20 2020 2022 5468     "\n",.    "Th
+00000230: 6973 206e 6f74 6562 6f6f 6b20 7368 6f77  is notebook show
+00000240: 7320 686f 7720 746f 2070 726f 6365 7373  s how to process
+00000250: 2061 2067 7269 6420 6d6f 6e74 6167 6520   a grid montage 
+00000260: 7573 696e 6720 6069 6e73 7461 6d61 7469  using `instamati
+00000270: 6360 2c20 7069 636b 2067 7269 6420 7371  c`, pick grid sq
+00000280: 7561 7265 732c 2061 6e64 2073 6574 2075  uares, and set u
+00000290: 7020 616e 2061 6371 7569 7369 7469 6f6e  p an acquisition
+000002a0: 2028 6061 6371 7569 7265 5f61 745f 6974   (`acquire_at_it
+000002b0: 656d 7360 292e 2054 6865 2064 6174 6120  ems`). The data 
+000002c0: 7765 7265 2063 6f6c 6c65 6374 6564 206f  were collected o
+000002d0: 6e20 6120 7a65 6f6c 6974 6520 7361 6d70  n a zeolite samp
+000002e0: 6c65 2028 3230 3230 2d30 322d 3132 292c  le (2020-02-12),
+000002f0: 2075 7369 6e67 2061 204a 454f 4c20 4a45   using a JEOL JE
+00000300: 4d2d 3134 3030 2040 2031 3230 206b 5620  M-1400 @ 120 kV 
+00000310: 696e 2063 6f6d 6269 6e61 7469 6f6e 2077  in combination w
+00000320: 6974 6820 6120 5456 4950 5320 462d 3431  ith a TVIPS F-41
+00000330: 3620 6361 6d65 7261 2e5c 6e22 2c0a 2020  6 camera.\n",.  
+00000340: 2020 225c 6e22 2c0a 2020 2020 2254 6865    "\n",.    "The
+00000350: 2064 6174 6120 666f 7220 7468 6973 2064   data for this d
+00000360: 656d 6f20 6172 6520 6176 6169 6c61 626c  emo are availabl
+00000370: 6520 6672 6f6d 207a 656e 6f64 6f3a 2068  e from zenodo: h
+00000380: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
+00000390: 302e 3532 3831 2f7a 656e 6f64 6f2e 3339  0.5281/zenodo.39
+000003a0: 3234 3038 395c 6e22 2c0a 2020 2020 225c  24089\n",.    "\
+000003b0: 6e22 2c0a 2020 2020 224d 616b 6520 7375  n",.    "Make su
+000003c0: 7265 2074 6f20 6368 616e 6765 2074 6865  re to change the
+000003d0: 2077 6f72 6b20 6469 7265 6374 6f72 7920   work directory 
+000003e0: 6265 6c6f 7720 746f 2070 6f69 6e74 2061  below to point a
+000003f0: 7420 7468 6520 7269 6768 7420 6c6f 6361  t the right loca
+00000400: 7469 6f6e 2e22 0a20 2020 5d0a 2020 7d2c  tion.".   ].  },
+00000410: 0a20 207b 0a20 2020 2263 656c 6c5f 7479  .  {.   "cell_ty
+00000420: 7065 223a 2022 636f 6465 222c 0a20 2020  pe": "code",.   
+00000430: 2265 7865 6375 7469 6f6e 5f63 6f75 6e74  "execution_count
+00000440: 223a 206e 756c 6c2c 0a20 2020 226d 6574  ": null,.   "met
+00000450: 6164 6174 6122 3a20 7b7d 2c0a 2020 2022  adata": {},.   "
+00000460: 6f75 7470 7574 7322 3a20 5b5d 2c0a 2020  outputs": [],.  
+00000470: 2022 736f 7572 6365 223a 205b 0a20 2020   "source": [.   
+00000480: 2022 6672 6f6d 2069 6e73 7461 6d61 7469   "from instamati
+00000490: 632e 6d6f 6e74 6167 6520 696d 706f 7274  c.montage import
+000004a0: 202a 5c6e 222c 0a20 2020 2022 696d 706f   *\n",.    "impo
+000004b0: 7274 206e 756d 7079 2061 7320 6e70 5c6e  rt numpy as np\n
+000004c0: 222c 0a20 2020 2022 6672 6f6d 2070 6174  ",.    "from pat
+000004d0: 686c 6962 2069 6d70 6f72 7420 5061 7468  hlib import Path
+000004e0: 5c6e 222c 0a20 2020 2022 6e70 2e73 6574  \n",.    "np.set
+000004f0: 5f70 7269 6e74 6f70 7469 6f6e 7328 7375  _printoptions(su
+00000500: 7070 7265 7373 3d54 7275 6529 5c6e 222c  ppress=True)\n",
+00000510: 0a20 2020 2022 5c6e 222c 0a20 2020 2022  .    "\n",.    "
+00000520: 2320 776f 726b 2064 6972 6563 746f 7279  # work directory
+00000530: 5c6e 222c 0a20 2020 2022 776f 726b 203d  \n",.    "work =
+00000540: 2050 6174 6828 725c 2243 3a2f 732f 6461   Path(r\"C:/s/da
+00000550: 7461 2f6d 6f6e 7461 6765 5f31 5c22 2922  ta/montage_1\")"
+00000560: 0a20 2020 5d0a 2020 7d2c 0a20 207b 0a20  .   ].  },.  {. 
+00000570: 2020 2263 656c 6c5f 7479 7065 223a 2022    "cell_type": "
+00000580: 6d61 726b 646f 776e 222c 0a20 2020 226d  markdown",.   "m
+00000590: 6574 6164 6174 6122 3a20 7b7d 2c0a 2020  etadata": {},.  
+000005a0: 2022 736f 7572 6365 223a 205b 0a20 2020   "source": [.   
+000005b0: 2022 2323 2053 6574 7469 6e67 2075 7020   "## Setting up 
+000005c0: 7468 6520 6d6f 6e74 6167 655c 6e22 2c0a  the montage\n",.
+000005d0: 2020 2020 225c 6e22 2c0a 2020 2020 224c      "\n",.    "L
+000005e0: 6f61 6420 7468 6520 606d 6f6e 7461 6765  oad the `montage
+000005f0: 2e79 616d 6c60 2066 696c 6520 616e 6420  .yaml` file and 
+00000600: 7468 6520 6173 736f 6369 6174 6564 2069  the associated i
+00000610: 6d61 6765 732e 220a 2020 205d 0a20 207d  mages.".   ].  }
+00000620: 2c0a 2020 7b0a 2020 2022 6365 6c6c 5f74  ,.  {.   "cell_t
+00000630: 7970 6522 3a20 2263 6f64 6522 2c0a 2020  ype": "code",.  
+00000640: 2022 6578 6563 7574 696f 6e5f 636f 756e   "execution_coun
+00000650: 7422 3a20 6e75 6c6c 2c0a 2020 2022 6d65  t": null,.   "me
+00000660: 7461 6461 7461 223a 207b 7d2c 0a20 2020  tadata": {},.   
+00000670: 226f 7574 7075 7473 223a 205b 5d2c 0a20  "outputs": [],. 
+00000680: 2020 2273 6f75 7263 6522 3a20 5b0a 2020    "source": [.  
+00000690: 2020 226d 203d 2049 6e73 7461 6d61 7469    "m = Instamati
+000006a0: 634d 6f6e 7461 6765 2e66 726f 6d5f 6d6f  cMontage.from_mo
+000006b0: 6e74 6167 655f 7961 6d6c 2877 6f72 6b20  ntage_yaml(work 
+000006c0: 2f20 276d 6f6e 7461 6765 2e79 616d 6c27  / 'montage.yaml'
+000006d0: 295c 6e22 2c0a 2020 2020 226d 2e67 7269  )\n",.    "m.gri
+000006e0: 6473 7065 6322 0a20 2020 5d0a 2020 7d2c  dspec".   ].  },
+000006f0: 0a20 207b 0a20 2020 2263 656c 6c5f 7479  .  {.   "cell_ty
+00000700: 7065 223a 2022 6d61 726b 646f 776e 222c  pe": "markdown",
+00000710: 0a20 2020 226d 6574 6164 6174 6122 3a20  .   "metadata": 
+00000720: 7b7d 2c0a 2020 2022 736f 7572 6365 223a  {},.   "source":
+00000730: 205b 0a20 2020 2022 4669 7273 742c 2077   [.    "First, w
+00000740: 6520 6361 6e20 6368 6563 6b20 7768 6174  e can check what
+00000750: 2074 6865 2064 6174 6120 6163 7475 616c   the data actual
+00000760: 6c79 206c 6f6f 6b20 6c69 6b65 2e20 546f  ly look like. To
+00000770: 2064 6f20 736f 2c20 7765 2063 616e 2073   do so, we can s
+00000780: 696d 706c 7920 6073 7469 7463 6860 2061  imply `stitch` a
+00000790: 6e64 2060 706c 6f74 6020 7468 6520 6461  nd `plot` the da
+000007a0: 7461 2075 7369 6e67 2061 2060 6269 6e6e  ta using a `binn
+000007b0: 696e 673d 3460 2074 6f20 636f 6e73 6572  ing=4` to conser
+000007c0: 7665 2061 2062 6974 206f 6620 6d65 6d6f  ve a bit of memo
+000007d0: 7279 2e20 5468 6973 206e 6169 7665 6c79  ry. This naively
+000007e0: 2070 6c6f 7473 2074 6865 2064 6174 6120   plots the data 
+000007f0: 6174 2074 6865 2065 7870 6563 7465 6420  at the expected 
+00000800: 706f 7369 7469 6f6e 732e 2041 6c74 686f  positions. Altho
+00000810: 7567 6820 7468 6520 7374 6974 6368 696e  ugh the stitchin
+00000820: 6720 6973 206e 6f74 2074 6861 7420 6772  g is not that gr
+00000830: 6561 742c 2069 7427 7320 656e 6f75 6768  eat, it's enough
+00000840: 2074 6f20 6765 7420 6120 6665 656c 696e   to get a feelin
+00000850: 6720 666f 7220 7468 6520 6461 7461 2e22  g for the data."
+00000860: 0a20 2020 5d0a 2020 7d2c 0a20 207b 0a20  .   ].  },.  {. 
+00000870: 2020 2263 656c 6c5f 7479 7065 223a 2022    "cell_type": "
+00000880: 636f 6465 222c 0a20 2020 2265 7865 6375  code",.   "execu
+00000890: 7469 6f6e 5f63 6f75 6e74 223a 206e 756c  tion_count": nul
+000008a0: 6c2c 0a20 2020 226d 6574 6164 6174 6122  l,.   "metadata"
+000008b0: 3a20 7b7d 2c0a 2020 2022 6f75 7470 7574  : {},.   "output
+000008c0: 7322 3a20 5b5d 2c0a 2020 2022 736f 7572  s": [],.   "sour
+000008d0: 6365 223a 205b 0a20 2020 2022 6d2e 6361  ce": [.    "m.ca
+000008e0: 6c63 756c 6174 655f 6d6f 6e74 6167 655f  lculate_montage_
+000008f0: 636f 6f72 6473 2829 5c6e 222c 0a20 2020  coords()\n",.   
+00000900: 2022 6d2e 7374 6974 6368 2862 696e 6e69   "m.stitch(binni
+00000910: 6e67 3d34 295c 6e22 2c0a 2020 2020 226d  ng=4)\n",.    "m
+00000920: 2e70 6c6f 7428 2922 0a20 2020 5d0a 2020  .plot()".   ].  
+00000930: 7d2c 0a20 207b 0a20 2020 2263 656c 6c5f  },.  {.   "cell_
+00000940: 7479 7065 223a 2022 6d61 726b 646f 776e  type": "markdown
+00000950: 222c 0a20 2020 226d 6574 6164 6174 6122  ",.   "metadata"
+00000960: 3a20 7b7d 2c0a 2020 2022 736f 7572 6365  : {},.   "source
+00000970: 223a 205b 0a20 2020 2022 546f 2067 6574  ": [.    "To get
+00000980: 2062 6574 7465 7220 7374 6974 6368 696e   better stitchin
+00000990: 672c 2077 6520 6e65 6564 2074 6f3a 5c6e  g, we need to:\n
+000009a0: 222c 0a20 2020 2022 5c6e 222c 0a20 2020  ",.    "\n",.   
+000009b0: 2022 2031 2e20 4265 7474 6572 2065 7374   " 1. Better est
+000009c0: 696d 6174 6520 7468 6520 6469 6666 6572  imate the differ
+000009d0: 656e 6365 2076 6563 746f 7273 2062 6574  ence vectors bet
+000009e0: 7765 656e 2065 6163 6820 7469 6c65 2075  ween each tile u
+000009f0: 7369 6e67 2063 726f 7373 2063 6f72 7265  sing cross corre
+00000a00: 6c61 7469 6f6e 5c6e 222c 0a20 2020 2022  lation\n",.    "
+00000a10: 2032 2e20 4f70 7469 6d69 7a65 2074 6865   2. Optimize the
+00000a20: 2063 6f6f 7264 696e 6174 6573 206f 6620   coordinates of 
+00000a30: 7468 6520 6469 6666 6572 656e 6365 2076  the difference v
+00000a40: 6563 746f 7273 2075 7369 6e67 206c 6561  ectors using lea
+00000a50: 7374 2d73 7175 6172 6573 206d 696e 696d  st-squares minim
+00000a60: 697a 6174 696f 6e5c 6e22 2c0a 2020 2020  ization\n",.    
+00000a70: 225c 6e22 2c0a 2020 2020 2254 6869 7320  "\n",.    "This 
+00000a80: 6170 7072 6f61 6368 2069 7320 6261 7365  approach is base
+00000a90: 6420 6f6e 202a 476c 6f62 616c 6c79 206f  d on *Globally o
+00000aa0: 7074 696d 616c 2073 7469 7463 6869 6e67  ptimal stitching
+00000ab0: 206f 6620 7469 6c65 6420 3344 206d 6963   of tiled 3D mic
+00000ac0: 726f 7363 6f70 6963 2069 6d61 6765 2061  roscopic image a
+00000ad0: 6371 7569 7369 7469 6f6e 732a 2062 7920  cquisitions* by 
+00000ae0: 5072 6569 6269 7368 2065 7420 616c 2e2c  Preibish et al.,
+00000af0: 2042 696f 696e 666f 726d 6174 6963 7320   Bioinformatics 
+00000b00: 3235 2028 3230 3039 292c 2031 3436 33e2  25 (2009), 1463.
+00000b10: 8093 3134 3635 2028 6874 7470 733a 2f2f  ..1465 (https://
+00000b20: 646f 692e 6f72 672f 3130 2e31 3039 332f  doi.org/10.1093/
+00000b30: 6269 6f69 6e66 6f72 6d61 7469 6373 2f62  bioinformatics/b
+00000b40: 7470 3138 3429 2e5c 6e22 2c0a 2020 2020  tp184).\n",.    
+00000b50: 225c 6e22 2c0a 2020 2020 2253 6f6d 6520  "\n",.    "Some 
+00000b60: 6d65 7472 6963 732c 2073 7563 6820 6173  metrics, such as
+00000b70: 2074 6865 206f 6274 6169 6e65 6420 7368   the obtained sh
+00000b80: 6966 7473 2061 6e64 2046 4654 2073 636f  ifts and FFT sco
+00000b90: 7265 7320 6172 6520 706c 6f74 7465 6420  res are plotted 
+00000ba0: 746f 2065 7661 6c75 6174 6520 7468 6520  to evaluate the 
+00000bb0: 7374 6974 6368 696e 672e 220a 2020 205d  stitching.".   ]
+00000bc0: 0a20 207d 2c0a 2020 7b0a 2020 2022 6365  .  },.  {.   "ce
+00000bd0: 6c6c 5f74 7970 6522 3a20 2263 6f64 6522  ll_type": "code"
+00000be0: 2c0a 2020 2022 6578 6563 7574 696f 6e5f  ,.   "execution_
+00000bf0: 636f 756e 7422 3a20 6e75 6c6c 2c0a 2020  count": null,.  
+00000c00: 2022 6d65 7461 6461 7461 223a 207b 7d2c   "metadata": {},
+00000c10: 0a20 2020 226f 7574 7075 7473 223a 205b  .   "outputs": [
+00000c20: 5d2c 0a20 2020 2273 6f75 7263 6522 3a20  ],.   "source": 
+00000c30: 5b0a 2020 2020 2223 2055 7365 2063 726f  [.    "# Use cro
+00000c40: 7373 2063 6f72 7265 6c61 7469 6f6e 2074  ss correlation t
+00000c50: 6f20 6765 7420 6469 6666 6572 656e 6365  o get difference
+00000c60: 2076 6563 746f 7273 5c6e 222c 0a20 2020   vectors\n",.   
+00000c70: 2022 6d2e 6361 6c63 756c 6174 655f 6469   "m.calculate_di
+00000c80: 6666 6572 656e 6365 5f76 6563 746f 7273  fference_vectors
+00000c90: 2874 6872 6573 686f 6c64 3d27 6175 746f  (threshold='auto
+00000ca0: 272c 205c 6e22 2c0a 2020 2020 2220 2020  ', \n",.    "   
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cc0: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
+00000cd0: 6f64 3d27 736b 696d 6167 6527 2c20 5c6e  od='skimage', \n
+00000ce0: 222c 0a20 2020 2022 2020 2020 2020 2020  ",.    "        
+00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d00: 2020 2020 2020 2070 6c6f 743d 4661 6c73         plot=Fals
+00000d10: 6529 5c6e 222c 0a20 2020 2022 5c6e 222c  e)\n",.    "\n",
+00000d20: 0a20 2020 2022 2320 706c 6f74 2074 6865  .    "# plot the
+00000d30: 2066 6674 5f73 636f 7265 735c 6e22 2c0a   fft_scores\n",.
+00000d40: 2020 2020 226d 2e70 6c6f 745f 6666 745f      "m.plot_fft_
+00000d50: 7363 6f72 6573 2829 5c6e 222c 0a20 2020  scores()\n",.   
+00000d60: 2022 5c6e 222c 0a20 2020 2022 2320 706c   "\n",.    "# pl
+00000d70: 6f74 2074 6865 2070 6978 656c 2073 6869  ot the pixel shi
+00000d80: 6674 735c 6e22 2c0a 2020 2020 226d 2e70  fts\n",.    "m.p
+00000d90: 6c6f 745f 7368 6966 7473 2829 5c6e 222c  lot_shifts()\n",
+00000da0: 0a20 2020 2022 5c6e 222c 0a20 2020 2022  .    "\n",.    "
+00000db0: 2320 6765 7420 636f 6f72 6473 206f 7074  # get coords opt
+00000dc0: 696d 697a 6564 2075 7369 6e67 2063 726f  imized using cro
+00000dd0: 7373 2063 6f72 7265 6c61 7469 6f6e 5c6e  ss correlation\n
+00000de0: 222c 0a20 2020 2022 6d2e 6f70 7469 6d69  ",.    "m.optimi
+00000df0: 7a65 5f6d 6f6e 7461 6765 5f63 6f6f 7264  ze_montage_coord
+00000e00: 7328 706c 6f74 3d54 7275 6529 5c6e 222c  s(plot=True)\n",
+00000e10: 0a20 2020 2022 5c6e 222c 0a20 2020 2022  .    "\n",.    "
+00000e20: 2320 7374 6974 6368 2069 6d61 6765 2c20  # stitch image, 
+00000e30: 7573 6520 6269 6e6e 696e 6720 3420 666f  use binning 4 fo
+00000e40: 7220 7370 6565 642d 7570 2061 6e64 206d  r speed-up and m
+00000e50: 656d 6f72 7920 636f 6e73 6572 7661 7469  emory conservati
+00000e60: 6f6e 5c6e 222c 0a20 2020 2022 6d2e 7374  on\n",.    "m.st
+00000e70: 6974 6368 2862 696e 6e69 6e67 3d34 295c  itch(binning=4)\
+00000e80: 6e22 2c0a 2020 2020 225c 6e22 2c0a 2020  n",.    "\n",.  
+00000e90: 2020 2223 2070 6c6f 7420 7468 6520 7374    "# plot the st
+00000ea0: 6974 6368 6564 2069 6d61 6765 5c6e 222c  itched image\n",
+00000eb0: 0a20 2020 2022 6d2e 706c 6f74 2829 220a  .    "m.plot()".
+00000ec0: 2020 205d 0a20 207d 2c0a 2020 7b0a 2020     ].  },.  {.  
+00000ed0: 2022 6365 6c6c 5f74 7970 6522 3a20 226d   "cell_type": "m
+00000ee0: 6172 6b64 6f77 6e22 2c0a 2020 2022 6d65  arkdown",.   "me
+00000ef0: 7461 6461 7461 223a 207b 7d2c 0a20 2020  tadata": {},.   
+00000f00: 2273 6f75 7263 6522 3a20 5b0a 2020 2020  "source": [.    
+00000f10: 2257 6520 6361 6e20 7361 7665 2074 6865  "We can save the
+00000f20: 2073 7469 7463 6865 6420 696d 6167 653a   stitched image:
+00000f30: 220a 2020 205d 0a20 207d 2c0a 2020 7b0a  ".   ].  },.  {.
+00000f40: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
+00000f50: 2263 6f64 6522 2c0a 2020 2022 6578 6563  "code",.   "exec
+00000f60: 7574 696f 6e5f 636f 756e 7422 3a20 6e75  ution_count": nu
+00000f70: 6c6c 2c0a 2020 2022 6d65 7461 6461 7461  ll,.   "metadata
+00000f80: 223a 207b 7d2c 0a20 2020 226f 7574 7075  ": {},.   "outpu
+00000f90: 7473 223a 205b 5d2c 0a20 2020 2273 6f75  ts": [],.   "sou
+00000fa0: 7263 6522 3a20 5b0a 2020 2020 226d 2e65  rce": [.    "m.e
+00000fb0: 7870 6f72 7428 776f 726b 202f 205c 2273  xport(work / \"s
+00000fc0: 7469 7463 6865 642e 7469 6666 5c22 2922  titched.tiff\")"
+00000fd0: 0a20 2020 5d0a 2020 7d2c 0a20 207b 0a20  .   ].  },.  {. 
+00000fe0: 2020 2263 656c 6c5f 7479 7065 223a 2022    "cell_type": "
+00000ff0: 6d61 726b 646f 776e 222c 0a20 2020 226d  markdown",.   "m
+00001000: 6574 6164 6174 6122 3a20 7b7d 2c0a 2020  etadata": {},.  
+00001010: 2022 736f 7572 6365 223a 205b 0a20 2020   "source": [.   
+00001020: 2022 5768 656e 2074 6865 2069 6d61 6765   "When the image
+00001030: 2068 6173 2062 6565 6e20 7374 6974 6368   has been stitch
+00001040: 6564 2028 7769 7468 206f 7220 7769 7468  ed (with or with
+00001050: 6f75 7420 6f70 7469 6d69 7a61 7469 6f6e  out optimization
+00001060: 292c 2077 6520 6361 6e20 6c6f 6f6b 2066  ), we can look f
+00001070: 6f72 2074 6865 2070 6f73 6974 696f 6e73  or the positions
+00001080: 206f 6620 7468 6520 6772 6964 2073 7175   of the grid squ
+00001090: 6172 6573 2f73 7175 6972 636c 6573 2e20  ares/squircles. 
+000010a0: 546f 2064 6f20 736f 2c20 6361 6c6c 2074  To do so, call t
+000010b0: 6865 206d 6574 686f 6420 602e 6669 6e64  he method `.find
+000010c0: 5f68 6f6c 6573 602e 2054 6865 2067 7269  _holes`. The gri
+000010d0: 6420 7371 7561 7265 7320 6172 6520 6964  d squares are id
+000010e0: 656e 7469 6669 6564 2061 7320 6f62 6a65  entified as obje
+000010f0: 6374 7320 726f 7567 686c 7920 7369 7a65  cts roughly size
+00001100: 6420 6064 6961 6d65 7465 7260 2077 6974  d `diameter` wit
+00001110: 6820 6120 746f 6c65 7261 6e63 6520 6f66  h a tolerance of
+00001120: 2031 3025 2e20 5468 6520 6d65 6469 616e   10%. The median
+00001130: 2061 7320 7765 6c6c 2061 7320 352f 3935   as well as 5/95
+00001140: 2070 6572 6365 6e74 696c 6573 2061 7265   percentiles are
+00001150: 2070 7269 6e74 6564 2074 6f20 6576 616c   printed to eval
+00001160: 7561 7465 2074 6865 2068 6f6c 6520 7369  uate the hole si
+00001170: 7a65 2064 6973 7472 6962 7574 696f 6e2e  ze distribution.
+00001180: 220a 2020 205d 0a20 207d 2c0a 2020 7b0a  ".   ].  },.  {.
+00001190: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
+000011a0: 2263 6f64 6522 2c0a 2020 2022 6578 6563  "code",.   "exec
+000011b0: 7574 696f 6e5f 636f 756e 7422 3a20 6e75  ution_count": nu
+000011c0: 6c6c 2c0a 2020 2022 6d65 7461 6461 7461  ll,.   "metadata
+000011d0: 223a 207b 7d2c 0a20 2020 226f 7574 7075  ": {},.   "outpu
+000011e0: 7473 223a 205b 5d2c 0a20 2020 2273 6f75  ts": [],.   "sou
+000011f0: 7263 6522 3a20 5b0a 2020 2020 2264 6961  rce": [.    "dia
+00001200: 6d65 7465 7220 3d20 3435 5f30 3030 2020  meter = 45_000  
+00001210: 2320 6e6d 5c6e 222c 0a20 2020 2022 7374  # nm\n",.    "st
+00001220: 6167 6563 6f6f 7264 732c 2069 6d61 6765  agecoords, image
+00001230: 636f 6f72 6473 203d 206d 2e66 696e 645f  coords = m.find_
+00001240: 686f 6c65 7328 706c 6f74 3d54 7275 652c  holes(plot=True,
+00001250: 2074 6f6c 6572 616e 6365 3d30 2e31 2922   tolerance=0.1)"
+00001260: 0a20 2020 5d0a 2020 7d2c 0a20 207b 0a20  .   ].  },.  {. 
+00001270: 2020 2263 656c 6c5f 7479 7065 223a 2022    "cell_type": "
+00001280: 6d61 726b 646f 776e 222c 0a20 2020 226d  markdown",.   "m
+00001290: 6574 6164 6174 6122 3a20 7b7d 2c0a 2020  etadata": {},.  
+000012a0: 2022 736f 7572 6365 223a 205b 0a20 2020   "source": [.   
+000012b0: 2022 4974 2069 7320 706f 7373 6962 6c65   "It is possible
+000012c0: 2074 6f20 6f70 7469 6d69 7a65 2074 6865   to optimize the
+000012d0: 2073 7461 6765 2063 6f6f 7264 696e 6174   stage coordinat
+000012e0: 6573 2066 6f72 206d 6f72 6520 6566 6669  es for more effi
+000012f0: 6369 656e 7420 6e61 7669 6761 7469 6f6e  cient navigation
+00001300: 2e20 496e 2074 6869 7320 6578 616d 706c  . In this exampl
+00001310: 652c 2074 6865 2074 6f74 616c 2073 7461  e, the total sta
+00001320: 6765 206d 6f76 656d 656e 7420 6361 6e20  ge movement can 
+00001330: 6265 2072 6564 7563 6564 2062 7920 6162  be reduced by ab
+00001340: 6f75 7420 3735 252c 2077 6869 6368 2077  out 75%, which w
+00001350: 696c 6c20 7361 7665 2061 206c 6f74 206f  ill save a lot o
+00001360: 6620 7469 6d65 2e20 5468 6520 6675 6e63  f time. The func
+00001370: 7469 6f6e 2075 7365 7320 7468 6520 5f74  tion uses the _t
+00001380: 776f 2d6f 7074 5f20 616c 676f 7269 7468  wo-opt_ algorith
+00001390: 6d20 666f 7220 6669 6e64 696e 6720 7468  m for finding th
+000013a0: 6520 7368 6f72 7465 7374 2070 6174 683a  e shortest path:
+000013b0: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
+000013c0: 7065 6469 612e 6f72 672f 7769 6b69 2f32  pedia.org/wiki/2
+000013d0: 2d6f 7074 2e22 0a20 2020 5d0a 2020 7d2c  -opt.".   ].  },
+000013e0: 0a20 207b 0a20 2020 2263 656c 6c5f 7479  .  {.   "cell_ty
+000013f0: 7065 223a 2022 636f 6465 222c 0a20 2020  pe": "code",.   
+00001400: 2265 7865 6375 7469 6f6e 5f63 6f75 6e74  "execution_count
+00001410: 223a 206e 756c 6c2c 0a20 2020 226d 6574  ": null,.   "met
+00001420: 6164 6174 6122 3a20 7b7d 2c0a 2020 2022  adata": {},.   "
+00001430: 6f75 7470 7574 7322 3a20 5b5d 2c0a 2020  outputs": [],.  
+00001440: 2022 736f 7572 6365 223a 205b 0a20 2020   "source": [.   
+00001450: 2022 6672 6f6d 2070 7973 6572 6961 6c65   "from pyseriale
+00001460: 6d2e 6e61 7669 6761 7469 6f6e 2069 6d70  m.navigation imp
+00001470: 6f72 7420 736f 7274 5f6e 6176 5f69 7465  ort sort_nav_ite
+00001480: 6d73 5f62 795f 7368 6f72 7465 7374 5f70  ms_by_shortest_p
+00001490: 6174 685c 6e22 2c0a 2020 2020 2273 7461  ath\n",.    "sta
+000014a0: 6765 636f 6f72 6473 203d 2073 6f72 745f  gecoords = sort_
+000014b0: 6e61 765f 6974 656d 735f 6279 5f73 686f  nav_items_by_sho
+000014c0: 7274 6573 745f 7061 7468 2873 7461 6765  rtest_path(stage
+000014d0: 636f 6f72 6473 2c20 706c 6f74 3d54 7275  coords, plot=Tru
+000014e0: 6529 3b22 0a20 2020 5d0a 2020 7d2c 0a20  e);".   ].  },. 
+000014f0: 207b 0a20 2020 2263 656c 6c5f 7479 7065   {.   "cell_type
+00001500: 223a 2022 6d61 726b 646f 776e 222c 0a20  ": "markdown",. 
+00001510: 2020 226d 6574 6164 6174 6122 3a20 7b7d    "metadata": {}
+00001520: 2c0a 2020 2022 736f 7572 6365 223a 205b  ,.   "source": [
+00001530: 0a20 2020 2022 5468 6520 6073 7461 6765  .    "The `stage
+00001540: 636f 6f72 6473 6020 6361 6e20 6265 2075  coords` can be u
+00001550: 7365 6420 746f 2073 6574 2075 7020 616e  sed to set up an
+00001560: 2061 7574 6f6d 6174 6564 202a 2a61 6371   automated **acq
+00001570: 7569 7265 2061 7420 6974 656d 732a 2a2e  uire at items**.
+00001580: 2054 6869 7320 6973 2075 7365 6675 6c20   This is useful 
+00001590: 746f 2074 616b 6520 6d65 6469 756d 206d  to take medium m
+000015a0: 6167 6e69 6669 6361 7469 6f6e 2069 6d61  agnification ima
+000015b0: 6765 7320 6672 6f6d 2074 6865 2072 6567  ges from the reg
+000015c0: 696f 6e73 206f 6620 696e 7465 7265 7374  ions of interest
+000015d0: 2c20 696e 206f 7572 2063 6173 652c 2074  , in our case, t
+000015e0: 6865 2067 7269 6420 7371 7561 7265 732e  he grid squares.
+000015f0: 2046 6972 7374 2c20 696e 6974 6961 6c69   First, initiali
+00001600: 7a65 2061 2063 6f6e 6e65 6374 696f 6e20  ze a connection 
+00001610: 746f 2074 6865 206d 6963 726f 7363 6f70  to the microscop
+00001620: 652e 220a 2020 205d 0a20 207d 2c0a 2020  e.".   ].  },.  
+00001630: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
+00001640: 3a20 2263 6f64 6522 2c0a 2020 2022 6578  : "code",.   "ex
+00001650: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
+00001660: 6e75 6c6c 2c0a 2020 2022 6d65 7461 6461  null,.   "metada
+00001670: 7461 223a 207b 7d2c 0a20 2020 226f 7574  ta": {},.   "out
+00001680: 7075 7473 223a 205b 5d2c 0a20 2020 2273  puts": [],.   "s
+00001690: 6f75 7263 6522 3a20 5b0a 2020 2020 2266  ource": [.    "f
+000016a0: 726f 6d20 696e 7374 616d 6174 6963 2069  rom instamatic i
+000016b0: 6d70 6f72 7420 5445 4d43 6f6e 7472 6f6c  mport TEMControl
+000016c0: 6c65 725c 6e22 2c0a 2020 2020 2263 7472  ler\n",.    "ctr
+000016d0: 6c20 3d20 5445 4d43 6f6e 7472 6f6c 6c65  l = TEMControlle
+000016e0: 722e 696e 6974 6961 6c69 7a65 2829 220a  r.initialize()".
+000016f0: 2020 205d 0a20 207d 2c0a 2020 7b0a 2020     ].  },.  {.  
+00001700: 2022 6365 6c6c 5f74 7970 6522 3a20 226d   "cell_type": "m
+00001710: 6172 6b64 6f77 6e22 2c0a 2020 2022 6d65  arkdown",.   "me
+00001720: 7461 6461 7461 223a 207b 7d2c 0a20 2020  tadata": {},.   
+00001730: 2273 6f75 7263 6522 3a20 5b0a 2020 2020  "source": [.    
+00001740: 224e 6578 742c 2077 6520 7368 6f75 6c64  "Next, we should
+00001750: 2073 6574 2075 7020 616e 2061 6371 7569   set up an acqui
+00001760: 7369 7469 6f6e 2066 756e 6374 696f 6e20  sition function 
+00001770: 666f 7220 6561 6368 2073 7461 6765 2070  for each stage p
+00001780: 6f73 6974 696f 6e2e 2054 6869 7320 7368  osition. This sh
+00001790: 6f75 6c64 3a5c 6e22 2c0a 2020 2020 225c  ould:\n",.    "\
+000017a0: 6e22 2c0a 2020 2020 2231 2e20 4365 6e74  n",.    "1. Cent
+000017b0: 6572 2074 6865 2067 7269 6420 7371 7561  er the grid squa
+000017c0: 7265 2062 7920 616c 6967 6e69 6e67 2069  re by aligning i
+000017d0: 7420 7769 7468 2061 2072 6566 6572 656e  t with a referen
+000017e0: 6365 2069 6d61 6765 5c6e 222c 0a20 2020  ce image\n",.   
+000017f0: 2022 322e 2054 616b 6520 616e 2069 6d61   "2. Take an ima
+00001800: 6765 2061 7420 6869 6768 206d 6167 5c6e  ge at high mag\n
+00001810: 222c 0a20 2020 2022 332e 2053 746f 7265  ",.    "3. Store
+00001820: 2074 6865 2069 6d61 6765 2061 6e64 2074   the image and t
+00001830: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
+00001840: 2073 7461 6765 2070 6f73 6974 696f 6e20   stage position 
+00001850: 696e 2061 2062 7566 6665 725c 6e22 2c0a  in a buffer\n",.
+00001860: 2020 2020 225c 6e22 2c0a 2020 2020 2249      "\n",.    "I
+00001870: 6e20 7468 6973 2070 7265 7061 7261 7469  n this preparati
+00001880: 6f6e 2073 7465 702c 2077 6520 6d75 6368  on step, we much
+00001890: 2066 6972 7374 206f 6274 6169 6e20 6120   first obtain a 
+000018a0: 7265 6665 7265 6e63 6520 696d 6167 6520  reference image 
+000018b0: 6672 6f6d 2061 2067 7269 6420 7371 7561  from a grid squa
+000018c0: 7265 2e20 5468 6520 6d61 676e 6966 6963  re. The magnific
+000018d0: 6174 696f 6e20 7368 6f75 6c64 2062 6520  ation should be 
+000018e0: 736f 2074 6861 7420 7468 6520 6772 6964  so that the grid
+000018f0: 2073 7175 6172 6520 6669 7473 2069 6e20   square fits in 
+00001900: 7468 6520 7669 6577 206f 6620 7468 6520  the view of the 
+00001910: 696d 6167 652e 2049 6e20 7468 6973 2065  image. In this e
+00001920: 7861 6d70 6c65 2c20 7765 2075 7365 2060  xample, we use `
+00001930: 3330 3078 6020 696e 2060 6c6f 776d 6167  300x` in `lowmag
+00001940: 602e 220a 2020 205d 0a20 207d 2c0a 2020  `.".   ].  },.  
+00001950: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
+00001960: 3a20 2263 6f64 6522 2c0a 2020 2022 6578  : "code",.   "ex
+00001970: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
+00001980: 6e75 6c6c 2c0a 2020 2022 6d65 7461 6461  null,.   "metada
+00001990: 7461 223a 207b 7d2c 0a20 2020 226f 7574  ta": {},.   "out
+000019a0: 7075 7473 223a 205b 5d2c 0a20 2020 2273  puts": [],.   "s
+000019b0: 6f75 7263 6522 3a20 5b0a 2020 2020 2269  ource": [.    "i
+000019c0: 6d70 6f72 7420 6d72 6366 696c 655c 6e22  mport mrcfile\n"
+000019d0: 2c0a 2020 2020 225c 6e22 2c0a 2020 2020  ,.    "\n",.    
+000019e0: 2223 2073 6574 206d 6963 726f 7363 6f70  "# set microscop
+000019f0: 6520 636f 6e64 6974 696f 6e73 5c6e 222c  e conditions\n",
+00001a00: 0a20 2020 2022 6374 726c 2e6d 6f64 652e  .    "ctrl.mode.
+00001a10: 7365 7428 276c 6f77 6d61 6727 295c 6e22  set('lowmag')\n"
+00001a20: 2c0a 2020 2020 2263 7472 6c2e 6d61 676e  ,.    "ctrl.magn
+00001a30: 6966 6963 6174 696f 6e2e 7661 6c75 6520  ification.value 
+00001a40: 3d20 3330 305c 6e22 2c0a 2020 2020 2262  = 300\n",.    "b
+00001a50: 696e 7369 7a65 203d 2034 5c6e 222c 0a20  insize = 4\n",. 
+00001a60: 2020 2022 5c6e 222c 0a20 2020 2022 2320     "\n",.    "# 
+00001a70: 7265 6665 7265 6e63 6520 696d 6167 6520  reference image 
+00001a80: 6f66 2061 2063 656e 7465 7265 6420 6772  of a centered gr
+00001a90: 6964 2073 7175 6172 655c 6e22 2c0a 2020  id square\n",.  
+00001aa0: 2020 2272 6566 5f69 6d67 203d 2063 7472    "ref_img = ctr
+00001ab0: 6c2e 6765 745f 7261 775f 696d 6167 6528  l.get_raw_image(
+00001ac0: 295c 6e22 2c0a 2020 2020 225c 6e22 2c0a  )\n",.    "\n",.
+00001ad0: 2020 2020 2266 203d 206d 7263 6669 6c65      "f = mrcfile
+00001ae0: 2e6e 6577 2877 6f72 6b20 2f20 2774 656d  .new(work / 'tem
+00001af0: 706c 6174 652e 6d72 6327 2c20 6461 7461  plate.mrc', data
+00001b00: 3d72 6566 5f69 6d67 2e61 7374 7970 6528  =ref_img.astype(
+00001b10: 6e70 2e69 6e74 3136 292c 206f 7665 7277  np.int16), overw
+00001b20: 7269 7465 3d54 7275 6529 5c6e 222c 0a20  rite=True)\n",. 
+00001b30: 2020 2022 662e 636c 6f73 6528 2922 0a20     "f.close()". 
+00001b40: 2020 5d0a 2020 7d2c 0a20 207b 0a20 2020    ].  },.  {.   
+00001b50: 2263 656c 6c5f 7479 7065 223a 2022 6d61  "cell_type": "ma
+00001b60: 726b 646f 776e 222c 0a20 2020 226d 6574  rkdown",.   "met
+00001b70: 6164 6174 6122 3a20 7b7d 2c0a 2020 2022  adata": {},.   "
+00001b80: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
+00001b90: 5468 656e 2c20 7765 2063 616e 2064 6566  Then, we can def
+00001ba0: 696e 6520 6f75 7220 6163 7175 6973 6974  ine our acquisit
+00001bb0: 696f 6e20 6675 6e63 7469 6f6e 2e20 5765  ion function. We
+00001bc0: 2077 696c 6c20 616c 6967 6e20 7468 6520   will align the 
+00001bd0: 7374 6167 6520 746f 2074 6865 2072 6566  stage to the ref
+00001be0: 6572 656e 6365 2069 6d61 6765 2075 7369  erence image usi
+00001bf0: 6e67 2063 726f 7373 2063 6f72 7265 6c61  ng cross correla
+00001c00: 7469 6f6e 2028 6063 7472 6c2e 616c 6967  tion (`ctrl.alig
+00001c10: 6e5f 746f 6029 2c20 616e 6420 7468 656e  n_to`), and then
+00001c20: 2074 616b 656e 2061 6e20 696d 6167 6520   taken an image 
+00001c30: 6f66 2074 6865 2063 656e 7465 7265 6420  of the centered 
+00001c40: 6772 6964 2073 7175 6172 652e 2041 6c74  grid square. Alt
+00001c50: 686f 7567 6820 7468 6973 2073 7465 7020  hough this step 
+00001c60: 6973 206f 7074 696f 6e61 6c2c 2069 7420  is optional, it 
+00001c70: 6d61 6b65 7320 7375 7265 2074 6861 7420  makes sure that 
+00001c80: 7468 6520 6772 6964 2073 7175 6172 6520  the grid square 
+00001c90: 6973 2063 656e 7465 7265 642e 2054 6869  is centered. Thi
+00001ca0: 7320 6865 6c70 7320 7768 656e 206c 6f6f  s helps when loo
+00001cb0: 6b69 6e67 2066 6f72 2070 6172 7469 636c  king for particl
+00001cc0: 6573 2c20 616e 6420 7265 6475 6365 7320  es, and reduces 
+00001cd0: 6572 726f 7273 2072 656c 6174 6564 2074  errors related t
+00001ce0: 6f20 7374 6167 6520 7472 616e 736c 6174  o stage translat
+00001cf0: 696f 6e20 616e 6420 6361 6c69 6272 6174  ion and calibrat
+00001d00: 696f 6e2e 2057 6520 616c 736f 2061 6371  ion. We also acq
+00001d10: 7569 7265 2061 6e20 696d 6167 6520 616e  uire an image an
+00001d20: 6420 7374 6f72 6520 7468 6520 6e65 7720  d store the new 
+00001d30: 7374 6167 6520 706f 7369 7469 6f6e 2074  stage position t
+00001d40: 6f20 6120 6275 6666 6572 2e22 0a20 2020  o a buffer.".   
+00001d50: 5d0a 2020 7d2c 0a20 207b 0a20 2020 2263  ].  },.  {.   "c
+00001d60: 656c 6c5f 7479 7065 223a 2022 636f 6465  ell_type": "code
+00001d70: 222c 0a20 2020 2265 7865 6375 7469 6f6e  ",.   "execution
+00001d80: 5f63 6f75 6e74 223a 206e 756c 6c2c 0a20  _count": null,. 
+00001d90: 2020 226d 6574 6164 6174 6122 3a20 7b7d    "metadata": {}
+00001da0: 2c0a 2020 2022 6f75 7470 7574 7322 3a20  ,.   "outputs": 
+00001db0: 5b5d 2c0a 2020 2022 736f 7572 6365 223a  [],.   "source":
+00001dc0: 205b 0a20 2020 2022 6275 6666 6572 203d   [.    "buffer =
+00001dd0: 205b 5d5c 6e22 2c0a 2020 2020 2273 7461   []\n",.    "sta
+00001de0: 6765 706f 7320 3d20 5b5d 5c6e 222c 0a20  gepos = []\n",. 
+00001df0: 2020 2022 5c6e 222c 0a20 2020 2022 5c6e     "\n",.    "\n
+00001e00: 222c 0a20 2020 2022 6465 6620 6163 7175  ",.    "def acqu
+00001e10: 6972 655f 6675 6e63 2863 7472 6c29 3a5c  ire_func(ctrl):\
+00001e20: 6e22 2c0a 2020 2020 2220 2020 2023 2041  n",.    "    # A
+00001e30: 6c69 676e 2074 6f20 7465 6d70 6c61 7465  lign to template
+00001e40: 5c6e 222c 0a20 2020 2022 2320 2020 2020  \n",.    "#     
+00001e50: 6374 726c 2e61 6c69 676e 5f74 6f28 7265  ctrl.align_to(re
+00001e60: 665f 696d 672c 2061 7070 6c79 3d54 7275  f_img, apply=Tru
+00001e70: 6529 5c6e 222c 0a20 2020 2022 2020 2020  e)\n",.    "    
+00001e80: 5c6e 222c 0a20 2020 2022 2020 2020 2320  \n",.    "    # 
+00001e90: 6f62 7461 696e 2069 6d61 6765 5c6e 222c  obtain image\n",
+00001ea0: 0a20 2020 2022 2020 2020 696d 672c 2068  .    "    img, h
+00001eb0: 203d 2063 7472 6c2e 6765 745f 696d 6167   = ctrl.get_imag
+00001ec0: 6528 6269 6e73 697a 653d 6269 6e73 697a  e(binsize=binsiz
+00001ed0: 6529 2020 5c6e 222c 0a20 2020 2022 2020  e)  \n",.    "  
+00001ee0: 2020 6275 6666 6572 2e61 7070 656e 6428    buffer.append(
+00001ef0: 696d 6729 5c6e 222c 0a20 2020 2022 2020  img)\n",.    "  
+00001f00: 2020 5c6e 222c 0a20 2020 2022 2020 2020    \n",.    "    
+00001f10: 2320 7374 6f72 6520 7374 6167 6520 706f  # store stage po
+00001f20: 7369 7469 6f6e 2061 6e64 2069 6d61 6765  sition and image
+00001f30: 2073 6f6d 6577 6865 7265 5c6e 222c 0a20   somewhere\n",. 
+00001f40: 2020 2022 2020 2020 706f 7320 3d20 6374     "    pos = ct
+00001f50: 726c 2e73 7461 6765 2e67 6574 2829 5c6e  rl.stage.get()\n
+00001f60: 222c 0a20 2020 2022 2020 2020 7374 6167  ",.    "    stag
+00001f70: 6570 6f73 2e61 7070 656e 6428 706f 7329  epos.append(pos)
+00001f80: 220a 2020 205d 0a20 207d 2c0a 2020 7b0a  ".   ].  },.  {.
+00001f90: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
+00001fa0: 226d 6172 6b64 6f77 6e22 2c0a 2020 2022  "markdown",.   "
+00001fb0: 6d65 7461 6461 7461 223a 207b 7d2c 0a20  metadata": {},. 
+00001fc0: 2020 2273 6f75 7263 6522 3a20 5b0a 2020    "source": [.  
+00001fd0: 2020 2257 6865 6e20 7468 6520 6675 6e63    "When the func
+00001fe0: 7469 6f6e 2069 7320 6465 6669 6e65 642c  tion is defined,
+00001ff0: 2077 6520 6361 6e20 7061 7373 2069 7420   we can pass it 
+00002000: 616e 6420 7468 6520 6c69 7374 206f 6620  and the list of 
+00002010: 6772 6964 2073 7175 6172 6520 7374 6167  grid square stag
+00002020: 6520 636f 6f72 6469 6e61 7465 7320 746f  e coordinates to
+00002030: 2074 6865 2066 756e 6374 696f 6e20 6063   the function `c
+00002040: 7472 6c2e 6163 7175 6972 655f 6174 5f69  trl.acquire_at_i
+00002050: 7465 6d73 602c 2077 6869 6368 2077 696c  tems`, which wil
+00002060: 6c20 6175 746f 6d61 7465 2074 6865 2066  l automate the f
+00002070: 756e 6374 696f 6e20 6174 2065 6163 6820  unction at each 
+00002080: 7374 6167 6520 706f 7369 7469 6f6e 2e22  stage position."
+00002090: 0a20 2020 5d0a 2020 7d2c 0a20 207b 0a20  .   ].  },.  {. 
+000020a0: 2020 2263 656c 6c5f 7479 7065 223a 2022    "cell_type": "
+000020b0: 636f 6465 222c 0a20 2020 2265 7865 6375  code",.   "execu
+000020c0: 7469 6f6e 5f63 6f75 6e74 223a 206e 756c  tion_count": nul
+000020d0: 6c2c 0a20 2020 226d 6574 6164 6174 6122  l,.   "metadata"
+000020e0: 3a20 7b7d 2c0a 2020 2022 6f75 7470 7574  : {},.   "output
+000020f0: 7322 3a20 5b5d 2c0a 2020 2022 736f 7572  s": [],.   "sour
+00002100: 6365 223a 205b 0a20 2020 2022 7365 6c20  ce": [.    "sel 
+00002110: 3d20 7374 6167 6563 6f6f 7264 735b 303a  = stagecoords[0:
+00002120: 3130 5d20 2023 2041 6371 7569 7265 2061  10]  # Acquire a
+00002130: 7420 7468 6520 6669 7273 7420 3130 2069  t the first 10 i
+00002140: 7465 6d73 5c6e 222c 0a20 2020 2022 6374  tems\n",.    "ct
+00002150: 726c 2e61 6371 7569 7265 5f61 745f 6974  rl.acquire_at_it
+00002160: 656d 7328 7365 6c2c 2061 6371 7569 7265  ems(sel, acquire
+00002170: 3d61 6371 7569 7265 5f66 756e 6329 220a  =acquire_func)".
+00002180: 2020 205d 0a20 207d 2c0a 2020 7b0a 2020     ].  },.  {.  
+00002190: 2022 6365 6c6c 5f74 7970 6522 3a20 226d   "cell_type": "m
+000021a0: 6172 6b64 6f77 6e22 2c0a 2020 2022 6d65  arkdown",.   "me
+000021b0: 7461 6461 7461 223a 207b 7d2c 0a20 2020  tadata": {},.   
+000021c0: 2273 6f75 7263 6522 3a20 5b0a 2020 2020  "source": [.    
+000021d0: 2248 6572 6520 6973 2061 206d 696e 696d  "Here is a minim
+000021e0: 616c 2065 7861 6d70 6c65 206f 6620 686f  al example of ho
+000021f0: 7720 7468 6520 6163 7175 6972 6520 6675  w the acquire fu
+00002200: 6e63 7469 6f6e 7320 6361 6e20 6265 2063  nctions can be c
+00002210: 6861 6e67 6564 2074 6f20 636f 6c6c 6563  hanged to collec
+00002220: 7420 6461 7461 2063 616e 2062 6520 7361  t data can be sa
+00002230: 7665 6420 746f 2061 2060 2e6e 6176 6020  ved to a `.nav` 
+00002240: 6669 6c65 2077 6869 6368 2063 616e 2062  file which can b
+00002250: 6520 7265 6164 2062 7920 6053 6572 6961  e read by `Seria
+00002260: 6c45 4d60 2e20 5c6e 222c 0a20 2020 2022  lEM`. \n",.    "
+00002270: 5c6e 222c 0a20 2020 2022 5468 6973 206d  \n",.    "This m
+00002280: 616b 6573 2075 7365 206f 6620 7468 6520  akes use of the 
+00002290: 6162 696c 6974 7920 746f 2070 6173 7320  ability to pass 
+000022a0: 6120 6070 6f73 745f 6163 7175 6972 6560  a `post_acquire`
+000022b0: 2066 756e 6374 696f 6e20 746f 2060 2e61   function to `.a
+000022c0: 6371 7569 7265 5f61 745f 6974 656d 7360  cquire_at_items`
+000022d0: 2e20 5468 6520 706f 7374 2061 6371 7569  . The post acqui
+000022e0: 7369 7469 6f6e 2063 616e 2062 6520 7573  sition can be us
+000022f0: 6564 2074 6f20 7361 7665 2074 6865 2069  ed to save the i
+00002300: 6d61 6765 7320 6173 2077 656c 6c20 6173  mages as well as
+00002310: 2074 6865 2072 6571 7569 7265 6420 6d65   the required me
+00002320: 7461 6461 7461 2074 6f20 6053 6572 6961  tadata to `Seria
+00002330: 6c45 4d60 2066 6f72 6d61 742c 206d 616b  lEM` format, mak
+00002340: 696e 6720 7573 6520 6f66 2074 6865 2060  ing use of the `
+00002350: 696e 7374 616d 6174 6963 2e73 6572 6961  instamatic.seria
+00002360: 6c65 6d60 206d 6f64 756c 652e 5c6e 222c  lem` module.\n",
+00002370: 0a20 2020 2022 5c6e 222c 0a20 2020 2022  .    "\n",.    "
+00002380: 5468 6520 6070 6f73 745f 6163 7175 6972  The `post_acquir
+00002390: 6560 2066 756e 6374 696f 6e20 7361 7665  e` function save
+000023a0: 7320 7468 6520 6461 7461 2074 6f20 602e  s the data to `.
+000023b0: 6d72 6360 2066 6f72 6d61 742c 2061 6e64  mrc` format, and
+000023c0: 2077 7269 7465 7320 616e 2069 6e70 7574   writes an input
+000023d0: 2066 696c 6520 666f 7220 5365 7269 616c   file for Serial
+000023e0: 454d 3a20 6069 6e73 7461 6d61 7469 632e  EM: `instamatic.
+000023f0: 6e61 7660 2e22 0a20 2020 5d0a 2020 7d2c  nav`.".   ].  },
+00002400: 0a20 207b 0a20 2020 2263 656c 6c5f 7479  .  {.   "cell_ty
+00002410: 7065 223a 2022 636f 6465 222c 0a20 2020  pe": "code",.   
+00002420: 2265 7865 6375 7469 6f6e 5f63 6f75 6e74  "execution_count
+00002430: 223a 206e 756c 6c2c 0a20 2020 226d 6574  ": null,.   "met
+00002440: 6164 6174 6122 3a20 7b7d 2c0a 2020 2022  adata": {},.   "
+00002450: 6f75 7470 7574 7322 3a20 5b5d 2c0a 2020  outputs": [],.  
+00002460: 2022 736f 7572 6365 223a 205b 0a20 2020   "source": [.   
+00002470: 2022 6672 6f6d 2070 7973 6572 6961 6c65   "from pyseriale
+00002480: 6d20 696d 706f 7274 204d 6170 4974 656d  m import MapItem
+00002490: 2c20 7772 6974 655f 6e61 765f 6669 6c65  , write_nav_file
+000024a0: 5c6e 222c 0a20 2020 2022 6672 6f6d 2069  \n",.    "from i
+000024b0: 6e73 7461 6d61 7469 6320 696d 706f 7274  nstamatic import
+000024c0: 2063 6f6e 6669 675c 6e22 2c0a 2020 2020   config\n",.    
+000024d0: 225c 6e22 2c0a 2020 2020 2223 2072 6566  "\n",.    "# ref
+000024e0: 6572 656e 6365 2069 6d61 6765 206f 6620  erence image of 
+000024f0: 6120 6365 6e74 6572 6564 2067 7269 6420  a centered grid 
+00002500: 7371 7561 7265 5c6e 222c 0a20 2020 2022  square\n",.    "
+00002510: 7265 665f 696d 6720 3d20 6374 726c 2e67  ref_img = ctrl.g
+00002520: 6574 5f72 6177 5f69 6d61 6765 2829 5c6e  et_raw_image()\n
+00002530: 222c 0a20 2020 2022 5c6e 222c 0a20 2020  ",.    "\n",.   
+00002540: 2022 6620 3d20 6d72 6366 696c 652e 6e65   "f = mrcfile.ne
+00002550: 7728 776f 726b 202f 205c 2274 656d 706c  w(work / \"templ
+00002560: 6174 652e 6d72 635c 222c 2064 6174 613d  ate.mrc\", data=
+00002570: 7265 665f 696d 672e 6173 7479 7065 286e  ref_img.astype(n
+00002580: 702e 696e 7431 3629 2c20 6f76 6572 7772  p.int16), overwr
+00002590: 6974 653d 5472 7565 295c 6e22 2c0a 2020  ite=True)\n",.  
+000025a0: 2020 2266 2e63 6c6f 7365 2829 5c6e 222c    "f.close()\n",
+000025b0: 0a20 2020 2022 5c6e 222c 0a20 2020 2022  .    "\n",.    "
+000025c0: 2320 656d 7074 7920 6275 6666 6572 735c  # empty buffers\
+000025d0: 6e22 2c0a 2020 2020 2262 7566 6665 7220  n",.    "buffer 
+000025e0: 3d20 5b5d 5c6e 222c 0a20 2020 2022 7374  = []\n",.    "st
+000025f0: 6167 6570 6f73 203d 205b 5d5c 6e22 2c0a  agepos = []\n",.
+00002600: 2020 2020 225c 6e22 2c0a 2020 2020 2220      "\n",.    " 
+00002610: 2020 5c6e 222c 0a20 2020 2022 6465 6620    \n",.    "def 
+00002620: 7772 6974 655f 6d72 635f 7374 6163 6b28  write_mrc_stack(
+00002630: 666e 3a73 7472 2c20 6461 7461 3a20 6c69  fn:str, data: li
+00002640: 7374 2c20 6f76 6572 7772 6974 653a 2062  st, overwrite: b
+00002650: 6f6f 6c3d 5472 7565 2c20 6d6d 6170 3a62  ool=True, mmap:b
+00002660: 6f6f 6c20 3d20 5472 7565 293a 5c6e 222c  ool = True):\n",
+00002670: 0a20 2020 2022 2020 2020 5c22 5c22 5c22  .    "    \"\"\"
+00002680: 5772 6974 6520 6120 7374 6163 6b20 6f66  Write a stack of
+00002690: 2069 6d61 6765 7320 746f 2061 6e20 6d72   images to an mr
+000026a0: 6320 6669 6c65 2e5c 225c 225c 225c 6e22  c file.\"\"\"\n"
+000026b0: 2c0a 2020 2020 2220 2020 2069 6620 6d6d  ,.    "    if mm
+000026c0: 6170 3a5c 6e22 2c0a 2020 2020 2220 2020  ap:\n",.    "   
+000026d0: 2020 2020 2073 6861 7065 203d 2028 6c65       shape = (le
+000026e0: 6e28 6275 6666 6572 292c 202a 6275 6666  n(buffer), *buff
+000026f0: 6572 5b30 5d2e 7368 6170 6529 5c6e 222c  er[0].shape)\n",
+00002700: 0a20 2020 2022 2020 2020 2020 2020 7769  .    "        wi
+00002710: 7468 206d 7263 6669 6c65 2e6e 6577 5f6d  th mrcfile.new_m
+00002720: 6d61 7028 666e 2c20 7368 6170 653d 7368  map(fn, shape=sh
+00002730: 6170 652c 206f 7665 7277 7269 7465 3d54  ape, overwrite=T
+00002740: 7275 652c 206d 7263 5f6d 6f64 653d 3129  rue, mrc_mode=1)
+00002750: 2061 7320 663a 5c6e 222c 0a20 2020 2022   as f:\n",.    "
+00002760: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002770: 692c 2069 6d20 696e 2065 6e75 6d65 7261  i, im in enumera
+00002780: 7465 2862 7566 6665 7229 3a5c 6e22 2c0a  te(buffer):\n",.
+00002790: 2020 2020 2220 2020 2020 2020 2020 2020      "           
+000027a0: 2020 2020 2066 2e64 6174 615b 695d 203d       f.data[i] =
+000027b0: 2069 6d5c 6e22 2c0a 2020 2020 2220 2020   im\n",.    "   
+000027c0: 2065 6c73 653a 5c6e 222c 0a20 2020 2022   else:\n",.    "
+000027d0: 2020 2020 2020 2020 6461 7461 203d 206e          data = n
+000027e0: 702e 6172 7261 7928 6461 7461 295c 6e22  p.array(data)\n"
+000027f0: 2c0a 2020 2020 2220 2020 2020 2020 2023  ,.    "        #
+00002800: 206d 7263 2063 616e 206f 6e6c 7920 6265   mrc can only be
+00002810: 2073 6176 6564 2061 7320 6120 3136 2d62   saved as a 16-b
+00002820: 6974 2069 6e74 6567 6572 5c6e 222c 0a20  it integer\n",. 
+00002830: 2020 2022 2020 2020 2020 2020 6461 7461     "        data
+00002840: 203d 2064 6174 612e 6173 7479 7065 286e   = data.astype(n
+00002850: 702e 696e 7431 3629 5c6e 222c 0a20 2020  p.int16)\n",.   
+00002860: 2022 2020 2020 2020 2020 7472 793a 5c6e   "        try:\n
+00002870: 222c 0a20 2020 2022 2020 2020 2020 2020  ",.    "        
+00002880: 2020 2020 6620 3d20 6d72 6366 696c 652e      f = mrcfile.
+00002890: 6e65 7728 666e 2c20 6461 7461 3d64 6174  new(fn, data=dat
+000028a0: 612c 206f 7665 7277 7269 7465 3d6f 7665  a, overwrite=ove
+000028b0: 7277 7269 7465 295c 6e22 2c0a 2020 2020  rwrite)\n",.    
+000028c0: 2220 2020 2020 2020 2065 7863 6570 7420  "        except 
+000028d0: 4f53 4572 726f 723a 5c6e 222c 0a20 2020  OSError:\n",.   
+000028e0: 2022 2020 2020 2020 2020 2020 2020 662e   "            f.
+000028f0: 636c 6f73 6528 295c 6e22 2c0a 2020 2020  close()\n",.    
+00002900: 2220 2020 205c 6e22 2c0a 2020 2020 225c  "    \n",.    "\
+00002910: 6e22 2c0a 2020 2020 2264 6566 2070 6f73  n",.    "def pos
+00002920: 745f 6163 7175 6972 6528 6374 726c 293a  t_acquire(ctrl):
+00002930: 5c6e 222c 0a20 2020 2022 2020 2020 666e  \n",.    "    fn
+00002940: 5f6e 6176 203d 2077 6f72 6b20 2f20 2769  _nav = work / 'i
+00002950: 6e73 7461 6d61 7469 632e 6e61 7627 5c6e  nstamatic.nav'\n
+00002960: 222c 0a20 2020 2022 2020 2020 666e 5f6d  ",.    "    fn_m
+00002970: 7263 203d 2077 6f72 6b20 2f20 276d 6d6d  rc = work / 'mmm
+00002980: 2e6d 7263 275c 6e22 2c0a 2020 2020 2220  .mrc'\n",.    " 
+00002990: 2020 205c 6e22 2c0a 2020 2020 2220 2020     \n",.    "   
+000029a0: 2077 7269 7465 5f6d 7263 5f73 7461 636b   write_mrc_stack
+000029b0: 2866 6e5f 6d72 632c 2062 7566 6665 7229  (fn_mrc, buffer)
+000029c0: 5c6e 222c 0a20 2020 2022 2020 2020 5c6e  \n",.    "    \n
+000029d0: 222c 0a20 2020 2022 2020 2020 6974 656d  ",.    "    item
+000029e0: 7320 3d20 5b5d 5c6e 222c 0a20 2020 2022  s = []\n",.    "
+000029f0: 2020 2020 5c6e 222c 0a20 2020 2022 2020      \n",.    "  
+00002a00: 2020 6d61 676e 6966 6963 6174 696f 6e20    magnification 
+00002a10: 3d20 6374 726c 2e6d 6167 6e69 6669 6361  = ctrl.magnifica
+00002a20: 7469 6f6e 2e76 616c 7565 5c6e 222c 0a20  tion.value\n",. 
+00002a30: 2020 2022 2020 2020 6d6f 6465 203d 2063     "    mode = c
+00002a40: 7472 6c2e 6d6f 6465 2e67 6574 2829 5c6e  trl.mode.get()\n
+00002a50: 222c 0a20 2020 2022 2020 2020 6d61 7073  ",.    "    maps
+00002a60: 6361 6c65 6d61 7420 3d20 636f 6e66 6967  calemat = config
+00002a70: 2e63 616c 6962 7261 7469 6f6e 5b6d 6f64  .calibration[mod
+00002a80: 655d 5b27 7374 6167 656d 6174 7269 7827  e]['stagematrix'
+00002a90: 5d5b 6d61 676e 6966 6963 6174 696f 6e5d  ][magnification]
+00002aa0: 5c6e 222c 0a20 2020 2022 2020 2020 6d61  \n",.    "    ma
+00002ab0: 7073 6361 6c65 6d61 7420 3d20 5b69 7465  pscalemat = [ite
+00002ac0: 6d2f 6269 6e73 697a 6520 666f 7220 6974  m/binsize for it
+00002ad0: 656d 2069 6e20 6d61 7073 6361 6c65 6d61  em in mapscalema
+00002ae0: 745d 5c6e 222c 0a20 2020 2022 2020 2020  t]\n",.    "    
+00002af0: 5c6e 222c 0a20 2020 2022 2020 2020 666f  \n",.    "    fo
+00002b00: 7220 692c 2069 6d61 6765 2069 6e20 656e  r i, image in en
+00002b10: 756d 6572 6174 6528 6275 6666 6572 293a  umerate(buffer):
+00002b20: 5c6e 222c 0a20 2020 2022 2020 2020 2020  \n",.    "      
+00002b30: 2020 782c 2079 2c20 7a2c 205f 2c20 5f20    x, y, z, _, _ 
+00002b40: 3d20 7374 6167 6570 6f73 5b69 5d5c 6e22  = stagepos[i]\n"
+00002b50: 2c0a 2020 2020 2220 2020 2020 2020 2073  ,.    "        s
+00002b60: 6861 7065 203d 2069 6d61 6765 2e73 6861  hape = image.sha
+00002b70: 7065 5c6e 222c 0a20 2020 2022 2020 2020  pe\n",.    "    
+00002b80: 2020 2020 2320 6269 6e73 697a 6520 3d20      # binsize = 
+00002b90: 6374 726c 2e63 616d 2e67 6574 4269 6e6e  ctrl.cam.getBinn
+00002ba0: 696e 6728 295c 6e22 2c0a 2020 2020 225c  ing()\n",.    "\
+00002bb0: 6e22 2c0a 2020 2020 2220 2020 2020 2020  n",.    "       
+00002bc0: 2064 203d 207b 7d5c 6e22 2c0a 2020 2020   d = {}\n",.    
+00002bd0: 2220 2020 2020 2020 2064 5b27 5374 6167  "        d['Stag
+00002be0: 6558 595a 275d 203d 2078 202f 2031 3030  eXYZ'] = x / 100
+00002bf0: 302c 2079 202f 2031 3030 302c 207a 202f  0, y / 1000, z /
+00002c00: 2031 3030 305c 6e22 2c0a 2020 2020 2220   1000\n",.    " 
+00002c10: 2020 2020 2020 2064 5b27 4d61 7046 696c         d['MapFil
+00002c20: 6527 5d20 3d20 666e 5f6d 7263 5c6e 222c  e'] = fn_mrc\n",
+00002c30: 0a20 2020 2022 2020 2020 2020 2020 645b  .    "        d[
+00002c40: 274d 6170 5365 6374 696f 6e27 5d20 3d20  'MapSection'] = 
+00002c50: 695c 6e22 2c0a 2020 2020 2220 2020 2020  i\n",.    "     
+00002c60: 2020 2064 5b27 4d61 7042 696e 6e69 6e67     d['MapBinning
+00002c70: 275d 203d 2062 696e 7369 7a65 5c6e 222c  '] = binsize\n",
+00002c80: 0a20 2020 2022 2020 2020 2020 2020 645b  .    "        d[
+00002c90: 274d 6170 4d61 6749 6e64 275d 203d 2063  'MapMagInd'] = c
+00002ca0: 7472 6c2e 6d61 676e 6966 6963 6174 696f  trl.magnificatio
+00002cb0: 6e2e 6162 736f 6c75 7465 5f69 6e64 6578  n.absolute_index
+00002cc0: 202b 2031 2020 2320 5365 7269 616c 454d   + 1  # SerialEM
+00002cd0: 2069 7320 312d 6261 7365 645c 6e22 2c0a   is 1-based\n",.
+00002ce0: 2020 2020 2220 2020 2020 2020 2064 5b27      "        d['
+00002cf0: 4d61 7053 6361 6c65 4d61 7427 5d20 3d20  MapScaleMat'] = 
+00002d00: 6d61 7073 6361 6c65 6d61 745c 6e22 2c0a  mapscalemat\n",.
+00002d10: 2020 2020 2220 2020 2020 2020 2064 5b27      "        d['
+00002d20: 4d61 7057 6964 7468 4865 6967 6874 275d  MapWidthHeight']
+00002d30: 203d 2073 6861 7065 5c6e 222c 0a20 2020   = shape\n",.   
+00002d40: 2022 5c6e 222c 0a20 2020 2022 2020 2020   "\n",.    "    
+00002d50: 2020 2020 6d61 705f 6974 656d 203d 204d      map_item = M
+00002d60: 6170 4974 656d 2e66 726f 6d5f 6469 6374  apItem.from_dict
+00002d70: 2864 295c 6e22 2c0a 2020 2020 2220 2020  (d)\n",.    "   
+00002d80: 2020 2020 2069 7465 6d73 2e61 7070 656e       items.appen
+00002d90: 6428 6d61 705f 6974 656d 295c 6e22 2c0a  d(map_item)\n",.
+00002da0: 2020 2020 225c 6e22 2c0a 2020 2020 2220      "\n",.    " 
+00002db0: 2020 2077 7269 7465 5f6e 6176 5f66 696c     write_nav_fil
+00002dc0: 6528 666e 5f6e 6176 2c20 2a69 7465 6d73  e(fn_nav, *items
+00002dd0: 295c 6e22 2c0a 2020 2020 2220 2020 205c  )\n",.    "    \
+00002de0: 6e22 2c0a 2020 2020 2220 2020 2070 7269  n",.    "    pri
+00002df0: 6e74 2866 5c22 4461 7461 2073 6176 6564  nt(f\"Data saved
+00002e00: 2074 6f20 607b 666e 5f6e 6176 7d60 2061   to `{fn_nav}` a
+00002e10: 6e64 2060 7b66 6e5f 6d72 637d 6020 287b  nd `{fn_mrc}` ({
+00002e20: 6c65 6e28 6275 6666 6572 297d 2069 6d61  len(buffer)} ima
+00002e30: 6765 7329 5c22 2922 0a20 2020 5d0a 2020  ges)\")".   ].  
+00002e40: 7d2c 0a20 207b 0a20 2020 2263 656c 6c5f  },.  {.   "cell_
+00002e50: 7479 7065 223a 2022 6d61 726b 646f 776e  type": "markdown
+00002e60: 222c 0a20 2020 226d 6574 6164 6174 6122  ",.   "metadata"
+00002e70: 3a20 7b7d 2c0a 2020 2022 736f 7572 6365  : {},.   "source
+00002e80: 223a 205b 0a20 2020 2022 4e65 7874 2077  ": [.    "Next w
+00002e90: 6520 6361 6c6c 2060 6374 726c 2e61 6371  e call `ctrl.acq
+00002ea0: 7569 7265 5f61 745f 6974 656d 7360 2061  uire_at_items` a
+00002eb0: 7320 6265 666f 7265 2077 6974 6820 7468  s before with th
+00002ec0: 6520 6e65 7720 6070 6f73 745f 6163 7175  e new `post_acqu
+00002ed0: 6972 6560 2066 756e 6374 696f 6e2e 220a  ire` function.".
+00002ee0: 2020 205d 0a20 207d 2c0a 2020 7b0a 2020     ].  },.  {.  
+00002ef0: 2022 6365 6c6c 5f74 7970 6522 3a20 2263   "cell_type": "c
+00002f00: 6f64 6522 2c0a 2020 2022 6578 6563 7574  ode",.   "execut
+00002f10: 696f 6e5f 636f 756e 7422 3a20 6e75 6c6c  ion_count": null
+00002f20: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
+00002f30: 207b 7d2c 0a20 2020 226f 7574 7075 7473   {},.   "outputs
+00002f40: 223a 205b 5d2c 0a20 2020 2273 6f75 7263  ": [],.   "sourc
+00002f50: 6522 3a20 5b0a 2020 2020 2273 656c 203d  e": [.    "sel =
+00002f60: 2073 7461 6765 636f 6f72 6473 5b30 3a31   stagecoords[0:1
+00002f70: 305d 2020 2320 4163 7175 6972 6520 6174  0]  # Acquire at
+00002f80: 2074 6865 2066 6972 7374 2031 3020 6974   the first 10 it
+00002f90: 656d 735c 6e22 2c0a 2020 2020 2263 7472  ems\n",.    "ctr
+00002fa0: 6c2e 6163 7175 6972 655f 6174 5f69 7465  l.acquire_at_ite
+00002fb0: 6d73 2873 656c 2c20 5c6e 222c 0a20 2020  ms(sel, \n",.   
+00002fc0: 2022 2020 2020 2020 2020 2020 2020 2020   "              
+00002fd0: 2020 2020 2020 2020 6163 7175 6972 653d          acquire=
+00002fe0: 6163 7175 6972 655f 6675 6e63 2c20 5c6e  acquire_func, \n
+00002ff0: 222c 0a20 2020 2022 2020 2020 2020 2020  ",.    "        
+00003000: 2020 2020 2020 2020 2020 2020 2020 706f                po
+00003010: 7374 5f61 6371 7569 7265 3d70 6f73 745f  st_acquire=post_
+00003020: 6163 7175 6972 6529 220a 2020 205d 0a20  acquire)".   ]. 
+00003030: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
+00003040: 5f74 7970 6522 3a20 226d 6172 6b64 6f77  _type": "markdow
+00003050: 6e22 2c0a 2020 2022 6d65 7461 6461 7461  n",.   "metadata
+00003060: 223a 207b 7d2c 0a20 2020 2273 6f75 7263  ": {},.   "sourc
+00003070: 6522 3a20 5b0a 2020 2020 224e 6f77 206c  e": [.    "Now l
+00003080: 6f61 6420 7570 2074 6865 2060 696e 7374  oad up the `inst
+00003090: 616d 6174 6963 2e6e 6176 6020 6669 6c65  amatic.nav` file
+000030a0: 2069 6e20 6053 6572 6961 6c45 4d60 2074   in `SerialEM` t
+000030b0: 6f20 7365 6520 7468 6520 7265 7375 6c74  o see the result
+000030c0: 2122 0a20 2020 5d0a 2020 7d2c 0a20 207b  !".   ].  },.  {
+000030d0: 0a20 2020 2263 656c 6c5f 7479 7065 223a  .   "cell_type":
+000030e0: 2022 636f 6465 222c 0a20 2020 2265 7865   "code",.   "exe
+000030f0: 6375 7469 6f6e 5f63 6f75 6e74 223a 206e  cution_count": n
+00003100: 756c 6c2c 0a20 2020 226d 6574 6164 6174  ull,.   "metadat
+00003110: 6122 3a20 7b7d 2c0a 2020 2022 6f75 7470  a": {},.   "outp
+00003120: 7574 7322 3a20 5b5d 2c0a 2020 2022 736f  uts": [],.   "so
+00003130: 7572 6365 223a 205b 5d0a 2020 7d2c 0a20  urce": [].  },. 
+00003140: 207b 0a20 2020 2263 656c 6c5f 7479 7065   {.   "cell_type
+00003150: 223a 2022 636f 6465 222c 0a20 2020 2265  ": "code",.   "e
+00003160: 7865 6375 7469 6f6e 5f63 6f75 6e74 223a  xecution_count":
+00003170: 206e 756c 6c2c 0a20 2020 226d 6574 6164   null,.   "metad
+00003180: 6174 6122 3a20 7b7d 2c0a 2020 2022 6f75  ata": {},.   "ou
+00003190: 7470 7574 7322 3a20 5b5d 2c0a 2020 2022  tputs": [],.   "
+000031a0: 736f 7572 6365 223a 205b 5d0a 2020 7d0a  source": [].  }.
+000031b0: 205d 2c0a 2022 6d65 7461 6461 7461 223a   ],. "metadata":
+000031c0: 207b 0a20 2022 6b65 726e 656c 7370 6563   {.  "kernelspec
+000031d0: 223a 207b 0a20 2020 2264 6973 706c 6179  ": {.   "display
+000031e0: 5f6e 616d 6522 3a20 2250 7974 686f 6e20  _name": "Python 
+000031f0: 3322 2c0a 2020 2022 6c61 6e67 7561 6765  3",.   "language
+00003200: 223a 2022 7079 7468 6f6e 222c 0a20 2020  ": "python",.   
+00003210: 226e 616d 6522 3a20 2270 7974 686f 6e33  "name": "python3
+00003220: 220a 2020 7d2c 0a20 2022 6c61 6e67 7561  ".  },.  "langua
+00003230: 6765 5f69 6e66 6f22 3a20 7b0a 2020 2022  ge_info": {.   "
+00003240: 636f 6465 6d69 7272 6f72 5f6d 6f64 6522  codemirror_mode"
+00003250: 3a20 7b0a 2020 2020 226e 616d 6522 3a20  : {.    "name": 
+00003260: 2269 7079 7468 6f6e 222c 0a20 2020 2022  "ipython",.    "
+00003270: 7665 7273 696f 6e22 3a20 330a 2020 207d  version": 3.   }
+00003280: 2c0a 2020 2022 6669 6c65 5f65 7874 656e  ,.   "file_exten
+00003290: 7369 6f6e 223a 2022 2e70 7922 2c0a 2020  sion": ".py",.  
+000032a0: 2022 6d69 6d65 7479 7065 223a 2022 7465   "mimetype": "te
+000032b0: 7874 2f78 2d70 7974 686f 6e22 2c0a 2020  xt/x-python",.  
+000032c0: 2022 6e61 6d65 223a 2022 7079 7468 6f6e   "name": "python
+000032d0: 222c 0a20 2020 226e 6263 6f6e 7665 7274  ",.   "nbconvert
+000032e0: 5f65 7870 6f72 7465 7222 3a20 2270 7974  _exporter": "pyt
+000032f0: 686f 6e22 2c0a 2020 2022 7079 676d 656e  hon",.   "pygmen
+00003300: 7473 5f6c 6578 6572 223a 2022 6970 7974  ts_lexer": "ipyt
+00003310: 686f 6e33 222c 0a20 2020 2276 6572 7369  hon3",.   "versi
+00003320: 6f6e 223a 2022 332e 382e 3322 0a20 207d  on": "3.8.3".  }
+00003330: 0a20 7d2c 0a20 226e 6266 6f72 6d61 7422  . },. "nbformat"
+00003340: 3a20 342c 0a20 226e 6266 6f72 6d61 745f  : 4,. "nbformat_
+00003350: 6d69 6e6f 7222 3a20 320a 7d0a            minor": 2.}.
```

### Comparing `instamatic-1.8.0/scripts/browser.py` & `instamatic-1.9.0/scripts/browser.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,262 +1,262 @@
-import argparse
-import glob
-import os
-import sys
-from pathlib import Path
-
-import matplotlib
-import matplotlib.pyplot as plt
-import numpy as np
-from scipy import ndimage
-from tqdm.auto import tqdm
-
-from instamatic import neural_network
-from instamatic.formats import *
-
-CMAP = 'gray'  # "viridis", "gray"
-
-ANGLE = -0.88 + np.pi / 2
-R = np.array([
-    [np.cos(ANGLE), -np.sin(ANGLE)],
-    [np.sin(ANGLE), np.cos(ANGLE)]])
-
-
-def get_stage_coords(fns, return_ims=False):
-    coords = []
-    has_crystals = []
-    t = tqdm(fns, desc='Parsing files')
-
-    imgs = []
-
-    for fn in t:
-        img, h = read_image(fn)
-        try:
-            dx, dy = h['exp_hole_offset']
-            cx, cy = h['exp_hole_center']
-        except KeyError:
-            dx, dy = h['exp_scan_offset']
-            cx, cy = h['exp_scan_center']
-        coords.append((cx + dx, cy + dy))
-
-        has_crystals.append(len(h['exp_crystal_coords']) > 0)
-        if return_ims:
-            img = ndimage.zoom(img, 0.0969)
-            imgs.append(img)
-    # convert to um
-
-    return np.array(coords) / 1000, np.array(has_crystals), imgs
-
-
-def lst2colormap(lst):
-    """Turn list of values into matplotlib colormap
-    http://stackoverflow.com/a/26552429."""
-    n = matplotlib.colors.Normalize(vmin=min(lst), vmax=max(lst))
-    m = matplotlib.cm.ScalarMappable(norm=n)
-    colormap = m.to_rgba(lst)
-    return colormap
-
-
-def run(filepat='images/image_*.tiff', results=None, stitch=False):
-    # use relpath to normalizes path
-    fns = [Path(fn).absolute() for fn in glob.glob(filepat)]
-
-    if len(fns) == 0:
-        sys.exit()
-
-    if stitch:
-        coord_color = 'none'
-    else:
-        coord_color = 'red'
-    picked_color = 'blue'
-
-    if results:
-        df, d = read_ycsv(results)
-        df.index = df.index.map(os.path.relpath)
-        if isinstance(d['cell'], (tuple, list)):
-            pixelsize = d['experiment']['pixelsize']
-            indexer = IndexerMulti.from_cells(d['cell'], pixelsize=pixelsize, **d['projections'])
-        else:
-            projector = Projector.from_parameters(thickness=d['projections']['thickness'], **d['cell'])
-            indexer = Indexer.from_projector(projector, pixelsize=d['experiment']['pixelsize'])
-
-    coords, has_crystals, imgs = get_stage_coords(fns, return_ims=stitch)
-
-    fn = fns[0]
-    img, h = read_image(fn)
-    imdim_x, imdim_y = np.array(h['ImageDimensions']) / 2
-
-    fig = plt.figure()
-    fig.canvas.set_window_title('instamatic.browser')
-
-    ax1 = plt.subplot(131, title='Stage map', aspect='equal')
-    # plt_coords, = ax1.plot(coords[:,0], coords[:,1], marker="+", picker=8, c=has_crystals)
-
-    coords = np.dot(coords, R)
-
-    if stitch:
-        for mini_img, coord in zip(imgs, coords):
-            sx, sy = coord
-            ax1.imshow(mini_img, interpolation='bilinear', extent=[sx - imdim_x, sx + imdim_x, sy - imdim_y, sy + imdim_y], cmap=CMAP)
-
-    ax1.scatter(coords[has_crystals, 0], coords[has_crystals, 1], marker='o', facecolor=coord_color)
-    ax1.scatter(coords[:, 0], coords[:, 1], marker='.', color=coord_color, picker=8)
-    highlight1, = ax1.plot([], [], marker='o', color=picked_color)
-
-    ax1.set_xlabel('Stage X')
-    ax1.set_ylabel('Stage Y')
-
-    ax2 = plt.subplot(132, title=f'{fn}\nx={0}, y={0}')
-    im2 = ax2.imshow(img, cmap=CMAP, vmax=np.percentile(img, 99.5))
-    plt_crystals, = ax2.plot([], [], marker='+', color='red', mew=2, picker=8, lw=0)
-    highlight2, = ax2.plot([], [], marker='+', color='blue', mew=2)
-
-    ax3 = plt.subplot(133, title='Diffraction pattern')
-    im3 = ax3.imshow(np.zeros_like(img), vmax=np.percentile(img, 99.5), cmap=CMAP)
-
-    class plt_diff:
-        center, = ax3.plot([], [], 'o', color='red', lw=0)
-        data = None
-
-    def onclick(event):
-        axes = event.artist.axes
-        ind = event.ind[0]
-
-        if axes == ax1:
-            fn = fns[ind]
-            ax2.texts = []
-
-            img, h = read_image(fn)
-            # img = np.rot90(img, k=3)
-            im2.set_data(img)
-            im2.set_clim(vmax=np.percentile(img, 99.5))
-
-            stage_x, stage_y = h.get('exp_stage_position', (0, 0))
-            ax2.set_xlabel('x={stage_x:.0f} y={stage_y:.0f}')
-            ax2.set_title(fn)
-            crystal_coords = np.array(h['exp_crystal_coords'])
-
-            if results:
-                crystal_fns = [fn.parents[1] / 'data' / f'{fn.stem}_{i:04d}{fn.suffix}' for i in range(len(crystal_coords))]
-                df.ix[crystal_fns]
-
-                for coord, crystal_fn in zip(crystal_coords, crystal_fns):
-                    try:
-                        phase, score = df.ix[crystal_fn, 'phase'], df.ix[crystal_fn, 'score']
-
-                    except KeyError:  # if crystal_fn not in df.index
-                        pass
-                    else:
-                        if score > 10:
-                            text = f' {phase}\n {score:.0f}'
-                            ax2.text(coord[1], coord[0], text)
-
-            if len(crystal_coords) > 0:
-                plt_crystals.set_xdata(crystal_coords[:, 1])
-                plt_crystals.set_ydata(crystal_coords[:, 0])
-            else:
-                plt_crystals.set_xdata([])
-                plt_crystals.set_ydata([])
-
-            highlight1.set_xdata(coords[ind, 0])
-            highlight1.set_ydata(coords[ind, 1])
-
-            highlight2.set_xdata([])
-            highlight2.set_ydata([])
-
-            if len(crystal_coords) > 0:
-                # to preload next diffraction pattern
-                axes = ax2
-                ind = 0
-
-        if axes == ax2:
-            fn = Path(ax2.get_title())
-            fn_diff = fn.parents[1] / 'data' / f'{fn.stem}_{ind:04d}{fn.suffix}'
-
-            img, h = read_image(fn_diff)
-
-            img_processed = neural_network.preprocess(img.astype(float))
-            quality = neural_network.predict(img_processed)
-            ax3.set_xlabel(f'Crystal quality: {quality:.2%}')
-
-            im3.set_data(img)
-            im3.set_clim(vmax=np.percentile(img, 99.5))
-            ax3.set_title(fn_diff)
-
-            highlight2.set_xdata(plt_crystals.get_xdata()[ind])
-            highlight2.set_ydata(plt_crystals.get_ydata()[ind])
-
-            if results:
-                if plt_diff.data:
-                    plt_diff.data.remove()
-                    plt_diff.data = None
-
-                try:
-                    r = df.ix[fn_diff]
-                except KeyError:
-                    plt_diff.center.set_xdata([])
-                    plt_diff.center.set_ydata([])
-                else:
-                    print()
-                    print(r)
-                    proj = indexer.get_projection(r)
-                    pks = proj[:, 3:5]
-
-                    i, j, proj = get_indices(pks, r.scale, (r.center_x, r.center_y), img.shape, hkl=proj)
-                    shape_vector = proj[:, 5]
-
-                    plt_diff.center.set_xdata(r.center_y)
-                    plt_diff.center.set_ydata(r.center_x)
-
-                    plt_diff.data = ax3.scatter(j, i, c=shape_vector, marker='+')
-
-        if axes == ax3:
-            pass
-
-        fig.canvas.draw()
-
-    fig.canvas.mpl_connect('pick_event', onclick)
-
-    plt.show()
-
-
-def main():
-    description = """
-Program for indexing electron diffraction images.
-
-Example:
-
-    instamatic.browser images/*.tiff -r results.csv
-"""
-
-    parser = argparse.ArgumentParser(
-        description=description,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-
-    parser.add_argument('args',
-                        type=str, metavar='FILE', nargs='?',
-                        help='File pattern to image files')
-
-    parser.add_argument('-s', '--stitch',
-                        action='store_true', dest='stitch',
-                        help='Stitch images together.')
-
-    parser.set_defaults(results=None,
-                        stitch=False,
-                        )
-
-    options = parser.parse_args()
-    arg = options.args
-
-    if not arg:
-        if os.path.exists('images'):
-            arg = 'images/*.h5'
-        else:
-            parser.print_help()
-            sys.exit()
-
-    run(filepat=arg, results=options.results, stitch=options.stitch)
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+import glob
+import os
+import sys
+from pathlib import Path
+
+import matplotlib
+import matplotlib.pyplot as plt
+import numpy as np
+from scipy import ndimage
+from tqdm.auto import tqdm
+
+from instamatic import neural_network
+from instamatic.formats import *
+
+CMAP = 'gray'  # "viridis", "gray"
+
+ANGLE = -0.88 + np.pi / 2
+R = np.array([
+    [np.cos(ANGLE), -np.sin(ANGLE)],
+    [np.sin(ANGLE), np.cos(ANGLE)]])
+
+
+def get_stage_coords(fns, return_ims=False):
+    coords = []
+    has_crystals = []
+    t = tqdm(fns, desc='Parsing files')
+
+    imgs = []
+
+    for fn in t:
+        img, h = read_image(fn)
+        try:
+            dx, dy = h['exp_hole_offset']
+            cx, cy = h['exp_hole_center']
+        except KeyError:
+            dx, dy = h['exp_scan_offset']
+            cx, cy = h['exp_scan_center']
+        coords.append((cx + dx, cy + dy))
+
+        has_crystals.append(len(h['exp_crystal_coords']) > 0)
+        if return_ims:
+            img = ndimage.zoom(img, 0.0969)
+            imgs.append(img)
+    # convert to um
+
+    return np.array(coords) / 1000, np.array(has_crystals), imgs
+
+
+def lst2colormap(lst):
+    """Turn list of values into matplotlib colormap
+    http://stackoverflow.com/a/26552429."""
+    n = matplotlib.colors.Normalize(vmin=min(lst), vmax=max(lst))
+    m = matplotlib.cm.ScalarMappable(norm=n)
+    colormap = m.to_rgba(lst)
+    return colormap
+
+
+def run(filepat='images/image_*.tiff', results=None, stitch=False):
+    # use relpath to normalizes path
+    fns = [Path(fn).absolute() for fn in glob.glob(filepat)]
+
+    if len(fns) == 0:
+        sys.exit()
+
+    if stitch:
+        coord_color = 'none'
+    else:
+        coord_color = 'red'
+    picked_color = 'blue'
+
+    if results:
+        df, d = read_ycsv(results)
+        df.index = df.index.map(os.path.relpath)
+        if isinstance(d['cell'], (tuple, list)):
+            pixelsize = d['experiment']['pixelsize']
+            indexer = IndexerMulti.from_cells(d['cell'], pixelsize=pixelsize, **d['projections'])
+        else:
+            projector = Projector.from_parameters(thickness=d['projections']['thickness'], **d['cell'])
+            indexer = Indexer.from_projector(projector, pixelsize=d['experiment']['pixelsize'])
+
+    coords, has_crystals, imgs = get_stage_coords(fns, return_ims=stitch)
+
+    fn = fns[0]
+    img, h = read_image(fn)
+    imdim_x, imdim_y = np.array(h['ImageDimensions']) / 2
+
+    fig = plt.figure()
+    fig.canvas.set_window_title('instamatic.browser')
+
+    ax1 = plt.subplot(131, title='Stage map', aspect='equal')
+    # plt_coords, = ax1.plot(coords[:,0], coords[:,1], marker="+", picker=8, c=has_crystals)
+
+    coords = np.dot(coords, R)
+
+    if stitch:
+        for mini_img, coord in zip(imgs, coords):
+            sx, sy = coord
+            ax1.imshow(mini_img, interpolation='bilinear', extent=[sx - imdim_x, sx + imdim_x, sy - imdim_y, sy + imdim_y], cmap=CMAP)
+
+    ax1.scatter(coords[has_crystals, 0], coords[has_crystals, 1], marker='o', facecolor=coord_color)
+    ax1.scatter(coords[:, 0], coords[:, 1], marker='.', color=coord_color, picker=8)
+    highlight1, = ax1.plot([], [], marker='o', color=picked_color)
+
+    ax1.set_xlabel('Stage X')
+    ax1.set_ylabel('Stage Y')
+
+    ax2 = plt.subplot(132, title=f'{fn}\nx={0}, y={0}')
+    im2 = ax2.imshow(img, cmap=CMAP, vmax=np.percentile(img, 99.5))
+    plt_crystals, = ax2.plot([], [], marker='+', color='red', mew=2, picker=8, lw=0)
+    highlight2, = ax2.plot([], [], marker='+', color='blue', mew=2)
+
+    ax3 = plt.subplot(133, title='Diffraction pattern')
+    im3 = ax3.imshow(np.zeros_like(img), vmax=np.percentile(img, 99.5), cmap=CMAP)
+
+    class plt_diff:
+        center, = ax3.plot([], [], 'o', color='red', lw=0)
+        data = None
+
+    def onclick(event):
+        axes = event.artist.axes
+        ind = event.ind[0]
+
+        if axes == ax1:
+            fn = fns[ind]
+            ax2.texts = []
+
+            img, h = read_image(fn)
+            # img = np.rot90(img, k=3)
+            im2.set_data(img)
+            im2.set_clim(vmax=np.percentile(img, 99.5))
+
+            stage_x, stage_y = h.get('exp_stage_position', (0, 0))
+            ax2.set_xlabel('x={stage_x:.0f} y={stage_y:.0f}')
+            ax2.set_title(fn)
+            crystal_coords = np.array(h['exp_crystal_coords'])
+
+            if results:
+                crystal_fns = [fn.parents[1] / 'data' / f'{fn.stem}_{i:04d}{fn.suffix}' for i in range(len(crystal_coords))]
+                df.ix[crystal_fns]
+
+                for coord, crystal_fn in zip(crystal_coords, crystal_fns):
+                    try:
+                        phase, score = df.ix[crystal_fn, 'phase'], df.ix[crystal_fn, 'score']
+
+                    except KeyError:  # if crystal_fn not in df.index
+                        pass
+                    else:
+                        if score > 10:
+                            text = f' {phase}\n {score:.0f}'
+                            ax2.text(coord[1], coord[0], text)
+
+            if len(crystal_coords) > 0:
+                plt_crystals.set_xdata(crystal_coords[:, 1])
+                plt_crystals.set_ydata(crystal_coords[:, 0])
+            else:
+                plt_crystals.set_xdata([])
+                plt_crystals.set_ydata([])
+
+            highlight1.set_xdata(coords[ind, 0])
+            highlight1.set_ydata(coords[ind, 1])
+
+            highlight2.set_xdata([])
+            highlight2.set_ydata([])
+
+            if len(crystal_coords) > 0:
+                # to preload next diffraction pattern
+                axes = ax2
+                ind = 0
+
+        if axes == ax2:
+            fn = Path(ax2.get_title())
+            fn_diff = fn.parents[1] / 'data' / f'{fn.stem}_{ind:04d}{fn.suffix}'
+
+            img, h = read_image(fn_diff)
+
+            img_processed = neural_network.preprocess(img.astype(float))
+            quality = neural_network.predict(img_processed)
+            ax3.set_xlabel(f'Crystal quality: {quality:.2%}')
+
+            im3.set_data(img)
+            im3.set_clim(vmax=np.percentile(img, 99.5))
+            ax3.set_title(fn_diff)
+
+            highlight2.set_xdata(plt_crystals.get_xdata()[ind])
+            highlight2.set_ydata(plt_crystals.get_ydata()[ind])
+
+            if results:
+                if plt_diff.data:
+                    plt_diff.data.remove()
+                    plt_diff.data = None
+
+                try:
+                    r = df.ix[fn_diff]
+                except KeyError:
+                    plt_diff.center.set_xdata([])
+                    plt_diff.center.set_ydata([])
+                else:
+                    print()
+                    print(r)
+                    proj = indexer.get_projection(r)
+                    pks = proj[:, 3:5]
+
+                    i, j, proj = get_indices(pks, r.scale, (r.center_x, r.center_y), img.shape, hkl=proj)
+                    shape_vector = proj[:, 5]
+
+                    plt_diff.center.set_xdata(r.center_y)
+                    plt_diff.center.set_ydata(r.center_x)
+
+                    plt_diff.data = ax3.scatter(j, i, c=shape_vector, marker='+')
+
+        if axes == ax3:
+            pass
+
+        fig.canvas.draw()
+
+    fig.canvas.mpl_connect('pick_event', onclick)
+
+    plt.show()
+
+
+def main():
+    description = """
+Program for indexing electron diffraction images.
+
+Example:
+
+    instamatic.browser images/*.tiff -r results.csv
+"""
+
+    parser = argparse.ArgumentParser(
+        description=description,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+
+    parser.add_argument('args',
+                        type=str, metavar='FILE', nargs='?',
+                        help='File pattern to image files')
+
+    parser.add_argument('-s', '--stitch',
+                        action='store_true', dest='stitch',
+                        help='Stitch images together.')
+
+    parser.set_defaults(results=None,
+                        stitch=False,
+                        )
+
+    options = parser.parse_args()
+    arg = options.args
+
+    if not arg:
+        if os.path.exists('images'):
+            arg = 'images/*.h5'
+        else:
+            parser.print_help()
+            sys.exit()
+
+    run(filepat=arg, results=options.results, stitch=options.stitch)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `instamatic-1.8.0/scripts/center_images_smv.py` & `instamatic-1.9.0/scripts/center_images_smv.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/scripts/diagnose_beam_drift.py` & `instamatic-1.9.0/scripts/diagnose_beam_drift.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/scripts/learn.py` & `instamatic-1.9.0/scripts/learn.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-import csv
-import glob
-import sys
-from pathlib import Path
-
-from tqdm.auto import tqdm
-
-from instamatic import neural_network
-from instamatic.formats import *
-
-
-def closest_distance(node, nodes):
-    """Get shortest between a node and a list of nodes (that includes the given
-    node)"""
-    nodes = np.asarray(nodes)
-    dist_2 = np.sum((nodes - node)**2, axis=1)
-    return np.sort(dist_2)[1]**0.5
-
-
-def find_isolated_crystals(fns, min_separation=1.5, boundary=0.5, plot=False):
-    """Find crystals that are at least `min_separation` in micrometers away
-    from other crystals."""
-    isolated = []
-
-    for fn in fns:
-        img, h = read_hdf5(fn)
-        coords = h['exp_crystal_coords']
-
-        if len(coords) == 0:
-            continue
-
-        # apply calibration
-        shape = h['ImageCameraDimensions']
-        dimensions = h['ImageDimensions']
-        calibrated_coords = np.multiply(coords, dimensions / shape)
-
-        boundary_px = shape * boundary / dimensions
-
-        objects = []
-        n_isolated = 0
-
-        for i, (coord, calibrated_coord) in enumerate(zip(coords, calibrated_coords)):
-            try:
-                min_dist = closest_distance(calibrated_coord, calibrated_coords)
-            except IndexError:
-                min_dist = 9999
-
-            x, y = coord
-
-            if not (boundary_px[0] < x < shape[0] - boundary_px[0]):
-                objects.append((x, y, 'orange'))
-            elif not (boundary_px[1] < y < shape[1] - boundary_px[1]):
-                objects.append((x, y, 'orange'))
-            elif min_dist > min_separation:
-                objects.append((x, y, 'red'))
-                n_isolated += 1
-                p = Path(fn)
-                isolated.append(p.parents[1] / 'data' / f'{p.stem}_{i:04d}{p.suffix}')
-            else:
-                objects.append((x, y, 'blue'))
-
-        if plot and n_isolated:
-            import matplotlib.pyplot as plt
-            fig, ax = plt.subplots()
-            ax.imshow(img)
-
-            for (x, y, color) in objects:
-                ax.scatter(y, x, color=color)
-
-            # diff_img, _ = read_hdf5(isolated[-1])
-            # ax2 = inset_locator.inset_axes(ax, "40%", "40%", loc=3)
-            # ax2.imshow(diff_img, vmax=np.percentile(diff_img, 99))
-            # ax2.axis("off")
-
-            ax.axis('off')
-            ax.set_title(fn)
-            plt.show()
-
-    return isolated
-
-
-def main(file_pattern):
-    image_fns = glob.glob(file_pattern)
-    print(len(image_fns), 'Images')
-
-    diff_fns = find_isolated_crystals(image_fns)
-    print(len(diff_fns), 'Patterns from isolated crystals')
-
-    lst = []
-    for fn in tqdm(diff_fns):
-        img, h = read_hdf5(fn)
-
-        frame = int(str(fn)[-12:-8])
-        number = int(str(fn)[-7:-3])
-
-        img_processed = neural_network.preprocess(img.astype(float))
-        prediction = neural_network.predict(img_processed)
-
-        if prediction < 0.5:
-            # print fn, "prediction too low", prediction
-            continue
-
-        try:
-            size = h['total_area_micrometer'] / h['crystal_clusters']  # micrometer^2
-        except KeyError:
-            # old data formats don't have this information
-            size = 0.0
-
-        try:
-            dx, dy = h['exp_hole_offset']
-            cx, cy = h['exp_hole_center']
-        except KeyError:
-            dx, dy = h['exp_scan_offset']
-            cx, cy = h['exp_scan_center']
-
-        prediction = round(prediction, 4)
-        size = round(size, 4)
-        x = int(cx + dx)
-        y = int(cy + dy)
-
-        lst.append((fn.absolute(), frame, number, prediction, size, x, y))
-
-    with open('learning.csv', 'w', newline='') as csvfile:
-        # writer = csv.DictWriter(csvfile, fieldnames=["filename", "frame", "number", "quality", "size", "xpos", "ypos"])
-        # writer.writeheader()
-        writer = csv.writer(csvfile)
-        writer.writerows(lst)
-
-
-def main_entry():
-    import argparse
-    description = """Predict whether a crystal is of good or bad quality by its diffraction pattern."""
-
-    parser = argparse.ArgumentParser(
-        description=description,
-        formatter_class=argparse.RawDescriptionHelpFormatter)
-
-    parser.add_argument('args',
-                        type=str, nargs=1, metavar='PAT',
-                        help='File pattern to glob for images (HDF5), i.e. `images/*.h5`.')
-
-    options = parser.parse_args()
-    args = options.args
-
-    if args:
-        pattern = args[0]
-    else:
-        pattern = 'images/*.h5'
-
-    main(pattern)
-
-
-if __name__ == '__main__':
-    main_entry()
+import csv
+import glob
+import sys
+from pathlib import Path
+
+from tqdm.auto import tqdm
+
+from instamatic import neural_network
+from instamatic.formats import *
+
+
+def closest_distance(node, nodes):
+    """Get shortest between a node and a list of nodes (that includes the given
+    node)"""
+    nodes = np.asarray(nodes)
+    dist_2 = np.sum((nodes - node)**2, axis=1)
+    return np.sort(dist_2)[1]**0.5
+
+
+def find_isolated_crystals(fns, min_separation=1.5, boundary=0.5, plot=False):
+    """Find crystals that are at least `min_separation` in micrometers away
+    from other crystals."""
+    isolated = []
+
+    for fn in fns:
+        img, h = read_hdf5(fn)
+        coords = h['exp_crystal_coords']
+
+        if len(coords) == 0:
+            continue
+
+        # apply calibration
+        shape = h['ImageCameraDimensions']
+        dimensions = h['ImageDimensions']
+        calibrated_coords = np.multiply(coords, dimensions / shape)
+
+        boundary_px = shape * boundary / dimensions
+
+        objects = []
+        n_isolated = 0
+
+        for i, (coord, calibrated_coord) in enumerate(zip(coords, calibrated_coords)):
+            try:
+                min_dist = closest_distance(calibrated_coord, calibrated_coords)
+            except IndexError:
+                min_dist = 9999
+
+            x, y = coord
+
+            if not (boundary_px[0] < x < shape[0] - boundary_px[0]):
+                objects.append((x, y, 'orange'))
+            elif not (boundary_px[1] < y < shape[1] - boundary_px[1]):
+                objects.append((x, y, 'orange'))
+            elif min_dist > min_separation:
+                objects.append((x, y, 'red'))
+                n_isolated += 1
+                p = Path(fn)
+                isolated.append(p.parents[1] / 'data' / f'{p.stem}_{i:04d}{p.suffix}')
+            else:
+                objects.append((x, y, 'blue'))
+
+        if plot and n_isolated:
+            import matplotlib.pyplot as plt
+            fig, ax = plt.subplots()
+            ax.imshow(img)
+
+            for (x, y, color) in objects:
+                ax.scatter(y, x, color=color)
+
+            # diff_img, _ = read_hdf5(isolated[-1])
+            # ax2 = inset_locator.inset_axes(ax, "40%", "40%", loc=3)
+            # ax2.imshow(diff_img, vmax=np.percentile(diff_img, 99))
+            # ax2.axis("off")
+
+            ax.axis('off')
+            ax.set_title(fn)
+            plt.show()
+
+    return isolated
+
+
+def main(file_pattern):
+    image_fns = glob.glob(file_pattern)
+    print(len(image_fns), 'Images')
+
+    diff_fns = find_isolated_crystals(image_fns)
+    print(len(diff_fns), 'Patterns from isolated crystals')
+
+    lst = []
+    for fn in tqdm(diff_fns):
+        img, h = read_hdf5(fn)
+
+        frame = int(str(fn)[-12:-8])
+        number = int(str(fn)[-7:-3])
+
+        img_processed = neural_network.preprocess(img.astype(float))
+        prediction = neural_network.predict(img_processed)
+
+        if prediction < 0.5:
+            # print fn, "prediction too low", prediction
+            continue
+
+        try:
+            size = h['total_area_micrometer'] / h['crystal_clusters']  # micrometer^2
+        except KeyError:
+            # old data formats don't have this information
+            size = 0.0
+
+        try:
+            dx, dy = h['exp_hole_offset']
+            cx, cy = h['exp_hole_center']
+        except KeyError:
+            dx, dy = h['exp_scan_offset']
+            cx, cy = h['exp_scan_center']
+
+        prediction = round(prediction, 4)
+        size = round(size, 4)
+        x = int(cx + dx)
+        y = int(cy + dy)
+
+        lst.append((fn.absolute(), frame, number, prediction, size, x, y))
+
+    with open('learning.csv', 'w', newline='') as csvfile:
+        # writer = csv.DictWriter(csvfile, fieldnames=["filename", "frame", "number", "quality", "size", "xpos", "ypos"])
+        # writer.writeheader()
+        writer = csv.writer(csvfile)
+        writer.writerows(lst)
+
+
+def main_entry():
+    import argparse
+    description = """Predict whether a crystal is of good or bad quality by its diffraction pattern."""
+
+    parser = argparse.ArgumentParser(
+        description=description,
+        formatter_class=argparse.RawDescriptionHelpFormatter)
+
+    parser.add_argument('args',
+                        type=str, nargs=1, metavar='PAT',
+                        help='File pattern to glob for images (HDF5), i.e. `images/*.h5`.')
+
+    options = parser.parse_args()
+    args = options.args
+
+    if args:
+        pattern = args[0]
+    else:
+        pattern = 'images/*.h5'
+
+    main(pattern)
+
+
+if __name__ == '__main__':
+    main_entry()
```

### Comparing `instamatic-1.8.0/scripts/make_interval_movie.py` & `instamatic-1.9.0/scripts/make_interval_movie.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/scripts/make_serialed_movie.py` & `instamatic-1.9.0/scripts/make_serialed_movie.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/scripts/process_dm.py` & `instamatic-1.9.0/scripts/process_dm.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/scripts/process_tpx.py` & `instamatic-1.9.0/scripts/process_tpx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Script to re-process cRED data collecting using instamatic with a Timepix
 camera.
 
-To use:
-    Run `python process_tpx.py cred_log.txt`
+To use:     Run `python process_tpx.py cred_log.txt`
 
-Where the first argument is the path to the cred_log.txt file. Assumes the data are stored
-in a subdirectory `tiff/*.tif` from where cred_log.txt is stored.
+Where the first argument is the path to the cred_log.txt file. Assumes
+the data are stored in a subdirectory `tiff/*.tif` from where
+cred_log.txt is stored.
 
 Defaults to `cred_log.txt` in the current directory if left blank.
 
-If the first argument is given as `all`, the script will look for
-all `cred_log.txt` files in the subdirectories, and iterate over those.
+If the first argument is given as `all`, the script will look for all
+`cred_log.txt` files in the subdirectories, and iterate over those.
 """
 import sys
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
```

### Comparing `instamatic-1.8.0/scripts/process_tvips.py` & `instamatic-1.9.0/scripts/process_tvips.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,244 +1,244 @@
-"""Script to process cRED data collecting using instamatic with the EMMENU
-plugin.
-
-To use:
-    Run `python process_tvips.py cred_log.txt`
-
-Where the first argument is the path to the cred_log.txt file. Assumes the data are stored
-in a subdirectory `tiff/*.tif` from where cred_log.txt is stored.
-
-Defaults to `cred_log.txt` in the current directory if left blank.
-
-If the first argument is given as `all`, the script will look for
-all `cred_log.txt` files in the subdirectories, and iterate over those.
-"""
-import sys
-from pathlib import Path
-
-import numpy as np
-import tifffile
-
-from instamatic.processing.ImgConversionTVIPS import ImgConversionTVIPS as ImgConversion
-from instamatic.tools import get_acquisition_time
-from instamatic.tools import relativistic_wavelength
-
-
-def extract_image_number(s):
-    p = Path(s)
-    return int(p.stem.split('_')[-1])
-
-
-def img_convert(credlog, tiff_path=None, pets_path='PETS', mrc_path='RED', smv_path='SMV'):
-    credlog = Path(credlog)
-    drc = credlog.parent
-
-    pattern = 'tiff/*.tif*'
-
-    image_fns = list(drc.glob(pattern))
-
-    # sort by frame number (avoid confusion with _9.tif -> _10.tif)
-    image_numbers = [extract_image_number(fn) for fn in image_fns]
-    image_numbers, image_fns = zip(*sorted(zip(image_numbers, image_fns)))
-
-    nframes = len(image_fns)
-    if nframes == 0:
-        print(f'No files found matching `{pattern}`')
-        exit()
-    else:
-        print(nframes)
-
-    ims = [tifffile.TiffFile(fn) for fn in image_fns]
-    hs = [im.tvips_metadata for im in ims]
-
-    ts = [h['Time'] for h in hs]  # sort by timestamps
-
-    h0 = hs[0]
-    exposure_time = h0['ExposureTime']
-
-    res = get_acquisition_time(timestamps=ts, exp_time=exposure_time, savefig=True, drc=drc)
-    acquisition_time = res.acquisition_time
-    overhead = res.overhead
-
-    with open(credlog, 'r') as f:
-        for line in f:
-            if line.startswith('Data Collection Time'):
-                timestamp = line.split(':', 1)[-1].strip()
-            if line.startswith('Starting angle'):
-                start_angle = float(line.split()[2])
-            if line.startswith('Ending angle'):
-                end_angle = float(line.split()[2])
-            if line.startswith('Rotation axis'):
-                rotation_axis = float(line.split()[2])
-            if line.startswith('Rotation speed'):
-                rotation_speed = float(line.split()[2])
-            if line.startswith('Beam stopper:'):
-                beamstop = 'yes' in line.split()[2]
-            if line.startswith('Camera length:'):
-                camera_length = float(line.split()[2])
-            if line.startswith('Pixelsize:'):
-                pixelsize = float(line.split()[1])
-            if line.startswith('Physical pixelsize:'):
-                physical_pixelsize = float(line.split()[2])
-            if line.startswith('Wavelength:'):
-                wavelength = float(line.split()[1])
-                
-    beamstop = True
-
-    # from cred_log
-
-    osc_angle = abs(rotation_speed * acquisition_time)
-    direction = [1, -1][end_angle < start_angle]
-    end_angle = start_angle + direction * nframes * osc_angle
-
-    # from header
-
-    high_tension = h0['TemHighTension']  # ev
-    camera = h0['CameraType']
-
-    # It seems that this number cannot be trusted, either in cm or mm, depending on the mode used
-    camera_length_tvips = int(h0['TemMagnification'])
-
-    wavelength_tvips = relativistic_wavelength(high_tension)
-
-    binning_x = h0['BinningX']
-    binning_y = h0['BinningY']
-
-    physical_pixelsize_x_tvips = binning_x * h0['PhysicalPixelSizeX'] / 1_000_000  # nm -> mm
-    physical_pixelsize_y_tvips = binning_y * h0['PhysicalPixelSizeY'] / 1_000_000  # nm -> mm
-
-    # pixelsize can be a factor 10 off, depending on the mode used
-    pixelsize_x_tvips = np.sin(h0['PixelSizeX'] / 1_000_000) / wavelength  # µrad/px -> rad/px -> px/Å
-    pixelsize_y_tvips = np.sin(h0['PixelSizeY'] / 1_000_000) / wavelength  # µrad/px -> rad/px -> px/Å
-
-    image_res_x_tvips = h0['ImageSizeX']
-    image_res_y_tvips = h0['ImageSizeY']
-
-    print(f'Number of frames: {nframes}')
-    print()
-    print('# cRED_log.txt')
-    print(f'Timestamp:                {timestamp}')
-    print(f'Start angle:              {start_angle:.2f} degrees')
-    print(f'End angle:                {end_angle:.2f} degrees')
-    print(f'Oscillation angle:        {osc_angle:.2f} degrees')
-    print(f'Rotation speed:           {rotation_speed:.2f} degrees/s')
-    print(f'Rotation axis at:         {rotation_axis:.2f} radians ({np.degrees(rotation_axis):.2f} degrees)')
-    print(f'Beamstop:                 {beamstop}')
-    print(f'Pixelsize:                {pixelsize} px/Ångstrom')
-    print(f'Physical Pixelsize:       {physical_pixelsize} mm')
-    print(f'Wavelength:               {wavelength} Ångstrom')
-    print(f'TEM Camera length:        {camera_length:.1f} mm')
-
-    print()
-    print('# TVIPS header')
-    print(f'Camera:                   {camera}')
-    print(f'Acquisition time:         {acquisition_time:.3f} s')
-    print(f'Exposure time:            {exposure_time/1000:.3f} s')
-    print(f'Overhead time:            {overhead:.3f} s')
-    print(f'Binning (X/Y):            {binning_x} {binning_y} px/bin')
-    print(f'Image resolution (X/Y):   {image_res_x_tvips} {image_res_y_tvips} pixels')
-    print(f'Pixelsize (X/Y):          {pixelsize_x_tvips:.5f} {pixelsize_y_tvips:.5f} px/Ångstrom???')
-    print(f'Physical pixelsize (X/Y): {physical_pixelsize_x_tvips} {physical_pixelsize_y_tvips} μm')
-    print(f'High tension:             {high_tension/1000} kV')
-    print(f'Wavelength:               {wavelength_tvips} Ångstrom')
-    print(f'Camera length:            {camera_length_tvips} mm')
-
-    # implement this later if it turns out to be necessary
-    assert pixelsize_x_tvips == pixelsize_y_tvips, 'Pixelsize is different in X / Y direction'
-    assert physical_pixelsize_x_tvips == physical_pixelsize_y_tvips, 'Physical pixelsize is different in X / Y direction'
-
-    buffer = []
-
-    print()
-    print('Reading data')
-    for i, fn in enumerate(image_fns):
-        j = i + 1  # j must be 1-indexed
-
-        im = ims[i]
-        h = hs[i]
-
-        img = im.asarray()
-
-        if img.dtype.type is np.int16:
-            if img.min() >= 0 and img.max() < 2**16:
-                img = img.astype(np.uint16)
-
-        assert img.dtype.type is np.uint16, f'Image (#{i}:{fn.stem}) dtype is {img.dtype} (must be np.uint16)'
-
-        h = {'ImageGetTime': timestamp, 'ImageExposureTime': exposure_time}
-
-        buffer.append((j, img, h))
-
-    print('Setting up image conversion')
-    img_conv = ImgConversion(buffer=buffer,
-                             osc_angle=osc_angle,
-                             start_angle=start_angle,
-                             end_angle=end_angle,
-                             rotation_axis=rotation_axis,
-                             acquisition_time=acquisition_time,
-                             flatfield=None,
-                             pixelsize=pixelsize,
-                             physical_pixelsize=physical_pixelsize,
-                             wavelength=wavelength)
-
-    if beamstop:
-        from instamatic.utils.beamstop import find_beamstop_rect
-        print('Finding beam stop')
-        stack_mean = np.mean(tuple(img_conv.data.values()), axis=0)
-        img_conv.mean_beam_center
-        beamstop_rect = find_beamstop_rect(stack_mean, img_conv.mean_beam_center, pad=1, savefig=True, drc=drc)
-        img_conv.add_beamstop(beamstop_rect)
-
-    if mrc_path:
-        mrc_path = drc / mrc_path
-    if smv_path:
-        smv_path = drc / smv_path
-    if tiff_path:
-        tiff_drc_name = tiff_path
-        tiff_path = drc / tiff_path
-    if pets_path:
-        pets_path = drc / pets_path
-
-    print('Writing data')
-    img_conv.threadpoolwriter(tiff_path=tiff_path,
-                              mrc_path=mrc_path,
-                              smv_path=smv_path,
-                              workers=8)
-
-    print('Writing input files')
-    if mrc_path:
-        img_conv.write_ed3d(mrc_path)
-        img_conv.write_REDp_shiftcorrection(mrc_path)
-
-    if smv_path:
-        img_conv.write_xds_inp(smv_path)
-        # img_conv.to_dials(smv_path)
-
-    if tiff_path:
-        img_conv.write_pets_inp(path=drc, tiff_path=tiff_drc_name)
-
-    if pets_path:
-        pets_tiff_path = '../tiff'
-        img_conv.write_pets2_inp(pets_path, tiff_path=pets_tiff_path)
-
-    img_conv.write_beam_centers(path=drc)
-
-
-def main():
-    try:
-        credlog = sys.argv[1]
-    except IndexError:
-        credlog = 'cRED_log.txt'
-
-    if credlog == 'all':
-        fns = Path('.').glob('**/cRED_log.txt')
-        
-        for fn in fns:
-            print(fn)
-            img_convert(fn)
-
-    else:
-        img_convert(credlog)
-        
-
-if __name__ == '__main__':
-    main()
+"""Script to process cRED data collecting using instamatic with the EMMENU
+plugin.
+
+To use, run: `python process_tvips.py cred_log.txt`
+
+Where the first argument is the path to the cred_log.txt file. Assumes
+the data are stored in a subdirectory `tiff/*.tif` from where
+cred_log.txt is stored.
+
+Defaults to `cred_log.txt` in the current directory if left blank.
+
+If the first argument is given as `all`, the script will look for all
+`cred_log.txt` files in the subdirectories, and iterate over those.
+"""
+import sys
+from pathlib import Path
+
+import numpy as np
+import tifffile
+
+from instamatic.processing.ImgConversionTVIPS import ImgConversionTVIPS as ImgConversion
+from instamatic.tools import get_acquisition_time
+from instamatic.tools import relativistic_wavelength
+
+
+def extract_image_number(s):
+    p = Path(s)
+    return int(p.stem.split('_')[-1])
+
+
+def img_convert(credlog, tiff_path=None, pets_path='PETS', mrc_path='RED', smv_path='SMV'):
+    credlog = Path(credlog)
+    drc = credlog.parent
+
+    pattern = 'tiff/*.tif*'
+
+    image_fns = list(drc.glob(pattern))
+
+    # sort by frame number (avoid confusion with _9.tif -> _10.tif)
+    image_numbers = [extract_image_number(fn) for fn in image_fns]
+    image_numbers, image_fns = zip(*sorted(zip(image_numbers, image_fns)))
+
+    nframes = len(image_fns)
+    if nframes == 0:
+        print(f'No files found matching `{pattern}`')
+        exit()
+    else:
+        print(nframes)
+
+    ims = [tifffile.TiffFile(fn) for fn in image_fns]
+    hs = [im.tvips_metadata for im in ims]
+
+    ts = [h['Time'] for h in hs]  # sort by timestamps
+
+    h0 = hs[0]
+    exposure_time = h0['ExposureTime']
+
+    res = get_acquisition_time(timestamps=ts, exp_time=exposure_time, savefig=True, drc=drc)
+    acquisition_time = res.acquisition_time
+    overhead = res.overhead
+
+    with open(credlog, 'r') as f:
+        for line in f:
+            if line.startswith('Data Collection Time'):
+                timestamp = line.split(':', 1)[-1].strip()
+            if line.startswith('Starting angle'):
+                start_angle = float(line.split()[2])
+            if line.startswith('Ending angle'):
+                end_angle = float(line.split()[2])
+            if line.startswith('Rotation axis'):
+                rotation_axis = float(line.split()[2])
+            if line.startswith('Rotation speed'):
+                rotation_speed = float(line.split()[2])
+            if line.startswith('Beam stopper:'):
+                beamstop = 'yes' in line.split()[2]
+            if line.startswith('Camera length:'):
+                camera_length = float(line.split()[2])
+            if line.startswith('Pixelsize:'):
+                pixelsize = float(line.split()[1])
+            if line.startswith('Physical pixelsize:'):
+                physical_pixelsize = float(line.split()[2])
+            if line.startswith('Wavelength:'):
+                wavelength = float(line.split()[1])
+
+    beamstop = True
+
+    # from cred_log
+
+    osc_angle = abs(rotation_speed * acquisition_time)
+    direction = [1, -1][end_angle < start_angle]
+    end_angle = start_angle + direction * nframes * osc_angle
+
+    # from header
+
+    high_tension = h0['TemHighTension']  # ev
+    camera = h0['CameraType']
+
+    # It seems that this number cannot be trusted, either in cm or mm, depending on the mode used
+    camera_length_tvips = int(h0['TemMagnification'])
+
+    wavelength_tvips = relativistic_wavelength(high_tension)
+
+    binning_x = h0['BinningX']
+    binning_y = h0['BinningY']
+
+    physical_pixelsize_x_tvips = binning_x * h0['PhysicalPixelSizeX'] / 1_000_000  # nm -> mm
+    physical_pixelsize_y_tvips = binning_y * h0['PhysicalPixelSizeY'] / 1_000_000  # nm -> mm
+
+    # pixelsize can be a factor 10 off, depending on the mode used
+    pixelsize_x_tvips = np.sin(h0['PixelSizeX'] / 1_000_000) / wavelength  # µrad/px -> rad/px -> px/Å
+    pixelsize_y_tvips = np.sin(h0['PixelSizeY'] / 1_000_000) / wavelength  # µrad/px -> rad/px -> px/Å
+
+    image_res_x_tvips = h0['ImageSizeX']
+    image_res_y_tvips = h0['ImageSizeY']
+
+    print(f'Number of frames: {nframes}')
+    print()
+    print('# cRED_log.txt')
+    print(f'Timestamp:                {timestamp}')
+    print(f'Start angle:              {start_angle:.2f} degrees')
+    print(f'End angle:                {end_angle:.2f} degrees')
+    print(f'Oscillation angle:        {osc_angle:.2f} degrees')
+    print(f'Rotation speed:           {rotation_speed:.2f} degrees/s')
+    print(f'Rotation axis at:         {rotation_axis:.2f} radians ({np.degrees(rotation_axis):.2f} degrees)')
+    print(f'Beamstop:                 {beamstop}')
+    print(f'Pixelsize:                {pixelsize} px/Ångstrom')
+    print(f'Physical Pixelsize:       {physical_pixelsize} mm')
+    print(f'Wavelength:               {wavelength} Ångstrom')
+    print(f'TEM Camera length:        {camera_length:.1f} mm')
+
+    print()
+    print('# TVIPS header')
+    print(f'Camera:                   {camera}')
+    print(f'Acquisition time:         {acquisition_time:.3f} s')
+    print(f'Exposure time:            {exposure_time/1000:.3f} s')
+    print(f'Overhead time:            {overhead:.3f} s')
+    print(f'Binning (X/Y):            {binning_x} {binning_y} px/bin')
+    print(f'Image resolution (X/Y):   {image_res_x_tvips} {image_res_y_tvips} pixels')
+    print(f'Pixelsize (X/Y):          {pixelsize_x_tvips:.5f} {pixelsize_y_tvips:.5f} px/Ångstrom???')
+    print(f'Physical pixelsize (X/Y): {physical_pixelsize_x_tvips} {physical_pixelsize_y_tvips} μm')
+    print(f'High tension:             {high_tension/1000} kV')
+    print(f'Wavelength:               {wavelength_tvips} Ångstrom')
+    print(f'Camera length:            {camera_length_tvips} mm')
+
+    # implement this later if it turns out to be necessary
+    assert pixelsize_x_tvips == pixelsize_y_tvips, 'Pixelsize is different in X / Y direction'
+    assert physical_pixelsize_x_tvips == physical_pixelsize_y_tvips, 'Physical pixelsize is different in X / Y direction'
+
+    buffer = []
+
+    print()
+    print('Reading data')
+    for i, fn in enumerate(image_fns):
+        j = i + 1  # j must be 1-indexed
+
+        im = ims[i]
+        h = hs[i]
+
+        img = im.asarray()
+
+        if img.dtype.type is np.int16:
+            if img.min() >= 0 and img.max() < 2**16:
+                img = img.astype(np.uint16)
+
+        assert img.dtype.type is np.uint16, f'Image (#{i}:{fn.stem}) dtype is {img.dtype} (must be np.uint16)'
+
+        h = {'ImageGetTime': timestamp, 'ImageExposureTime': exposure_time}
+
+        buffer.append((j, img, h))
+
+    print('Setting up image conversion')
+    img_conv = ImgConversion(buffer=buffer,
+                             osc_angle=osc_angle,
+                             start_angle=start_angle,
+                             end_angle=end_angle,
+                             rotation_axis=rotation_axis,
+                             acquisition_time=acquisition_time,
+                             flatfield=None,
+                             pixelsize=pixelsize,
+                             physical_pixelsize=physical_pixelsize,
+                             wavelength=wavelength)
+
+    if beamstop:
+        from instamatic.utils.beamstop import find_beamstop_rect
+        print('Finding beam stop')
+        stack_mean = np.mean(tuple(img_conv.data.values()), axis=0)
+        img_conv.mean_beam_center
+        beamstop_rect = find_beamstop_rect(stack_mean, img_conv.mean_beam_center, pad=1, savefig=True, drc=drc)
+        img_conv.add_beamstop(beamstop_rect)
+
+    if mrc_path:
+        mrc_path = drc / mrc_path
+    if smv_path:
+        smv_path = drc / smv_path
+    if tiff_path:
+        tiff_drc_name = tiff_path
+        tiff_path = drc / tiff_path
+    if pets_path:
+        pets_path = drc / pets_path
+
+    print('Writing data')
+    img_conv.threadpoolwriter(tiff_path=tiff_path,
+                              mrc_path=mrc_path,
+                              smv_path=smv_path,
+                              workers=8)
+
+    print('Writing input files')
+    if mrc_path:
+        img_conv.write_ed3d(mrc_path)
+        img_conv.write_REDp_shiftcorrection(mrc_path)
+
+    if smv_path:
+        img_conv.write_xds_inp(smv_path)
+        # img_conv.to_dials(smv_path)
+
+    if tiff_path:
+        img_conv.write_pets_inp(path=drc, tiff_path=tiff_drc_name)
+
+    if pets_path:
+        pets_tiff_path = '../tiff'
+        img_conv.write_pets2_inp(pets_path, tiff_path=pets_tiff_path)
+
+    img_conv.write_beam_centers(path=drc)
+
+
+def main():
+    try:
+        credlog = sys.argv[1]
+    except IndexError:
+        credlog = 'cRED_log.txt'
+
+    if credlog == 'all':
+        fns = Path('.').glob('**/cRED_log.txt')
+
+        for fn in fns:
+            print(fn)
+            img_convert(fn)
+
+    else:
+        img_convert(credlog)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `instamatic-1.8.0/scripts/viewer.py` & `instamatic-1.9.0/scripts/viewer.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/setup.cfg` & `instamatic-1.9.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,225 +1,223 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6175 7468  [metadata]..auth
-00000010: 6f72 203d 2053 7465 6620 536d 6565 7473  or = Stef Smeets
-00000020: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
-00000030: 2073 2e73 6d65 6574 7340 6573 6369 656e   s.smeets@escien
-00000040: 6365 6365 6e74 6572 2e6e 6c0d 0a63 6c61  cecenter.nl..cla
-00000050: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-00000060: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000070: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000080: 332e 370d 0a09 5072 6f67 7261 6d6d 696e  3.7...Programmin
-00000090: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000000a0: 7468 6f6e 203a 3a20 332e 380d 0a09 5072  thon :: 3.8...Pr
-000000b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000000c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000000d0: 332e 390d 0a09 4465 7665 6c6f 706d 656e  3.9...Developmen
-000000e0: 7420 5374 6174 7573 203a 3a20 3520 2d20  t Status :: 5 - 
-000000f0: 5072 6f64 7563 7469 6f6e 2f53 7461 626c  Production/Stabl
-00000100: 650d 0a09 496e 7465 6e64 6564 2041 7564  e...Intended Aud
-00000110: 6965 6e63 6520 3a3a 2053 6369 656e 6365  ience :: Science
-00000120: 2f52 6573 6561 7263 680d 0a09 4c69 6365  /Research...Lice
-00000130: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000140: 7665 6420 3a3a 2042 5344 204c 6963 656e  ved :: BSD Licen
-00000150: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
-00000160: 7973 7465 6d20 3a3a 204d 6963 726f 736f  ystem :: Microso
-00000170: 6674 203a 3a20 5769 6e64 6f77 730d 0a09  ft :: Windows...
-00000180: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
-00000190: 6669 632f 456e 6769 6e65 6572 696e 6720  fic/Engineering 
-000001a0: 3a3a 2048 756d 616e 204d 6163 6869 6e65  :: Human Machine
-000001b0: 2049 6e74 6572 6661 6365 730d 0a09 546f   Interfaces...To
-000001c0: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
-000001d0: 632f 456e 6769 6e65 6572 696e 6720 3a3a  c/Engineering ::
-000001e0: 2043 6865 6d69 7374 7279 0d0a 0954 6f70   Chemistry...Top
-000001f0: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
-00000200: 6576 656c 6f70 6d65 6e74 203a 3a20 4c69  evelopment :: Li
-00000210: 6272 6172 6965 730d 0a64 6573 6372 6970  braries..descrip
-00000220: 7469 6f6e 203d 2044 5079 7468 6f6e 2070  tion = DPython p
-00000230: 726f 6772 616d 2066 6f72 2061 7574 6f6d  rogram for autom
-00000240: 6174 6564 2065 6c65 6374 726f 6e20 6469  ated electron di
-00000250: 6666 7261 6374 696f 6e20 6461 7461 2063  ffraction data c
-00000260: 6f6c 6c65 6374 696f 6e0d 0a6b 6579 776f  ollection..keywo
-00000270: 7264 7320 3d20 0d0a 0965 6c65 6374 726f  rds = ...electro
-00000280: 6e2d 6372 7973 7461 6c6c 6f67 7261 7068  n-crystallograph
-00000290: 790d 0a09 656c 6563 7472 6f6e 2d6d 6963  y...electron-mic
-000002a0: 726f 7363 6f70 790d 0a09 656c 6563 7472  roscopy...electr
-000002b0: 6f6e 2d64 6966 6672 6163 7469 6f6e 0d0a  on-diffraction..
-000002c0: 0973 6572 6961 6c2d 6372 7973 7461 6c6c  .serial-crystall
-000002d0: 6f67 7261 7068 790d 0a09 3344 2d65 6c65  ography...3D-ele
-000002e0: 6374 726f 6e2d 6469 6666 7261 6374 696f  ctron-diffractio
-000002f0: 6e0d 0a09 6d69 6372 6f2d 6564 0d0a 0964  n...micro-ed...d
-00000300: 6174 612d 636f 6c6c 6563 7469 6f6e 0d0a  ata-collection..
-00000310: 0961 7574 6f6d 6174 696f 6e0d 0a6c 6f6e  .automation..lon
-00000320: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-00000330: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
-00000340: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-00000350: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-00000360: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-00000370: 6e61 6d65 203d 2069 6e73 7461 6d61 7469  name = instamati
-00000380: 630d 0a70 726f 6a65 6374 5f75 726c 7320  c..project_urls 
-00000390: 3d20 0d0a 0942 7567 2054 7261 636b 6572  = ...Bug Tracker
-000003a0: 203d 2068 7474 703a 2f2f 6769 7468 7562   = http://github
-000003b0: 2e63 6f6d 2f69 6e73 7461 6d61 7469 632d  .com/instamatic-
-000003c0: 6465 762f 696e 7374 616d 6174 6963 2f69  dev/instamatic/i
-000003d0: 7373 7565 730d 0a09 446f 6375 6d65 6e74  ssues...Document
-000003e0: 6174 696f 6e20 3d20 6874 7470 733a 2f2f  ation = https://
-000003f0: 696e 7374 616d 6174 6963 2e72 6561 6474  instamatic.readt
-00000400: 6865 646f 6373 2e69 6f2f 0d0a 7572 6c20  hedocs.io/..url 
-00000410: 3d20 6874 7470 3a2f 2f67 6974 6875 622e  = http://github.
-00000420: 636f 6d2f 696e 7374 616d 6174 6963 2d64  com/instamatic-d
-00000430: 6576 2f69 6e73 7461 6d61 7469 630d 0a76  ev/instamatic..v
-00000440: 6572 7369 6f6e 203d 2031 2e38 2e30 0d0a  ersion = 1.8.0..
-00000450: 0d0a 5b6f 7074 696f 6e73 5d0d 0a7a 6970  ..[options]..zip
-00000460: 5f73 6166 6520 3d20 4661 6c73 650d 0a69  _safe = False..i
-00000470: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-00000480: 6174 6120 3d20 5472 7565 0d0a 7061 636b  ata = True..pack
-00000490: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
-000004a0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-000004b0: 200d 0a09 636f 6d74 7970 6573 203e 3d20   ...comtypes >= 
-000004c0: 312e 312e 370d 0a09 6835 7079 203e 3d20  1.1.7...h5py >= 
-000004d0: 322e 3130 2e30 0d0a 0969 7079 7468 6f6e  2.10.0...ipython
-000004e0: 203e 3d20 372e 3131 2e31 0d0a 096c 6d66   >= 7.11.1...lmf
-000004f0: 6974 203e 3d20 312e 302e 300d 0a09 6d61  it >= 1.0.0...ma
-00000500: 7470 6c6f 746c 6962 203e 3d20 332e 312e  tplotlib >= 3.1.
-00000510: 320d 0a09 6d72 6366 696c 6520 3e3d 2031  2...mrcfile >= 1
-00000520: 2e31 2e32 0d0a 096e 756d 7079 203e 3d20  .1.2...numpy >= 
-00000530: 312e 3137 2e33 0d0a 0970 616e 6461 7320  1.17.3...pandas 
-00000540: 3e3d 2031 2e30 2e30 0d0a 0970 696c 6c6f  >= 1.0.0...pillo
-00000550: 7720 3e3d 2037 2e30 2e30 0d0a 0970 7977  w >= 7.0.0...pyw
-00000560: 696e 6175 746f 203e 3d20 302e 362e 380d  inauto >= 0.6.8.
-00000570: 0a09 7079 7961 6d6c 203e 3d20 352e 330d  ..pyyaml >= 5.3.
-00000580: 0a09 7363 696b 6974 2d69 6d61 6765 203e  ..scikit-image >
-00000590: 3d20 302e 3137 2e31 0d0a 0973 6369 7079  = 0.17.1...scipy
-000005a0: 203e 3d20 312e 332e 320d 0a09 7469 6666   >= 1.3.2...tiff
-000005b0: 6669 6c65 203e 3d20 3230 3139 2e37 2e32  file >= 2019.7.2
-000005c0: 362e 320d 0a09 7471 646d 203e 3d20 342e  6.2...tqdm >= 4.
-000005d0: 3431 2e31 0d0a 0976 6972 7475 616c 626f  41.1...virtualbo
-000005e0: 7820 3e3d 2032 2e30 2e30 0d0a 0970 7973  x >= 2.0.0...pys
-000005f0: 6572 6961 6c65 6d20 3e3d 2030 2e33 2e32  erialem >= 0.3.2
-00000600: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 7874  ....[options.ext
-00000610: 7261 735f 7265 7175 6972 655d 0d0a 6465  ras_require]..de
-00000620: 7665 6c6f 7020 3d20 0d0a 0962 756d 7032  velop = ...bump2
-00000630: 7665 7273 696f 6e0d 0a09 6368 6563 6b2d  version...check-
-00000640: 6d61 6e69 6665 7374 0d0a 0970 7265 2d63  manifest...pre-c
-00000650: 6f6d 6d69 740d 0a09 666c 616b 6538 0d0a  ommit...flake8..
-00000660: 0970 7974 6573 7420 3e3d 2035 2e34 2e31  .pytest >= 5.4.1
-00000670: 0d0a 0970 7974 6573 742d 636f 7620 3e3d  ...pytest-cov >=
-00000680: 2032 2e38 2e31 0d0a 7365 7276 616c 203d   2.8.1..serval =
-00000690: 200d 0a09 7365 7276 616c 2d74 6f6f 6c6b   ...serval-toolk
-000006a0: 6974 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  it....[options.p
-000006b0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a69  ackages.find]..i
-000006c0: 6e63 6c75 6465 203d 2069 6e73 7461 6d61  nclude = instama
-000006d0: 7469 632c 2069 6e73 7461 6d61 7469 632e  tic, instamatic.
-000006e0: 2a2c 2069 6e73 7461 6d61 7469 632e 6578  *, instamatic.ex
-000006f0: 7065 7269 6d65 6e74 732e 2a0d 0a0d 0a5b  periments.*....[
-00000700: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
-00000710: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
-00000720: 6372 6970 7473 203d 200d 0a09 696e 7374  cripts = ...inst
-00000730: 616d 6174 6963 203d 2069 6e73 7461 6d61  amatic = instama
-00000740: 7469 632e 6d61 696e 3a6d 6169 6e0d 0a09  tic.main:main...
-00000750: 696e 7374 616d 6174 6963 2e63 6f6e 7472  instamatic.contr
-00000760: 6f6c 6c65 7220 3d20 696e 7374 616d 6174  oller = instamat
-00000770: 6963 2e54 454d 436f 6e74 726f 6c6c 6572  ic.TEMController
-00000780: 2e54 454d 436f 6e74 726f 6c6c 6572 3a6d  .TEMController:m
-00000790: 6169 6e5f 656e 7472 790d 0a09 696e 7374  ain_entry...inst
-000007a0: 616d 6174 6963 2e73 6572 6961 6c65 6420  amatic.serialed 
-000007b0: 3d20 696e 7374 616d 6174 6963 2e65 7870  = instamatic.exp
-000007c0: 6572 696d 656e 7473 2e73 6572 6961 6c65  eriments.seriale
-000007d0: 642e 6578 7065 7269 6d65 6e74 3a6d 6169  d.experiment:mai
-000007e0: 6e0d 0a09 696e 7374 616d 6174 6963 2e63  n...instamatic.c
-000007f0: 616d 6572 6120 3d20 696e 7374 616d 6174  amera = instamat
-00000800: 6963 2e63 616d 6572 612e 6361 6d65 7261  ic.camera.camera
-00000810: 3a6d 6169 6e5f 656e 7472 790d 0a09 696e  :main_entry...in
-00000820: 7374 616d 6174 6963 2e63 616c 6962 7261  stamatic.calibra
-00000830: 7465 5f73 7461 6765 5f6c 6f77 6d61 6720  te_stage_lowmag 
-00000840: 3d20 696e 7374 616d 6174 6963 2e63 616c  = instamatic.cal
-00000850: 6962 7261 7465 2e63 616c 6962 7261 7465  ibrate.calibrate
-00000860: 5f73 7461 6765 5f6c 6f77 6d61 673a 6d61  _stage_lowmag:ma
-00000870: 696e 5f65 6e74 7279 0d0a 0969 6e73 7461  in_entry...insta
-00000880: 6d61 7469 632e 6361 6c69 6272 6174 655f  matic.calibrate_
-00000890: 7374 6167 655f 6d61 6731 203d 2069 6e73  stage_mag1 = ins
-000008a0: 7461 6d61 7469 632e 6361 6c69 6272 6174  tamatic.calibrat
-000008b0: 652e 6361 6c69 6272 6174 655f 7374 6167  e.calibrate_stag
-000008c0: 655f 6d61 6731 3a6d 6169 6e5f 656e 7472  e_mag1:main_entr
-000008d0: 790d 0a09 696e 7374 616d 6174 6963 2e63  y...instamatic.c
-000008e0: 616c 6962 7261 7465 5f62 6561 6d73 6869  alibrate_beamshi
-000008f0: 6674 203d 2069 6e73 7461 6d61 7469 632e  ft = instamatic.
-00000900: 6361 6c69 6272 6174 652e 6361 6c69 6272  calibrate.calibr
-00000910: 6174 655f 6265 616d 7368 6966 743a 6d61  ate_beamshift:ma
-00000920: 696e 5f65 6e74 7279 0d0a 0969 6e73 7461  in_entry...insta
-00000930: 6d61 7469 632e 6361 6c69 6272 6174 655f  matic.calibrate_
-00000940: 6469 7265 6374 6265 616d 203d 2069 6e73  directbeam = ins
-00000950: 7461 6d61 7469 632e 6361 6c69 6272 6174  tamatic.calibrat
-00000960: 652e 6361 6c69 6272 6174 655f 6469 7265  e.calibrate_dire
-00000970: 6374 6265 616d 3a6d 6169 6e5f 656e 7472  ctbeam:main_entr
-00000980: 790d 0a09 696e 7374 616d 6174 6963 2e63  y...instamatic.c
-00000990: 616c 6962 7261 7465 5f73 7461 6765 6d61  alibrate_stagema
-000009a0: 7472 6978 203d 2069 6e73 7461 6d61 7469  trix = instamati
-000009b0: 632e 6361 6c69 6272 6174 652e 6361 6c69  c.calibrate.cali
-000009c0: 6272 6174 655f 7374 6167 656d 6174 7269  brate_stagematri
-000009d0: 783a 6d61 696e 5f65 6e74 7279 0d0a 0969  x:main_entry...i
-000009e0: 6e73 7461 6d61 7469 632e 666c 6174 6669  nstamatic.flatfi
-000009f0: 656c 6420 3d20 696e 7374 616d 6174 6963  eld = instamatic
-00000a00: 2e70 726f 6365 7373 696e 672e 666c 6174  .processing.flat
-00000a10: 6669 656c 643a 6d61 696e 5f65 6e74 7279  field:main_entry
-00000a20: 0d0a 0969 6e73 7461 6d61 7469 632e 7374  ...instamatic.st
-00000a30: 7265 7463 685f 636f 7272 6563 7469 6f6e  retch_correction
-00000a40: 203d 2069 6e73 7461 6d61 7469 632e 7072   = instamatic.pr
-00000a50: 6f63 6573 7369 6e67 2e73 7472 6574 6368  ocessing.stretch
-00000a60: 5f63 6f72 7265 6374 696f 6e3a 6d61 696e  _correction:main
-00000a70: 5f65 6e74 7279 0d0a 0969 6e73 7461 6d61  _entry...instama
-00000a80: 7469 632e 6272 6f77 7365 7220 3d20 7363  tic.browser = sc
-00000a90: 7269 7074 732e 6272 6f77 7365 723a 6d61  ripts.browser:ma
-00000aa0: 696e 0d0a 0969 6e73 7461 6d61 7469 632e  in...instamatic.
-00000ab0: 7669 6577 6572 203d 2073 6372 6970 7473  viewer = scripts
-00000ac0: 2e76 6965 7765 723a 6d61 696e 0d0a 0969  .viewer:main...i
-00000ad0: 6e73 7461 6d61 7469 632e 6465 666f 6375  nstamatic.defocu
-00000ae0: 735f 6865 6c70 6572 203d 2069 6e73 7461  s_helper = insta
-00000af0: 6d61 7469 632e 6775 692e 6465 666f 6375  matic.gui.defocu
-00000b00: 735f 6275 7474 6f6e 3a6d 6169 6e0d 0a09  s_button:main...
-00000b10: 696e 7374 616d 6174 6963 2e66 696e 645f  instamatic.find_
-00000b20: 6372 7973 7461 6c73 203d 2069 6e73 7461  crystals = insta
-00000b30: 6d61 7469 632e 7072 6f63 6573 7369 6e67  matic.processing
-00000b40: 2e66 696e 645f 6372 7973 7461 6c73 3a6d  .find_crystals:m
-00000b50: 6169 6e5f 656e 7472 790d 0a09 696e 7374  ain_entry...inst
-00000b60: 616d 6174 6963 2e66 696e 645f 6372 7973  amatic.find_crys
-00000b70: 7461 6c73 5f69 6c61 7374 696b 203d 2069  tals_ilastik = i
-00000b80: 6e73 7461 6d61 7469 632e 7072 6f63 6573  nstamatic.proces
-00000b90: 7369 6e67 2e66 696e 645f 6372 7973 7461  sing.find_crysta
-00000ba0: 6c73 5f69 6c61 7374 696b 3a6d 6169 6e5f  ls_ilastik:main_
-00000bb0: 656e 7472 790d 0a09 696e 7374 616d 6174  entry...instamat
-00000bc0: 6963 2e6c 6561 726e 203d 2073 6372 6970  ic.learn = scrip
-00000bd0: 7473 2e6c 6561 726e 3a6d 6169 6e5f 656e  ts.learn:main_en
-00000be0: 7472 790d 0a09 696e 7374 616d 6174 6963  try...instamatic
-00000bf0: 2e74 656d 7365 7276 6572 203d 2069 6e73  .temserver = ins
-00000c00: 7461 6d61 7469 632e 7365 7276 6572 2e74  tamatic.server.t
-00000c10: 656d 5f73 6572 7665 723a 6d61 696e 0d0a  em_server:main..
-00000c20: 0969 6e73 7461 6d61 7469 632e 6361 6d73  .instamatic.cams
-00000c30: 6572 7665 7220 3d20 696e 7374 616d 6174  erver = instamat
-00000c40: 6963 2e73 6572 7665 722e 6361 6d5f 7365  ic.server.cam_se
-00000c50: 7276 6572 3a6d 6169 6e0d 0a09 696e 7374  rver:main...inst
-00000c60: 616d 6174 6963 2e64 6961 6c73 7365 7276  amatic.dialsserv
-00000c70: 6572 203d 2069 6e73 7461 6d61 7469 632e  er = instamatic.
-00000c80: 7365 7276 6572 2e64 6961 6c73 5f73 6572  server.dials_ser
-00000c90: 7665 723a 6d61 696e 0d0a 0969 6e73 7461  ver:main...insta
-00000ca0: 6d61 7469 632e 564d 7365 7276 6572 203d  matic.VMserver =
-00000cb0: 2069 6e73 7461 6d61 7469 632e 7365 7276   instamatic.serv
-00000cc0: 6572 2e76 6d5f 7562 756e 7475 5f73 6572  er.vm_ubuntu_ser
-00000cd0: 7665 723a 6d61 696e 0d0a 0969 6e73 7461  ver:main...insta
-00000ce0: 6d61 7469 632e 7864 7373 6572 7665 7220  matic.xdsserver 
-00000cf0: 3d20 696e 7374 616d 6174 6963 2e73 6572  = instamatic.ser
-00000d00: 7665 722e 7864 735f 7365 7276 6572 3a6d  ver.xds_server:m
-00000d10: 6169 6e0d 0a09 696e 7374 616d 6174 6963  ain...instamatic
-00000d20: 2e74 656d 7365 7276 6572 5f66 6569 203d  .temserver_fei =
-00000d30: 2069 6e73 7461 6d61 7469 632e 7365 7276   instamatic.serv
-00000d40: 6572 2e54 454d 5365 7276 6572 5f46 4549  er.TEMServer_FEI
-00000d50: 3a6d 6169 6e0d 0a09 696e 7374 616d 6174  :main...instamat
-00000d60: 6963 2e67 6f6e 696f 746f 6f6c 7365 7276  ic.goniotoolserv
-00000d70: 6572 203d 2069 6e73 7461 6d61 7469 632e  er = instamatic.
-00000d80: 7365 7276 6572 2e67 6f6e 696f 746f 6f6c  server.goniotool
-00000d90: 5f73 6572 7665 723a 6d61 696e 0d0a 0969  _server:main...i
-00000da0: 6e73 7461 6d61 7469 632e 6175 746f 636f  nstamatic.autoco
-00000db0: 6e66 6967 203d 2069 6e73 7461 6d61 7469  nfig = instamati
-00000dc0: 632e 636f 6e66 6967 2e61 7574 6f63 6f6e  c.config.autocon
-00000dd0: 6669 673a 6d61 696e 0d0a 0d0a 5b65 6767  fig:main....[egg
-00000de0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000df0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000e00: 2030 0d0a 0d0a                            0....
+00000000: 5b6d 6574 6164 6174 615d 0a61 7574 686f  [metadata].autho
+00000010: 7220 3d20 5374 6566 2053 6d65 6574 730a  r = Stef Smeets.
+00000020: 6175 7468 6f72 5f65 6d61 696c 203d 2073  author_email = s
+00000030: 2e73 6d65 6574 7340 6573 6369 656e 6365  .smeets@escience
+00000040: 6365 6e74 6572 2e6e 6c0a 636c 6173 7369  center.nl.classi
+00000050: 6669 6572 7320 3d20 0a09 5072 6f67 7261  fiers = ..Progra
+00000060: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000070: 3a20 5079 7468 6f6e 203a 3a20 332e 370a  : Python :: 3.7.
+00000080: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000090: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000000a0: 3a3a 2033 2e38 0a09 5072 6f67 7261 6d6d  :: 3.8..Programm
+000000b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000000c0: 5079 7468 6f6e 203a 3a20 332e 390a 0950  Python :: 3.9..P
+000000d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000000e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000000f0: 2033 2e31 300a 0950 726f 6772 616d 6d69   3.10..Programmi
+00000100: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000110: 7974 686f 6e20 3a3a 2033 2e31 310a 0944  ython :: 3.11..D
+00000120: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
+00000130: 7320 3a3a 2035 202d 2050 726f 6475 6374  s :: 5 - Product
+00000140: 696f 6e2f 5374 6162 6c65 0a09 496e 7465  ion/Stable..Inte
+00000150: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000160: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
+00000170: 680a 094c 6963 656e 7365 203a 3a20 4f53  h..License :: OS
+00000180: 4920 4170 7072 6f76 6564 203a 3a20 4253  I Approved :: BS
+00000190: 4420 4c69 6365 6e73 650a 094f 7065 7261  D License..Opera
+000001a0: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
+000001b0: 6963 726f 736f 6674 203a 3a20 5769 6e64  icrosoft :: Wind
+000001c0: 6f77 730a 0954 6f70 6963 203a 3a20 5363  ows..Topic :: Sc
+000001d0: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
+000001e0: 7269 6e67 203a 3a20 4875 6d61 6e20 4d61  ring :: Human Ma
+000001f0: 6368 696e 6520 496e 7465 7266 6163 6573  chine Interfaces
+00000200: 0a09 546f 7069 6320 3a3a 2053 6369 656e  ..Topic :: Scien
+00000210: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
+00000220: 6720 3a3a 2043 6865 6d69 7374 7279 0a09  g :: Chemistry..
+00000230: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
+00000240: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
+00000250: 204c 6962 7261 7269 6573 0a64 6573 6372   Libraries.descr
+00000260: 6970 7469 6f6e 203d 2050 7974 686f 6e20  iption = Python 
+00000270: 7072 6f67 7261 6d20 666f 7220 6175 746f  program for auto
+00000280: 6d61 7465 6420 656c 6563 7472 6f6e 2064  mated electron d
+00000290: 6966 6672 6163 7469 6f6e 2064 6174 6120  iffraction data 
+000002a0: 636f 6c6c 6563 7469 6f6e 0a6b 6579 776f  collection.keywo
+000002b0: 7264 7320 3d20 0a09 656c 6563 7472 6f6e  rds = ..electron
+000002c0: 2d63 7279 7374 616c 6c6f 6772 6170 6879  -crystallography
+000002d0: 0a09 656c 6563 7472 6f6e 2d6d 6963 726f  ..electron-micro
+000002e0: 7363 6f70 790a 0965 6c65 6374 726f 6e2d  scopy..electron-
+000002f0: 6469 6666 7261 6374 696f 6e0a 0973 6572  diffraction..ser
+00000300: 6961 6c2d 6372 7973 7461 6c6c 6f67 7261  ial-crystallogra
+00000310: 7068 790a 0933 442d 656c 6563 7472 6f6e  phy..3D-electron
+00000320: 2d64 6966 6672 6163 7469 6f6e 0a09 6d69  -diffraction..mi
+00000330: 6372 6f2d 6564 0a09 6461 7461 2d63 6f6c  cro-ed..data-col
+00000340: 6c65 6374 696f 6e0a 0961 7574 6f6d 6174  lection..automat
+00000350: 696f 6e0a 6c6f 6e67 5f64 6573 6372 6970  ion.long_descrip
+00000360: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
+00000370: 444d 452e 6d64 0a6c 6f6e 675f 6465 7363  DME.md.long_desc
+00000380: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+00000390: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+000003a0: 646f 776e 0a6e 616d 6520 3d20 696e 7374  down.name = inst
+000003b0: 616d 6174 6963 0a70 726f 6a65 6374 5f75  amatic.project_u
+000003c0: 726c 7320 3d20 0a09 4275 6720 5472 6163  rls = ..Bug Trac
+000003d0: 6b65 7220 3d20 6874 7470 3a2f 2f67 6974  ker = http://git
+000003e0: 6875 622e 636f 6d2f 696e 7374 616d 6174  hub.com/instamat
+000003f0: 6963 2d64 6576 2f69 6e73 7461 6d61 7469  ic-dev/instamati
+00000400: 632f 6973 7375 6573 0a09 446f 6375 6d65  c/issues..Docume
+00000410: 6e74 6174 696f 6e20 3d20 6874 7470 733a  ntation = https:
+00000420: 2f2f 696e 7374 616d 6174 6963 2e72 6561  //instamatic.rea
+00000430: 6474 6865 646f 6373 2e69 6f2f 0a75 726c  dthedocs.io/.url
+00000440: 203d 2068 7474 703a 2f2f 6769 7468 7562   = http://github
+00000450: 2e63 6f6d 2f69 6e73 7461 6d61 7469 632d  .com/instamatic-
+00000460: 6465 762f 696e 7374 616d 6174 6963 0a76  dev/instamatic.v
+00000470: 6572 7369 6f6e 203d 2031 2e39 2e30 0a0a  ersion = 1.9.0..
+00000480: 5b6f 7074 696f 6e73 5d0a 7a69 705f 7361  [options].zip_sa
+00000490: 6665 203d 2046 616c 7365 0a69 6e63 6c75  fe = False.inclu
+000004a0: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+000004b0: 3d20 5472 7565 0a70 6163 6b61 6765 7320  = True.packages 
+000004c0: 3d20 6669 6e64 3a0a 696e 7374 616c 6c5f  = find:.install_
+000004d0: 7265 7175 6972 6573 203d 200a 0963 6f6d  requires = ..com
+000004e0: 7479 7065 7320 3e3d 2031 2e31 2e37 0a09  types >= 1.1.7..
+000004f0: 6835 7079 203e 3d20 322e 3130 2e30 0a09  h5py >= 2.10.0..
+00000500: 6970 7974 686f 6e20 3e3d 2037 2e31 312e  ipython >= 7.11.
+00000510: 310a 096c 6d66 6974 203e 3d20 312e 302e  1..lmfit >= 1.0.
+00000520: 300a 096d 6174 706c 6f74 6c69 6220 3e3d  0..matplotlib >=
+00000530: 2033 2e31 2e32 0a09 6d72 6366 696c 6520   3.1.2..mrcfile 
+00000540: 3e3d 2031 2e31 2e32 0a09 6e75 6d70 7920  >= 1.1.2..numpy 
+00000550: 3e3d 2031 2e31 372e 330a 0970 616e 6461  >= 1.17.3..panda
+00000560: 7320 3e3d 2031 2e30 2e30 0a09 7069 6c6c  s >= 1.0.0..pill
+00000570: 6f77 203e 3d20 372e 302e 300a 0970 7977  ow >= 7.0.0..pyw
+00000580: 696e 6175 746f 203e 3d20 302e 362e 380a  inauto >= 0.6.8.
+00000590: 0970 7979 616d 6c20 3e3d 2035 2e33 0a09  .pyyaml >= 5.3..
+000005a0: 7363 696b 6974 2d69 6d61 6765 203e 3d20  scikit-image >= 
+000005b0: 302e 3137 2e31 0a09 7363 6970 7920 3e3d  0.17.1..scipy >=
+000005c0: 2031 2e33 2e32 0a09 7469 6666 6669 6c65   1.3.2..tifffile
+000005d0: 203e 3d20 3230 3139 2e37 2e32 362e 320a   >= 2019.7.26.2.
+000005e0: 0974 7164 6d20 3e3d 2034 2e34 312e 310a  .tqdm >= 4.41.1.
+000005f0: 0976 6972 7475 616c 626f 7820 3e3d 2032  .virtualbox >= 2
+00000600: 2e30 2e30 0a09 7079 7365 7269 616c 656d  .0.0..pyserialem
+00000610: 203e 3d20 302e 332e 320a 0a5b 6f70 7469   >= 0.3.2..[opti
+00000620: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
+00000630: 7265 5d0a 6465 7665 6c6f 7020 3d20 0a09  re].develop = ..
+00000640: 6275 6d70 3276 6572 7369 6f6e 0a09 6368  bump2version..ch
+00000650: 6563 6b2d 6d61 6e69 6665 7374 0a09 7072  eck-manifest..pr
+00000660: 652d 636f 6d6d 6974 0a09 7079 7465 7374  e-commit..pytest
+00000670: 203e 3d20 352e 342e 310a 0970 7974 6573   >= 5.4.1..pytes
+00000680: 742d 636f 7620 3e3d 2032 2e38 2e31 0a73  t-cov >= 2.8.1.s
+00000690: 6572 7661 6c20 3d20 0a09 7365 7276 616c  erval = ..serval
+000006a0: 2d74 6f6f 6c6b 6974 0a0a 5b6f 7074 696f  -toolkit..[optio
+000006b0: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+000006c0: 5d0a 696e 636c 7564 6520 3d20 696e 7374  ].include = inst
+000006d0: 616d 6174 6963 2c20 696e 7374 616d 6174  amatic, instamat
+000006e0: 6963 2e2a 2c20 696e 7374 616d 6174 6963  ic.*, instamatic
+000006f0: 2e65 7870 6572 696d 656e 7473 2e2a 0a0a  .experiments.*..
+00000700: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
+00000710: 6f69 6e74 735d 0a63 6f6e 736f 6c65 5f73  oints].console_s
+00000720: 6372 6970 7473 203d 200a 0969 6e73 7461  cripts = ..insta
+00000730: 6d61 7469 6320 3d20 696e 7374 616d 6174  matic = instamat
+00000740: 6963 2e6d 6169 6e3a 6d61 696e 0a09 696e  ic.main:main..in
+00000750: 7374 616d 6174 6963 2e63 6f6e 7472 6f6c  stamatic.control
+00000760: 6c65 7220 3d20 696e 7374 616d 6174 6963  ler = instamatic
+00000770: 2e54 454d 436f 6e74 726f 6c6c 6572 2e54  .TEMController.T
+00000780: 454d 436f 6e74 726f 6c6c 6572 3a6d 6169  EMController:mai
+00000790: 6e5f 656e 7472 790a 0969 6e73 7461 6d61  n_entry..instama
+000007a0: 7469 632e 7365 7269 616c 6564 203d 2069  tic.serialed = i
+000007b0: 6e73 7461 6d61 7469 632e 6578 7065 7269  nstamatic.experi
+000007c0: 6d65 6e74 732e 7365 7269 616c 6564 2e65  ments.serialed.e
+000007d0: 7870 6572 696d 656e 743a 6d61 696e 0a09  xperiment:main..
+000007e0: 696e 7374 616d 6174 6963 2e63 616d 6572  instamatic.camer
+000007f0: 6120 3d20 696e 7374 616d 6174 6963 2e63  a = instamatic.c
+00000800: 616d 6572 612e 6361 6d65 7261 3a6d 6169  amera.camera:mai
+00000810: 6e5f 656e 7472 790a 0969 6e73 7461 6d61  n_entry..instama
+00000820: 7469 632e 6361 6c69 6272 6174 655f 7374  tic.calibrate_st
+00000830: 6167 655f 6c6f 776d 6167 203d 2069 6e73  age_lowmag = ins
+00000840: 7461 6d61 7469 632e 6361 6c69 6272 6174  tamatic.calibrat
+00000850: 652e 6361 6c69 6272 6174 655f 7374 6167  e.calibrate_stag
+00000860: 655f 6c6f 776d 6167 3a6d 6169 6e5f 656e  e_lowmag:main_en
+00000870: 7472 790a 0969 6e73 7461 6d61 7469 632e  try..instamatic.
+00000880: 6361 6c69 6272 6174 655f 7374 6167 655f  calibrate_stage_
+00000890: 6d61 6731 203d 2069 6e73 7461 6d61 7469  mag1 = instamati
+000008a0: 632e 6361 6c69 6272 6174 652e 6361 6c69  c.calibrate.cali
+000008b0: 6272 6174 655f 7374 6167 655f 6d61 6731  brate_stage_mag1
+000008c0: 3a6d 6169 6e5f 656e 7472 790a 0969 6e73  :main_entry..ins
+000008d0: 7461 6d61 7469 632e 6361 6c69 6272 6174  tamatic.calibrat
+000008e0: 655f 6265 616d 7368 6966 7420 3d20 696e  e_beamshift = in
+000008f0: 7374 616d 6174 6963 2e63 616c 6962 7261  stamatic.calibra
+00000900: 7465 2e63 616c 6962 7261 7465 5f62 6561  te.calibrate_bea
+00000910: 6d73 6869 6674 3a6d 6169 6e5f 656e 7472  mshift:main_entr
+00000920: 790a 0969 6e73 7461 6d61 7469 632e 6361  y..instamatic.ca
+00000930: 6c69 6272 6174 655f 6469 7265 6374 6265  librate_directbe
+00000940: 616d 203d 2069 6e73 7461 6d61 7469 632e  am = instamatic.
+00000950: 6361 6c69 6272 6174 652e 6361 6c69 6272  calibrate.calibr
+00000960: 6174 655f 6469 7265 6374 6265 616d 3a6d  ate_directbeam:m
+00000970: 6169 6e5f 656e 7472 790a 0969 6e73 7461  ain_entry..insta
+00000980: 6d61 7469 632e 6361 6c69 6272 6174 655f  matic.calibrate_
+00000990: 7374 6167 656d 6174 7269 7820 3d20 696e  stagematrix = in
+000009a0: 7374 616d 6174 6963 2e63 616c 6962 7261  stamatic.calibra
+000009b0: 7465 2e63 616c 6962 7261 7465 5f73 7461  te.calibrate_sta
+000009c0: 6765 6d61 7472 6978 3a6d 6169 6e5f 656e  gematrix:main_en
+000009d0: 7472 790a 0969 6e73 7461 6d61 7469 632e  try..instamatic.
+000009e0: 666c 6174 6669 656c 6420 3d20 696e 7374  flatfield = inst
+000009f0: 616d 6174 6963 2e70 726f 6365 7373 696e  amatic.processin
+00000a00: 672e 666c 6174 6669 656c 643a 6d61 696e  g.flatfield:main
+00000a10: 5f65 6e74 7279 0a09 696e 7374 616d 6174  _entry..instamat
+00000a20: 6963 2e73 7472 6574 6368 5f63 6f72 7265  ic.stretch_corre
+00000a30: 6374 696f 6e20 3d20 696e 7374 616d 6174  ction = instamat
+00000a40: 6963 2e70 726f 6365 7373 696e 672e 7374  ic.processing.st
+00000a50: 7265 7463 685f 636f 7272 6563 7469 6f6e  retch_correction
+00000a60: 3a6d 6169 6e5f 656e 7472 790a 0969 6e73  :main_entry..ins
+00000a70: 7461 6d61 7469 632e 6272 6f77 7365 7220  tamatic.browser 
+00000a80: 3d20 7363 7269 7074 732e 6272 6f77 7365  = scripts.browse
+00000a90: 723a 6d61 696e 0a09 696e 7374 616d 6174  r:main..instamat
+00000aa0: 6963 2e76 6965 7765 7220 3d20 7363 7269  ic.viewer = scri
+00000ab0: 7074 732e 7669 6577 6572 3a6d 6169 6e0a  pts.viewer:main.
+00000ac0: 0969 6e73 7461 6d61 7469 632e 6465 666f  .instamatic.defo
+00000ad0: 6375 735f 6865 6c70 6572 203d 2069 6e73  cus_helper = ins
+00000ae0: 7461 6d61 7469 632e 6775 692e 6465 666f  tamatic.gui.defo
+00000af0: 6375 735f 6275 7474 6f6e 3a6d 6169 6e0a  cus_button:main.
+00000b00: 0969 6e73 7461 6d61 7469 632e 6669 6e64  .instamatic.find
+00000b10: 5f63 7279 7374 616c 7320 3d20 696e 7374  _crystals = inst
+00000b20: 616d 6174 6963 2e70 726f 6365 7373 696e  amatic.processin
+00000b30: 672e 6669 6e64 5f63 7279 7374 616c 733a  g.find_crystals:
+00000b40: 6d61 696e 5f65 6e74 7279 0a09 696e 7374  main_entry..inst
+00000b50: 616d 6174 6963 2e66 696e 645f 6372 7973  amatic.find_crys
+00000b60: 7461 6c73 5f69 6c61 7374 696b 203d 2069  tals_ilastik = i
+00000b70: 6e73 7461 6d61 7469 632e 7072 6f63 6573  nstamatic.proces
+00000b80: 7369 6e67 2e66 696e 645f 6372 7973 7461  sing.find_crysta
+00000b90: 6c73 5f69 6c61 7374 696b 3a6d 6169 6e5f  ls_ilastik:main_
+00000ba0: 656e 7472 790a 0969 6e73 7461 6d61 7469  entry..instamati
+00000bb0: 632e 6c65 6172 6e20 3d20 7363 7269 7074  c.learn = script
+00000bc0: 732e 6c65 6172 6e3a 6d61 696e 5f65 6e74  s.learn:main_ent
+00000bd0: 7279 0a09 696e 7374 616d 6174 6963 2e74  ry..instamatic.t
+00000be0: 656d 7365 7276 6572 203d 2069 6e73 7461  emserver = insta
+00000bf0: 6d61 7469 632e 7365 7276 6572 2e74 656d  matic.server.tem
+00000c00: 5f73 6572 7665 723a 6d61 696e 0a09 696e  _server:main..in
+00000c10: 7374 616d 6174 6963 2e63 616d 7365 7276  stamatic.camserv
+00000c20: 6572 203d 2069 6e73 7461 6d61 7469 632e  er = instamatic.
+00000c30: 7365 7276 6572 2e63 616d 5f73 6572 7665  server.cam_serve
+00000c40: 723a 6d61 696e 0a09 696e 7374 616d 6174  r:main..instamat
+00000c50: 6963 2e64 6961 6c73 7365 7276 6572 203d  ic.dialsserver =
+00000c60: 2069 6e73 7461 6d61 7469 632e 7365 7276   instamatic.serv
+00000c70: 6572 2e64 6961 6c73 5f73 6572 7665 723a  er.dials_server:
+00000c80: 6d61 696e 0a09 696e 7374 616d 6174 6963  main..instamatic
+00000c90: 2e56 4d73 6572 7665 7220 3d20 696e 7374  .VMserver = inst
+00000ca0: 616d 6174 6963 2e73 6572 7665 722e 766d  amatic.server.vm
+00000cb0: 5f75 6275 6e74 755f 7365 7276 6572 3a6d  _ubuntu_server:m
+00000cc0: 6169 6e0a 0969 6e73 7461 6d61 7469 632e  ain..instamatic.
+00000cd0: 7864 7373 6572 7665 7220 3d20 696e 7374  xdsserver = inst
+00000ce0: 616d 6174 6963 2e73 6572 7665 722e 7864  amatic.server.xd
+00000cf0: 735f 7365 7276 6572 3a6d 6169 6e0a 0969  s_server:main..i
+00000d00: 6e73 7461 6d61 7469 632e 7465 6d73 6572  nstamatic.temser
+00000d10: 7665 725f 6665 6920 3d20 696e 7374 616d  ver_fei = instam
+00000d20: 6174 6963 2e73 6572 7665 722e 5445 4d53  atic.server.TEMS
+00000d30: 6572 7665 725f 4645 493a 6d61 696e 0a09  erver_FEI:main..
+00000d40: 696e 7374 616d 6174 6963 2e67 6f6e 696f  instamatic.gonio
+00000d50: 746f 6f6c 7365 7276 6572 203d 2069 6e73  toolserver = ins
+00000d60: 7461 6d61 7469 632e 7365 7276 6572 2e67  tamatic.server.g
+00000d70: 6f6e 696f 746f 6f6c 5f73 6572 7665 723a  oniotool_server:
+00000d80: 6d61 696e 0a09 696e 7374 616d 6174 6963  main..instamatic
+00000d90: 2e61 7574 6f63 6f6e 6669 6720 3d20 696e  .autoconfig = in
+00000da0: 7374 616d 6174 6963 2e63 6f6e 6669 672e  stamatic.config.
+00000db0: 6175 746f 636f 6e66 6967 3a6d 6169 6e0a  autoconfig:main.
+00000dc0: 0a5b 6567 675f 696e 666f 5d0a 7461 675f  .[egg_info].tag_
+00000dd0: 6275 696c 6420 3d20 0a74 6167 5f64 6174  build = .tag_dat
+00000de0: 6520 3d20 300a 0a                        e = 0..
```

### Comparing `instamatic-1.8.0/tests/config/calibration/test.yaml` & `instamatic-1.9.0/tests/config/calibration/test.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/tests/config/microscope/test.yaml` & `instamatic-1.9.0/tests/config/microscope/test.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.8.0/tests/test_ctrl.py` & `instamatic-1.9.0/tests/test_ctrl.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-import numpy as np
-import pytest
-
-
-def test_setup(ctrl):
-    from instamatic import TEMController
-
-    ctrl2 = TEMController.get_instance()
-    assert ctrl2 is ctrl
-
-
-def test_other(ctrl):
-    ctrl.spotsize = 1
-    assert ctrl.spotsize == 1
-
-    stagematrix = ctrl.get_stagematrix()
-    assert stagematrix.shape == (2, 2)
-
-    ctrl.store('test1')
-    ctrl.restore('test1')
-
-    ctrl.mode.set('diff')
-    ctrl.store_diff_beam()
-
-    ctrl.mode.set('mag1')
-    with pytest.raises(Exception):
-        ctrl.store_diff()
-
-
-def test_stage(ctrl):
-    stage = ctrl.stage
-
-    pos = stage.get()
-    assert isinstance(pos, tuple)
-    assert len(pos) == 5
-
-    stage.neutral()
-    assert stage.xy == (0, 0)
-
-    stage.x = 100
-    assert stage.x == 100
-    stage.y = -100
-    assert stage.y == -100
-    stage.z = 10
-    assert stage.z == 10
-    stage.a = 1
-    assert stage.a == 1
-    stage.b = -1
-    assert stage.b == -1
-
-    stage.xy = (0, 0)
-    assert stage.xy == (0, 0)
-
-    stage.set_a_with_speed(45, speed=12, wait=True)
-    assert not stage.is_moving()
-
-    assert stage.a == 45
-
-    stage.set(x=0, y=0, z=0)
-    stage.move_in_projection(delta_x=1, delta_y=1)
-
-    assert abs(stage.y) + abs(stage.z) == pytest.approx(np.sqrt(2))
-    assert stage.x == 1
-
-    stage.set(x=0, y=0, z=0)
-    stage.move_along_optical_axis(1)
-    assert abs(stage.y) + abs(stage.z) == pytest.approx(np.sqrt(2))
-
-    stage.xy = (0, 0)
-    stage.move_xy_with_backlash_correction(shift_x=100, shift_y=100)
-    assert stage.xy == (100, 100)
-    stage.move_xy_with_backlash_correction(shift_x=-100, shift_y=-100)
-    assert stage.xy == (0, 0)
-
-    stage.eliminate_backlash_a()
-    stage.eliminate_backlash_xy()
-
-    with pytest.raises(TypeError):
-        stage.set('rawr')
-
-
-def test_deflectors(ctrl):
-    for deflector in (
-        ctrl.guntilt,
-        ctrl.beamshift,
-        ctrl.beamtilt,
-        ctrl.diffshift,
-        ctrl.imageshift1,
-        ctrl.imageshift2,
-    ):
-        val = deflector.get()
-        assert len(val) == 2
-        assert isinstance(val, tuple)
-
-        deflector.x = 100
-        deflector.y = 200
-        assert deflector.x == 100
-        assert deflector.y == 200
-        assert deflector.xy == (100, 200)
-
-        deflector.xy = (10, 20)
-        assert deflector.xy == (10, 20)
-
-        deflector.neutral()
-
-    with pytest.raises(TypeError):
-        deflector.set('rawr')
-
-
-def test_magnification(ctrl):
-    lens = ctrl.magnification
-
-    lens.index = 0
-    assert lens.index == 0
-    lens.increase()
-    assert lens.index == 1
-    mag = lens.value
-    assert isinstance(mag, int)
-
-    lens.decrease()
-    assert lens.index == 0
-    lens.set(mag)
-    assert lens.index == 1
-
-    assert isinstance(lens.absolute_index, int)
-
-    with pytest.raises(ValueError):
-        lens.set(-1)
-
-    ranges = lens.get_ranges()
-    assert isinstance(ranges, dict)
-    assert 'lowmag' in ranges
-    assert 'mag1' in ranges
-    assert 'diff' in ranges
-
-
-def test_difffocus(ctrl):
-    lens = ctrl.difffocus
-
-    ctrl.mode.set('mag1')
-    with pytest.raises(ValueError):
-        val = lens.get()
-
-    ctrl.mode.set('diff')
-
-    lens.value = 0
-    val = lens.get()
-    assert isinstance(val, int)
-    assert val == 0
-
-    defocus_val = 1500
-    lens.defocus(defocus_val)
-    assert lens.value == defocus_val
-    assert lens.is_defocused
-    lens.refocus()
-    assert lens.value == 0
-    assert not lens.is_defocused
-
-    ctrl.mode.set('mag1')
-
-
-def test_brightness(ctrl):
-    lens = ctrl.brightness
-    lens.max()  # set to max
-    lens.min()  # set to 0
-    val = lens.get()
-    assert isinstance(val, int)
-    assert val == 0
-
-    lens.value = 100
-    assert lens.value == 100
-
-
-def test_beam(ctrl):
-    beam = ctrl.beam
-    unblanked = 'unblanked'
-
-    beam.unblank()
-    assert beam.get() == unblanked
-
-    beam.blank()
-    assert beam.is_blanked
-
-    beam.set(unblanked)
-    assert beam.state == unblanked
-
-    with pytest.raises(ValueError):
-        beam.set('rawr')
-
-
-def test_mode(ctrl):
-    mode = ctrl.mode
-
-    mode.set('diff')
-    assert mode == 'diff'
-    mode.set('lowmag')
-    assert mode == 'lowmag'
-
-    mode.set('mag1')
-    assert mode == 'mag1'
-
-    with pytest.raises(ValueError):
-        mode.set('rawr')
-
-
-def test_screen(ctrl):
-    screen = ctrl.screen
-
-    screen.down()
-    screen.up()
-    assert screen.is_up
-
-    screen.down()
-    assert screen.get() == 'down'
-    assert screen.get() != 'up'
-
-    with pytest.raises(ValueError):
-        screen.set('rawr')
-
-
-def test_align_to(ctrl):
-    reference = ctrl.get_raw_image()
-    pos = ctrl.stage.xy
-
-    shift = ctrl.align_to(reference, apply=True)
-
-    assert len(shift) == 2
-    assert pos != ctrl.stage.xy
-
-
-if __name__ == '__main__':
-    test_ctrl()
-
-    from IPython import embed
-    embed(banner1='')
+import numpy as np
+import pytest
+
+
+def test_setup(ctrl):
+    from instamatic import TEMController
+
+    ctrl2 = TEMController.get_instance()
+    assert ctrl2 is ctrl
+
+
+def test_other(ctrl):
+    ctrl.spotsize = 1
+    assert ctrl.spotsize == 1
+
+    stagematrix = ctrl.get_stagematrix()
+    assert stagematrix.shape == (2, 2)
+
+    ctrl.store('test1')
+    ctrl.restore('test1')
+
+    ctrl.mode.set('diff')
+    ctrl.store_diff_beam()
+
+    ctrl.mode.set('mag1')
+    with pytest.raises(Exception):
+        ctrl.store_diff()
+
+
+def test_stage(ctrl):
+    stage = ctrl.stage
+
+    pos = stage.get()
+    assert isinstance(pos, tuple)
+    assert len(pos) == 5
+
+    stage.neutral()
+    assert stage.xy == (0, 0)
+
+    stage.x = 100
+    assert stage.x == 100
+    stage.y = -100
+    assert stage.y == -100
+    stage.z = 10
+    assert stage.z == 10
+    stage.a = 1
+    assert stage.a == 1
+    stage.b = -1
+    assert stage.b == -1
+
+    stage.xy = (0, 0)
+    assert stage.xy == (0, 0)
+
+    stage.set_a_with_speed(45, speed=12, wait=True)
+    assert not stage.is_moving()
+
+    assert stage.a == 45
+
+    stage.set(x=0, y=0, z=0)
+    stage.move_in_projection(delta_x=1, delta_y=1)
+
+    assert abs(stage.y) + abs(stage.z) == pytest.approx(np.sqrt(2))
+    assert stage.x == 1
+
+    stage.set(x=0, y=0, z=0)
+    stage.move_along_optical_axis(1)
+    assert abs(stage.y) + abs(stage.z) == pytest.approx(np.sqrt(2))
+
+    stage.xy = (0, 0)
+    stage.move_xy_with_backlash_correction(shift_x=100, shift_y=100)
+    assert stage.xy == (100, 100)
+    stage.move_xy_with_backlash_correction(shift_x=-100, shift_y=-100)
+    assert stage.xy == (0, 0)
+
+    stage.eliminate_backlash_a()
+    stage.eliminate_backlash_xy()
+
+    with pytest.raises(TypeError):
+        stage.set('rawr')
+
+
+def test_deflectors(ctrl):
+    for deflector in (
+        ctrl.guntilt,
+        ctrl.beamshift,
+        ctrl.beamtilt,
+        ctrl.diffshift,
+        ctrl.imageshift1,
+        ctrl.imageshift2,
+    ):
+        val = deflector.get()
+        assert len(val) == 2
+        assert isinstance(val, tuple)
+
+        deflector.x = 100
+        deflector.y = 200
+        assert deflector.x == 100
+        assert deflector.y == 200
+        assert deflector.xy == (100, 200)
+
+        deflector.xy = (10, 20)
+        assert deflector.xy == (10, 20)
+
+        deflector.neutral()
+
+    with pytest.raises(TypeError):
+        deflector.set('rawr')
+
+
+def test_magnification(ctrl):
+    lens = ctrl.magnification
+
+    lens.index = 0
+    assert lens.index == 0
+    lens.increase()
+    assert lens.index == 1
+    mag = lens.value
+    assert isinstance(mag, int)
+
+    lens.decrease()
+    assert lens.index == 0
+    lens.set(mag)
+    assert lens.index == 1
+
+    assert isinstance(lens.absolute_index, int)
+
+    with pytest.raises(ValueError):
+        lens.set(-1)
+
+    ranges = lens.get_ranges()
+    assert isinstance(ranges, dict)
+    assert 'lowmag' in ranges
+    assert 'mag1' in ranges
+    assert 'diff' in ranges
+
+
+def test_difffocus(ctrl):
+    lens = ctrl.difffocus
+
+    ctrl.mode.set('mag1')
+    with pytest.raises(ValueError):
+        val = lens.get()
+
+    ctrl.mode.set('diff')
+
+    lens.value = 0
+    val = lens.get()
+    assert isinstance(val, int)
+    assert val == 0
+
+    defocus_val = 1500
+    lens.defocus(defocus_val)
+    assert lens.value == defocus_val
+    assert lens.is_defocused
+    lens.refocus()
+    assert lens.value == 0
+    assert not lens.is_defocused
+
+    ctrl.mode.set('mag1')
+
+
+def test_brightness(ctrl):
+    lens = ctrl.brightness
+    lens.max()  # set to max
+    lens.min()  # set to 0
+    val = lens.get()
+    assert isinstance(val, int)
+    assert val == 0
+
+    lens.value = 100
+    assert lens.value == 100
+
+
+def test_beam(ctrl):
+    beam = ctrl.beam
+    unblanked = 'unblanked'
+
+    beam.unblank()
+    assert beam.get() == unblanked
+
+    beam.blank()
+    assert beam.is_blanked
+
+    beam.set(unblanked)
+    assert beam.state == unblanked
+
+    with pytest.raises(ValueError):
+        beam.set('rawr')
+
+
+def test_mode(ctrl):
+    mode = ctrl.mode
+
+    mode.set('diff')
+    assert mode == 'diff'
+    mode.set('lowmag')
+    assert mode == 'lowmag'
+
+    mode.set('mag1')
+    assert mode == 'mag1'
+
+    with pytest.raises(ValueError):
+        mode.set('rawr')
+
+
+def test_screen(ctrl):
+    screen = ctrl.screen
+
+    screen.down()
+    screen.up()
+    assert screen.is_up
+
+    screen.down()
+    assert screen.get() == 'down'
+    assert screen.get() != 'up'
+
+    with pytest.raises(ValueError):
+        screen.set('rawr')
+
+
+def test_align_to(ctrl):
+    reference = ctrl.get_raw_image()
+    pos = ctrl.stage.xy
+
+    shift = ctrl.align_to(reference, apply=True)
+
+    assert len(shift) == 2
+    assert pos != ctrl.stage.xy
+
+
+if __name__ == '__main__':
+    test_ctrl()
+
+    from IPython import embed
+    embed(banner1='')
```

### Comparing `instamatic-1.8.0/tests/test_experiments.py` & `instamatic-1.9.0/tests/test_experiments.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-import tempfile
-import threading
-from unittest.mock import MagicMock
-
-
-def test_cred(ctrl):
-    """This one is difficult to test with threads and events."""
-    from instamatic.experiments import cred
-
-    stopEvent = threading.Event()
-    stopEvent.set()
-
-    tempdrc = tempfile.TemporaryDirectory()
-    expdir = tempdrc.name
-
-    logger = MagicMock()
-
-    cexp = cred.experiment.Experiment(
-        ctrl,
-        path=expdir,
-        stop_event=stopEvent,
-        log=logger,
-        mode='simulate',
-    )
-    cexp.start_collection()
-
-    tempdrc.cleanup()
-
-
-def test_cred_tvips(ctrl):
-    from instamatic.experiments import cRED_tvips
-
-    tempdrc = tempfile.TemporaryDirectory()
-    expdir = tempdrc.name
-
-    logger = MagicMock()
-
-    ctrl.stage.a = 20
-    target_angle = -20
-    exposure = 0.1
-    manual_control = False
-    mode = 'diff'
-
-    exp = cRED_tvips.Experiment(
-        ctrl=ctrl,
-        path=expdir,
-        log=logger,
-        mode=mode,
-        track=None,
-        exposure=exposure,
-    )
-    exp.get_ready()
-
-    exp.start_collection(
-        target_angle=target_angle,
-        manual_control=manual_control,
-    )
-
-    tempdrc.cleanup()
-
-
-def test_red(ctrl):
-    from instamatic.experiments import RED
-
-    tempdrc = tempfile.TemporaryDirectory()
-    expdir = tempdrc.name
-
-    logger = MagicMock()
-
-    exposure_time = 0.01
-    tilt_range = 5
-    stepsize = 1.0
-
-    red_exp = RED.Experiment(
-        ctrl=ctrl,
-        path=expdir,
-        log=logger,
-        flatfield=None,
-    )
-
-    for x in range(2):
-        red_exp.start_collection(
-            exposure_time=exposure_time,
-            tilt_range=tilt_range,
-            stepsize=stepsize,
-        )
-
-    red_exp.finalize()
-
-    tempdrc.cleanup()
+import tempfile
+import threading
+from unittest.mock import MagicMock
+
+
+def test_cred(ctrl):
+    """This one is difficult to test with threads and events."""
+    from instamatic.experiments import cred
+
+    stopEvent = threading.Event()
+    stopEvent.set()
+
+    tempdrc = tempfile.TemporaryDirectory()
+    expdir = tempdrc.name
+
+    logger = MagicMock()
+
+    cexp = cred.experiment.Experiment(
+        ctrl,
+        path=expdir,
+        stop_event=stopEvent,
+        log=logger,
+        mode='simulate',
+    )
+    cexp.start_collection()
+
+    tempdrc.cleanup()
+
+
+def test_cred_tvips(ctrl):
+    from instamatic.experiments import cRED_tvips
+
+    tempdrc = tempfile.TemporaryDirectory()
+    expdir = tempdrc.name
+
+    logger = MagicMock()
+
+    ctrl.stage.a = 20
+    target_angle = -20
+    exposure = 0.1
+    manual_control = False
+    mode = 'diff'
+
+    exp = cRED_tvips.Experiment(
+        ctrl=ctrl,
+        path=expdir,
+        log=logger,
+        mode=mode,
+        track=None,
+        exposure=exposure,
+    )
+    exp.get_ready()
+
+    exp.start_collection(
+        target_angle=target_angle,
+        manual_control=manual_control,
+    )
+
+    tempdrc.cleanup()
+
+
+def test_red(ctrl):
+    from instamatic.experiments import RED
+
+    tempdrc = tempfile.TemporaryDirectory()
+    expdir = tempdrc.name
+
+    logger = MagicMock()
+
+    exposure_time = 0.01
+    tilt_range = 5
+    stepsize = 1.0
+
+    red_exp = RED.Experiment(
+        ctrl=ctrl,
+        path=expdir,
+        log=logger,
+        flatfield=None,
+    )
+
+    for x in range(2):
+        red_exp.start_collection(
+            exposure_time=exposure_time,
+            tilt_range=tilt_range,
+            stepsize=stepsize,
+        )
+
+    red_exp.finalize()
+
+    tempdrc.cleanup()
```

### Comparing `instamatic-1.8.0/tests/test_formats.py` & `instamatic-1.9.0/tests/test_formats.py`

 * *Files identical despite different names*

