# Comparing `tmp/MAVProxy-1.8.8.tar.gz` & `tmp/MAVProxy-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MAVProxy-1.8.8.tar", last modified: Tue Jun 11 02:15:52 2019, max compression
+gzip compressed data, was "dist/MAVProxy-1.8.9.tar", last modified: Mon Jul 29 06:27:52 2019, max compression
```

## Comparing `MAVProxy-1.8.8.tar` & `MAVProxy-1.8.9.tar`

### file list

```diff
@@ -1,644 +1,649 @@
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)       48 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/__init__.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/tools/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/tools/graphs/
--rw-r--r--   0 tridge    (1000) tridge    (1000)    13435 2019-06-11 02:14:43.000000 MAVProxy-1.8.8/MAVProxy/tools/graphs/mavgraphs.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    12462 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/tools/graphs/ekf3Graphs.xml
--rw-r--r--   0 tridge    (1000) tridge    (1000)    12798 2019-06-11 02:14:27.000000 MAVProxy-1.8.8/MAVProxy/tools/graphs/ekfGraphs.xml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    13109 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/tools/graphs/mavgraphs2.xml
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    23547 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/tools/MAVExplorer.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    20958 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/tools/mavflightview.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     8632 2018-06-08 00:11:39.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_log.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)       16 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/__init__.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     2826 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_DGPS.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     4800 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_horizon.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5670 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_HIL.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3935 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_nsh.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3768 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_relay.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     4375 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_help.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     4229 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_output.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5823 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_battery.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     4632 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_checklist.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3456 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_auxopt.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3940 2018-06-20 08:21:08.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_system_time.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cmac_check/
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    12492 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cmac_check/__init__.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)      962 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cmac_check/cmac-foamy-mission-ccw.txt
--rw-r--r--   0 tridge    (1000) tridge    (1000)      132 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cmac_check/cmac-foamy-fence.txt
--rw-r--r--   0 tridge    (1000) tridge    (1000)       59 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cmac_check/cmac-foamy-rally.txt
--rw-r--r--   0 tridge    (1000) tridge    (1000)      962 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cmac_check/cmac-foamy-mission-cw.txt
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5429 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_GPSInput.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     4391 2018-09-30 22:36:33.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_sensors.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5821 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_followtest.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    19230 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/__init__.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    31204 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/sc_SonyQX1.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     7912 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/sc_main.py
--rwxrwxr-x   0 tridge    (1000) tridge    (1000)     4930 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/sc_ExifWriter.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     6701 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/sc_video.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5119 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/sc_config.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3303 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/sc_webcam.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2252 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/ssdp.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5954 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_gasheli.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3750 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_rcsetup.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3070 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_ppp.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1690 2018-09-07 09:01:39.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_message.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     9183 2018-10-15 07:15:05.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/__init__.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)        0 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/__init__.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      275 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/mavcesium_default.ini
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/templates/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1476 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/templates/settings_menu.html
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     4873 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/templates/index.html
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1428 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/templates/settings_general.html
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      104 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/templates/settings_model.html
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1497 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/templates/context_menu.html
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2322 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/config.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      886 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/lighterShared.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/BaseLayerPicker/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      620 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/BaseLayerPicker/lighter.css
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2001 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/BaseLayerPicker/BaseLayerPicker.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Timeline/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      336 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Timeline/lighter.css
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1354 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Timeline/Timeline.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/InfoBox/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3045 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/InfoBox/InfoBoxDescription.css
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1579 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/InfoBox/InfoBox.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Animation/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1701 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Animation/lighter.css
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2355 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Animation/Animation.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Geocoder/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      397 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Geocoder/lighter.css
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1537 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Geocoder/Geocoder.css
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5099 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/lighter.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/FullscreenButton/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      102 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/FullscreenButton/FullscreenButton.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/SelectionIndicator/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      338 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/SelectionIndicator/SelectionIndicator.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Cesium3DTilesInspector/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2574 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Cesium3DTilesInspector/Cesium3DTilesInspector.css
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1546 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/shared.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/ProjectionPicker/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1046 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/ProjectionPicker/ProjectionPicker.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Viewer/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1367 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Viewer/Viewer.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/NavigationHelpButton/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      890 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/NavigationHelpButton/lighter.css
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1722 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/NavigationHelpButton/NavigationHelpButton.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/PerformanceWatchdog/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      256 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/PerformanceWatchdog/PerformanceWatchdog.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/SceneModePicker/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1582 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/SceneModePicker/SceneModePicker.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TerrainProviders/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     6173 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TerrainProviders/Ellipsoid.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     4482 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TerrainProviders/STK.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      781 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TimelineIcons.png
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    11575 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/esriWorldImagery.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     7491 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/naturalEarthII.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     7270 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapboxStreets.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     9943 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/bingAerial.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2663 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/openStreetMap.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     4119 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/stamenToner.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    11555 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/esriNationalGeographic.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     8076 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/bingRoads.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     8300 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapboxTerrain.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    10374 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/bingAerialLabels.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     8501 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/esriWorldStreetMap.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    11342 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapQuestOpenStreetMap.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     9242 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapboxSatellite.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5836 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/blackMarble.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    10806 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/stamenWatercolor.png
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5555 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchZoom.svg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5706 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/Mouse.svg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5654 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/MouseMiddle.svg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5647 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/MouseRight.svg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5701 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchRotate.svg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     6416 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchDrag.svg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5656 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/MouseLeft.svg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5996 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchTilt.svg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3565 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/Touch.svg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      723 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/info-loading.gif
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumWidget/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      269 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumWidget/lighter.css
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1006 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumWidget/CesiumWidget.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/VRButton/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)       94 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/VRButton/VRButton.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumInspector/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1970 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumInspector/CesiumInspector.css
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    22424 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/widgets.css
--rw-rw-r--   0 tridge    (1000) tridge    (1000)  2786998 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Cesium.js
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    18309 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/cesiumWorkerBootstrapper.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   124421 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolylineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    95272 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createSphereGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   193321 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/transcodeCRNToDXT.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   100382 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipseOutlineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   203242 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCorridorGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   111067 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createFrustumGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   163149 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createRectangleGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   184068 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createVerticesFromGoogleEarthEnterpriseBuffer.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   219814 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolygonGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   113295 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createFrustumOutlineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    94573 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCylinderGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   139600 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   185374 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/upsampleQuantizedTerrainMesh.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   182327 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createVerticesFromHeightmap.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   139351 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/combineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    89849 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createSphereOutlineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    32071 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/decodeGoogleEarthEnterprisePacket.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    91793 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCylinderOutlineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   190159 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolylineVolumeOutlineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   194480 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCorridorOutlineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    87453 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createBoxOutlineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1048 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/transferTypedArrayTest.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   121961 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createSimplePolylineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    92852 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createBoxGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   181378 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createVerticesFromQuantizedTerrainMesh.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   187463 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createWallGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   205356 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCircleGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    94321 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipsoidGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    88928 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipsoidOutlineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   203374 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipseGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   184551 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createWallOutlineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   107464 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createRectangleOutlineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   211473 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolygonOutlineGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   220382 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolylineVolumeGeometry.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   101776 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCircleOutlineGeometry.js
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/ThirdParty/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/ThirdParty/Workers/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    19929 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/ThirdParty/Workers/deflate.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    24593 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/ThirdParty/Workers/inflate.js
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    67428 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_0.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    65311 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_18.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    66408 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_3.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    65711 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_15.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    64664 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_12.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    65547 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_14.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    65594 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_6.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    65312 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_26.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    67315 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_1.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    65854 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_13.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    64955 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_25.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    65903 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_4.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    64979 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_22.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    65331 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_20.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    64845 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_21.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    65012 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_11.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    65986 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_10.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    27598 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_27.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    65539 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_19.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    66086 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_23.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    66859 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_9.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    65624 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_17.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    66932 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_8.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    64896 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_24.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    67101 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_7.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    66031 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_16.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    67804 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_2.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    65381 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_5.json
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   528939 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/approximateTerrainHeights.json
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/0/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    12067 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/0/0.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/1/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    14055 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/1/0.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    12957 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/1.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     9032 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/0.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    11859 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/3.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    11362 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/2.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    10234 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/1.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     9531 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/0.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    10754 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/3.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    11678 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/2.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    12265 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/1.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     8474 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/0.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    11888 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/3.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    16477 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/2.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     9307 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/1.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     8157 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/0.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    10341 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/3.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     7891 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/2.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    12456 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/1.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    10657 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/0.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    14940 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/3.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    12262 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/2.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    10274 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/1.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     7540 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/0.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    11877 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/3.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    16112 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/2.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     6850 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/1.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     7852 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/0.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    15862 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/3.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    11581 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/2.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    11564 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/1.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     6636 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/0.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    12756 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/3.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    16411 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/2.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      794 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/tilemapresource.xml
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/3/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    13262 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/3/1.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    10532 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/3/0.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/0/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    11399 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/0/1.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     7278 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/0/0.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/2/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    15312 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/2/1.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     9643 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/2/0.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/1/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    13142 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/1/1.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    10652 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/1/0.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2411 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/water.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2703 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/star.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2407 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/laundry.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2714 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bakery.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1765 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/building.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2595 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/america-football.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1425 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/grocery.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2979 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/london-underground.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2228 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/fire-station.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1312 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/roadblock.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1188 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/airfield.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1293 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/alcohol-shop.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      788 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/city.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2411 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/campsite.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2249 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-metro.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3610 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cesium.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2816 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-light.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2681 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/zoo.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2502 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/college.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2284 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/park2.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      936 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bank.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1999 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/golf.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1533 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/emergency-telephone.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1907 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/minefield.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      582 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/square.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2194 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/police.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2420 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/soccer.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3146 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/dog-park.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1838 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/baseball.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1606 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/gift.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2106 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/swimming.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2879 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/ferry.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2048 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/harbor.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1371 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/music.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3159 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/art-gallery.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1092 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/industrial.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1702 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/telephone.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1554 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/airport.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1996 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-underground.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3989 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bicycle.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2145 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/village.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1518 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cafe.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3301 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/hairdresser.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1318 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/basketball.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      650 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/square-stroked.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2384 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/religious-jewish.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2499 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/restaurant.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3345 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/skiing.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1908 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/warehouse.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1474 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/mobilephone.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1376 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/monument.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1498 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/car.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2073 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2057 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/garden.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1658 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/tennis.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2005 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/town-hall.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1378 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/logging.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3357 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/oil-well.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1403 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/beer.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2942 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/scooter.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1772 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/polling-place.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      909 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/hospital.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2137 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/triangle.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1307 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/entrance.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1273 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/post.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3838 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/school.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1435 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bar.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1355 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/library.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3460 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/star-stroked.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2258 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/pharmacy.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2059 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/heliport.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2448 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/marker.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2429 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/danger.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1603 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/chemist.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1917 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/waste-basket.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1745 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/heart.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1677 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cricket.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      967 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cemetery.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1976 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/camera.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      998 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bus.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2578 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/museum.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2037 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/clothing-store.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1111 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/place-of-worship.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2151 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/wetland.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1002 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/commercial.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1563 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/parking-garage.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2019 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/fast-food.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1125 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/town.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2917 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/toilets.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2126 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/circle-stroked.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1680 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/embassy.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2270 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/slaughterhouse.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1459 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/circle.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3233 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/theatre.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1888 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cross.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2071 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-above.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1686 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/farm.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1602 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/ice-cream.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1129 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/suitcase.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      948 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/religious-christian.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3414 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/marker-stroked.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1703 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/dam.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3856 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/playground.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3925 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/religious-muslim.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3288 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/pitch.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1773 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/land-use.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2837 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/triangle-stroked.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1250 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/parking.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1371 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/prison.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1944 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/lighthouse.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2059 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/park.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1362 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/lodging.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1544 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/shop.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1741 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/fuel.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1492 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cinema.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1653 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rocket.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3437 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/disability.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   294196 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/waterNormals.jpg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   168640 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_pz.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   138551 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_px.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   134462 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_mx.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   168829 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_py.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   183677 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_mz.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   167849 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_my.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    34121 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/waterNormalsSmall.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    18196 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/moonSmall.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      348 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/pin.svg
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      722 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/favicon-32x32.png
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1905 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/cesium.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/third_party/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      237 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/third_party/tether.min.css
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    31018 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/third_party/font-awesome.min.css
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   150952 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/third_party/bootstrap.min.css
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    19176 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/blu-blank.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    18905 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/ylw-blank.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    18816 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/R.png
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2341 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/websocket.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    25412 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/hud.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      274 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/util.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2305 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/cesium_setup.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2457 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/wp.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3598 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/context_menu.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1049 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/settings.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    34111 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/core.js
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    24632 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/tether.min.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    46654 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/bootstrap.min.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    86659 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/jquery-3.2.1.min.js
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    77160 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.woff2
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   165742 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   165548 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   444379 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   134808 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/FontAwesome.otf
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    98024 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.woff
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/pointers/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1176 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/pointers/move.png
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/models/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   346955 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/models/rat.gltf
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    10339 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/models/rat.glb
--rw-rw-r--   0 tridge    (1000) tridge    (1000)       12 2016-07-28 07:03:42.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/api_keys.txt~
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     8176 2018-10-15 07:15:05.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/cesium_web_server.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     8176 2017-11-12 22:28:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/cesium_web_server.py~
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3755 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_signing.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3033 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_serial.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     3210 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_example.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    34951 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_wp.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1295 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_msg.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    12715 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_rally.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2280 2014-05-17 03:17:49.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_GPS.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     5230 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_heliplane.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     4721 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_graph.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     5314 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_restserver.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1119 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_timesync.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     8232 2018-09-07 09:01:39.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_tracker.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    18022 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_param.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2964 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_gopro.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/
--rw-r--r--   0 tridge    (1000) tridge    (1000)     6732 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/__init__.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    31024 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/magical_ui.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3043 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/glrenderer.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     8116 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/wxvehicle.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/data/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      683 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/data/quadcopter.mtl
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     9420 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/data/arrow.obj
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   456031 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/data/quadcopter.obj
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      422 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/data/arrow.mtl
--rw-r--r--   0 tridge    (1000) tridge    (1000)     8622 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/wxgeodesicgrid.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1389 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_test.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    15488 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cmdlong.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2060 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_antenna.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2951 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mode.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      926 2018-09-30 22:36:33.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_layout.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    13029 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_dataflash_logger.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    12594 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_firmware.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    10362 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_adsb.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    12739 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_fence.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/
--rw-r--r--   0 tridge    (1000) tridge    (1000)    37537 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/__init__.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     9339 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/mp_slipmap.py
--rwxrwxr-x   0 tridge    (1000) tridge    (1000)     3983 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/mp_elevation.py
--rwxrwxr-x   0 tridge    (1000) tridge    (1000)     1479 2016-04-27 06:39:39.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/elev_check.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    22787 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/mp_slipmap_util.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1658 2018-09-30 22:36:33.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/hawk.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      287 2018-06-08 00:11:39.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/flag.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      303 2018-06-08 00:11:39.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/rallypoint.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      316 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/redantenna.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     4128 2018-07-13 07:41:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/greensub.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1124 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/barrell.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2557 2013-09-17 07:00:02.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/copter.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2001 2018-09-30 22:36:33.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/migbird.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5413 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/loading.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      563 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/greenrover.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1058 2018-09-30 22:36:33.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/cloud.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      431 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/greensinglecopter.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      432 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/bluesinglecopter.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1869 2013-02-21 06:14:28.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/iconWarning32.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      880 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/ramp.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      430 2018-06-08 00:11:39.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/bluecopter.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      616 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/hoop.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      429 2018-06-08 00:11:39.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/greencopter.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2963 2018-07-13 07:41:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/bluesub.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1339 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/home.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2329 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/greenplane.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      614 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/redrover.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      471 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/greenheli.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     6903 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/unavailable.jpg
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      453 2018-06-08 00:11:39.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/redcopter.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3207 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/redplane.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2346 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/orangeplane.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      312 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/blueantenna.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3641 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/camera-small-red.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1522 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/redheli.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      479 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/redsinglecopter.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      383 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/redboat.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      395 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/blueboat.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      612 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/bluerover.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2386 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/blueplane.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3903 2018-07-13 07:41:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/redsub.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      314 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/greenantenna.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1871 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/blueheli.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2260 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/purpleplane.png
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    23042 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/mp_tile.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    27776 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/mp_slipmap_ui.py
--rwxrwxr-x   0 tridge    (1000) tridge    (1000)     7427 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/GAreader.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    17373 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/srtm.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     4873 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_devop.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3560 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_tuneopt.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     6748 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cameraview.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     6012 2018-09-30 22:36:33.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_arm.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     7703 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_calibration.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    24836 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_console.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/
--rw-r--r--   0 tridge    (1000) tridge    (1000)     1353 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/__init__.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_app/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      457 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_app/bluemarble.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     9218 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_app/index.html
--rw-rw-r--   0 tridge    (1000) tridge    (1000)   108839 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_app/modestmaps.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      880 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_app/drone-md.png
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2339 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_app/bing.js
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      603 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_app/drone-sm.png
--rw-r--r--   0 tridge    (1000) tridge    (1000)     1971 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_server.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/
--rw-r--r--   0 tridge    (1000) tridge    (1000)     5079 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/__init__.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     4938 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/controls.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3380 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/findjoy.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      890 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/xbox-360.yml
--rw-r--r--   0 tridge    (1000) tridge    (1000)     1588 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/Logitech_WingMan_3D.yml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      852 2017-09-20 02:44:05.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/great-planes.yml
--rw-r--r--   0 tridge    (1000) tridge    (1000)      396 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/taranis.yml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1555 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/logitech-dual-action.yml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      490 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/cypress-spektrum.yml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      866 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/carolbox-usb.yml
--rw-r--r--   0 tridge    (1000) tridge    (1000)     1215 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/logicool-f310.yml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      827 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/saili-simulator.yml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      574 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/sony-playstation.yml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1711 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/xboxdrv-mode2.yml
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     8607 2018-09-07 09:01:39.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_gimbal.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)       17 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/__init__.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     1297 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/textconsole.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     5107 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/wxconsole_ui.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)      171 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/wx_processguard.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      940 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/dumpstacks.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/optparse_gui/
--rw-r--r--   0 tridge    (1000) tridge    (1000)    12088 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/optparse_gui/__init__.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    14175 2018-10-17 07:13:35.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/optparse_gui/saved.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     4900 2014-05-09 05:09:49.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/optparse_gui/demo2.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1881 2013-12-19 04:53:14.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/optparse_gui/demo1.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     1608 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/wxhorizon.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    21938 2018-09-07 09:01:39.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/opengl.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     6166 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/live_graph_ui.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     2953 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/wxgrapheditor.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    12917 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/mp_menu.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    21770 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/grapher.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      343 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/graphdefinition.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     2929 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/graph_ui.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     7711 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/wxsettings_ui.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      404 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/wxconsole_util.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)       45 2018-10-15 04:40:55.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/testproc.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     7522 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/rline.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    13224 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/mp_checklist.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     6259 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/mp_module.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    17583 2018-10-17 07:11:31.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/mp_tabbedimage.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     1276 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/mp_widgets.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     6084 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/mp_settings.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/MacOS/
--rw-r--r--   0 tridge    (1000) tridge    (1000)       62 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/MacOS/__init__.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    72673 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/MacOS/backend_wx.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     5884 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/MacOS/backend_wxagg.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    17832 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/MacOS/wxversion.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    18965 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/MacOS/backend_agg.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     3598 2018-09-30 22:36:33.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/mp_substitute.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1688 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/wxhorizon_util.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    11795 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/wavefront.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     4318 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/win_layout.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     2165 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/multiproc.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    10123 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/geodesic_grid.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     3609 2019-04-08 08:01:12.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/wxconsole.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)     3201 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/live_graph.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     3976 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/mav_fft.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/ANUGA/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     9935 2018-05-22 23:55:27.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/ANUGA/lat_long_UTM_conversion.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)        0 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/ANUGA/__init__.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     6427 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/ANUGA/redfearn.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    16586 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/ANUGA/geo_reference.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      206 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/wx_util.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     2595 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/wxsettings.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    32242 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/wxhorizon_ui.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    20348 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/mp_image.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)      635 2014-05-17 03:18:14.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/mav_param.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    12111 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/mp_util.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)      235 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/lib/wx_loader.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     4556 2018-09-30 22:36:33.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_speech.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)     2362 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_messagerate.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     4240 2016-08-22 23:01:20.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_rc.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    13413 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misc.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    17132 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_genobstacles.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2705 2018-05-31 03:57:37.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_follow.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     5594 2017-05-08 04:49:31.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_terrain.py
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misseditor/
--rw-r--r--   0 tridge    (1000) tridge    (1000)     1038 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misseditor/__init__.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2907 2018-10-13 01:17:37.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misseditor/button_renderer.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2253 2018-10-13 01:17:37.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misseditor/me_defines.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1750 2018-10-13 01:17:37.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misseditor/me_event.py
--rwxr-xr-x   0 tridge    (1000) tridge    (1000)    33161 2019-06-11 02:09:53.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misseditor/missionEditorFrame.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    13792 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misseditor/mission_editor.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    30091 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_link.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    15977 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_kmlread.py
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     2237 2017-05-10 10:36:13.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_txload.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    13352 2018-12-21 10:26:06.000000 MAVProxy-1.8.8/MAVProxy/modules/mavproxy_asterix.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)    49155 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/MAVProxy/mavproxy.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)       38 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/setup.cfg
--rw-r--r--   0 tridge    (1000) tridge    (1000)     1381 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/PKG-INFO
--rw-r--r--   0 tridge    (1000) tridge    (1000)     4070 2019-06-11 02:14:52.000000 MAVProxy-1.8.8/setup.py
--rw-r--r--   0 tridge    (1000) tridge    (1000)      640 2019-06-10 20:41:38.000000 MAVProxy-1.8.8/README.md
-drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy.egg-info/
--rw-rw-r--   0 tridge    (1000) tridge    (1000)       47 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy.egg-info/requires.txt
--rw-rw-r--   0 tridge    (1000) tridge    (1000)        1 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy.egg-info/dependency_links.txt
--rw-rw-r--   0 tridge    (1000) tridge    (1000)        9 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy.egg-info/top_level.txt
--rw-rw-r--   0 tridge    (1000) tridge    (1000)     1381 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy.egg-info/PKG-INFO
--rw-rw-r--   0 tridge    (1000) tridge    (1000)    72837 2019-06-11 02:15:52.000000 MAVProxy-1.8.8/MAVProxy.egg-info/SOURCES.txt
--rw-rw-r--   0 tridge    (1000) tridge    (1000)        1 2013-11-19 04:00:46.000000 MAVProxy-1.8.8/MAVProxy.egg-info/zip-safe
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)       48 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/__init__.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/tools/
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/tools/graphs/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    14414 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/tools/graphs/mavgraphs.xml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    12457 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/tools/graphs/ekf3Graphs.xml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    12793 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/tools/graphs/ekfGraphs.xml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    13109 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/tools/graphs/mavgraphs2.xml
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    23547 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/tools/MAVExplorer.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    21034 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/tools/mavflightview.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     8632 2018-06-08 00:11:39.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_log.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)       16 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/__init__.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     2826 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_DGPS.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4800 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_horizon.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5670 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_HIL.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3935 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_nsh.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3768 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_relay.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     4375 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_help.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4229 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_output.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5823 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_battery.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     4650 2019-07-18 01:22:16.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_checklist.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3456 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_auxopt.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3940 2018-06-20 08:21:08.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_system_time.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5429 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_GPSInput.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4391 2018-09-30 22:36:33.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_sensors.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5821 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_followtest.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    19230 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    31204 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/sc_SonyQX1.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     7912 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/sc_main.py
+-rwxrwxr-x   0 tridge    (1000) tridge    (1000)     4930 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/sc_ExifWriter.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     6701 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/sc_video.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5119 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/sc_config.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3303 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/sc_webcam.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2252 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/ssdp.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5954 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_gasheli.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3750 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_rcsetup.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3070 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_ppp.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1690 2018-09-07 09:01:39.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_message.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     9183 2018-10-15 07:15:05.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/__init__.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)        0 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      275 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/mavcesium_default.ini
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/templates/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1476 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/templates/settings_menu.html
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4873 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/templates/index.html
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1428 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/templates/settings_general.html
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      104 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/templates/settings_model.html
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1497 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/templates/context_menu.html
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2322 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/config.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      886 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/lighterShared.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/BaseLayerPicker/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      620 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/BaseLayerPicker/lighter.css
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2001 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/BaseLayerPicker/BaseLayerPicker.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Timeline/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      336 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Timeline/lighter.css
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1354 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Timeline/Timeline.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/InfoBox/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3045 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/InfoBox/InfoBoxDescription.css
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1579 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/InfoBox/InfoBox.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Animation/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1701 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Animation/lighter.css
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2355 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Animation/Animation.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Geocoder/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      397 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Geocoder/lighter.css
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1537 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Geocoder/Geocoder.css
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5099 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/lighter.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/FullscreenButton/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      102 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/FullscreenButton/FullscreenButton.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/SelectionIndicator/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      338 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/SelectionIndicator/SelectionIndicator.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Cesium3DTilesInspector/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2574 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Cesium3DTilesInspector/Cesium3DTilesInspector.css
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1546 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/shared.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/ProjectionPicker/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1046 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/ProjectionPicker/ProjectionPicker.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Viewer/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1367 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Viewer/Viewer.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/NavigationHelpButton/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      890 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/NavigationHelpButton/lighter.css
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1722 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/NavigationHelpButton/NavigationHelpButton.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/PerformanceWatchdog/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      256 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/PerformanceWatchdog/PerformanceWatchdog.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/SceneModePicker/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1582 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/SceneModePicker/SceneModePicker.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TerrainProviders/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     6173 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TerrainProviders/Ellipsoid.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4482 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TerrainProviders/STK.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      781 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TimelineIcons.png
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11575 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/esriWorldImagery.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     7491 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/naturalEarthII.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     7270 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapboxStreets.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     9943 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/bingAerial.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2663 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/openStreetMap.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4119 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/stamenToner.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11555 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/esriNationalGeographic.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     8076 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/bingRoads.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     8300 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapboxTerrain.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    10374 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/bingAerialLabels.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     8501 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/esriWorldStreetMap.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11342 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapQuestOpenStreetMap.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     9242 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapboxSatellite.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5836 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/blackMarble.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    10806 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/stamenWatercolor.png
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5555 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchZoom.svg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5706 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/Mouse.svg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5654 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/MouseMiddle.svg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5647 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/MouseRight.svg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5701 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchRotate.svg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     6416 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchDrag.svg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5656 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/MouseLeft.svg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5996 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchTilt.svg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3565 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/Touch.svg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      723 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/info-loading.gif
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumWidget/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      269 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumWidget/lighter.css
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1006 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumWidget/CesiumWidget.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/VRButton/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)       94 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/VRButton/VRButton.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumInspector/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1970 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumInspector/CesiumInspector.css
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    22424 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/widgets.css
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)  2786998 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Cesium.js
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    18309 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/cesiumWorkerBootstrapper.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   124421 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolylineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    95272 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createSphereGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   193321 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/transcodeCRNToDXT.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   100382 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipseOutlineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   203242 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCorridorGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   111067 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createFrustumGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   163149 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createRectangleGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   184068 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createVerticesFromGoogleEarthEnterpriseBuffer.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   219814 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolygonGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   113295 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createFrustumOutlineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    94573 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCylinderGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   139600 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   185374 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/upsampleQuantizedTerrainMesh.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   182327 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createVerticesFromHeightmap.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   139351 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/combineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    89849 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createSphereOutlineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    32071 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/decodeGoogleEarthEnterprisePacket.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    91793 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCylinderOutlineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   190159 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolylineVolumeOutlineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   194480 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCorridorOutlineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    87453 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createBoxOutlineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1048 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/transferTypedArrayTest.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   121961 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createSimplePolylineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    92852 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createBoxGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   181378 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createVerticesFromQuantizedTerrainMesh.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   187463 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createWallGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   205356 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCircleGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    94321 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipsoidGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    88928 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipsoidOutlineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   203374 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipseGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   184551 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createWallOutlineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   107464 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createRectangleOutlineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   211473 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolygonOutlineGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   220382 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolylineVolumeGeometry.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   101776 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCircleOutlineGeometry.js
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/ThirdParty/
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/ThirdParty/Workers/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    19929 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/ThirdParty/Workers/deflate.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    24593 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/ThirdParty/Workers/inflate.js
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    67428 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_0.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    65311 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_18.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    66408 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_3.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    65711 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_15.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    64664 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_12.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    65547 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_14.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    65594 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_6.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    65312 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_26.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    67315 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_1.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    65854 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_13.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    64955 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_25.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    65903 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_4.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    64979 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_22.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    65331 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_20.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    64845 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_21.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    65012 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_11.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    65986 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_10.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    27598 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_27.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    65539 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_19.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    66086 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_23.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    66859 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_9.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    65624 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_17.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    66932 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_8.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    64896 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_24.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    67101 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_7.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    66031 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_16.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    67804 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_2.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    65381 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_5.json
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   528939 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/approximateTerrainHeights.json
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/0/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    12067 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/0/0.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/1/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    14055 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/1/0.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    12957 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/1.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     9032 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/0.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11859 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/3.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11362 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/2.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    10234 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/1.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     9531 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/0.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    10754 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/3.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11678 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/2.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    12265 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/1.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     8474 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/0.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11888 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/3.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    16477 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/2.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     9307 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/1.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     8157 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/0.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    10341 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/3.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     7891 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/2.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    12456 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/1.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    10657 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/0.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    14940 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/3.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    12262 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/2.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    10274 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/1.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     7540 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/0.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11877 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/3.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    16112 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/2.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     6850 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/1.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     7852 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/0.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    15862 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/3.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11581 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/2.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11564 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/1.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     6636 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/0.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    12756 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/3.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    16411 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/2.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      794 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/tilemapresource.xml
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/3/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    13262 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/3/1.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    10532 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/3/0.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/0/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11399 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/0/1.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     7278 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/0/0.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/2/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    15312 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/2/1.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     9643 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/2/0.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/1/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    13142 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/1/1.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    10652 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/1/0.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2411 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/water.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2703 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/star.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2407 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/laundry.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2714 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bakery.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1765 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/building.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2595 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/america-football.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1425 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/grocery.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2979 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/london-underground.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2228 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/fire-station.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1312 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/roadblock.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1188 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/airfield.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1293 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/alcohol-shop.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      788 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/city.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2411 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/campsite.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2249 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-metro.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3610 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cesium.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2816 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-light.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2681 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/zoo.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2502 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/college.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2284 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/park2.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      936 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bank.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1999 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/golf.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1533 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/emergency-telephone.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1907 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/minefield.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      582 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/square.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2194 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/police.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2420 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/soccer.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3146 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/dog-park.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1838 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/baseball.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1606 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/gift.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2106 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/swimming.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2879 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/ferry.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2048 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/harbor.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1371 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/music.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3159 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/art-gallery.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1092 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/industrial.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1702 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/telephone.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1554 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/airport.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1996 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-underground.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3989 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bicycle.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2145 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/village.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1518 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cafe.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3301 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/hairdresser.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1318 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/basketball.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      650 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/square-stroked.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2384 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/religious-jewish.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2499 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/restaurant.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3345 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/skiing.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1908 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/warehouse.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1474 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/mobilephone.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1376 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/monument.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1498 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/car.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2073 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2057 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/garden.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1658 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/tennis.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2005 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/town-hall.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1378 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/logging.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3357 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/oil-well.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1403 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/beer.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2942 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/scooter.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1772 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/polling-place.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      909 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/hospital.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2137 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/triangle.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1307 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/entrance.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1273 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/post.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3838 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/school.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1435 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bar.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1355 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/library.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3460 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/star-stroked.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2258 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/pharmacy.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2059 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/heliport.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2448 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/marker.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2429 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/danger.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1603 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/chemist.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1917 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/waste-basket.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1745 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/heart.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1677 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cricket.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      967 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cemetery.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1976 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/camera.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      998 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bus.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2578 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/museum.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2037 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/clothing-store.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1111 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/place-of-worship.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2151 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/wetland.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1002 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/commercial.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1563 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/parking-garage.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2019 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/fast-food.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1125 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/town.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2917 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/toilets.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2126 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/circle-stroked.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1680 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/embassy.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2270 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/slaughterhouse.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1459 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/circle.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3233 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/theatre.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1888 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cross.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2071 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-above.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1686 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/farm.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1602 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/ice-cream.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1129 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/suitcase.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      948 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/religious-christian.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3414 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/marker-stroked.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1703 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/dam.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3856 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/playground.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3925 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/religious-muslim.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3288 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/pitch.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1773 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/land-use.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2837 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/triangle-stroked.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1250 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/parking.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1371 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/prison.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1944 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/lighthouse.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2059 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/park.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1362 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/lodging.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1544 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/shop.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1741 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/fuel.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1492 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cinema.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1653 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rocket.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3437 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/disability.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   294196 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/waterNormals.jpg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   168640 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_pz.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   138551 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_px.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   134462 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_mx.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   168829 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_py.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   183677 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_mz.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   167849 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_my.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    34121 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/waterNormalsSmall.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    18196 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/moonSmall.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      348 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/pin.svg
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      722 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/favicon-32x32.png
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1905 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/cesium.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/third_party/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      237 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/third_party/tether.min.css
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    31018 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/third_party/font-awesome.min.css
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   150952 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/third_party/bootstrap.min.css
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    19176 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/blu-blank.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    18905 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/ylw-blank.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    18816 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/R.png
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2341 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/websocket.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    25412 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/hud.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      274 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/util.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2305 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/cesium_setup.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2457 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/wp.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3598 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/context_menu.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1049 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/settings.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    34111 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/core.js
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    24632 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/tether.min.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    46654 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/bootstrap.min.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    86659 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/jquery-3.2.1.min.js
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    77160 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.woff2
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   165742 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   165548 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   444379 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   134808 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/FontAwesome.otf
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    98024 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.woff
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/pointers/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1176 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/pointers/move.png
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/models/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   346955 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/models/rat.gltf
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    10339 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/models/rat.glb
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)       12 2016-07-28 07:03:42.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/api_keys.txt~
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     8176 2018-10-15 07:15:05.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/cesium_web_server.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     8176 2017-11-12 22:28:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/cesium_web_server.py~
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3755 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_signing.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3033 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_serial.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     3181 2019-07-18 01:22:19.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_example.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    34951 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_wp.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1295 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_msg.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    12715 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_rally.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2280 2014-05-17 03:17:49.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_GPS.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     5230 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_heliplane.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     4721 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_graph.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     5314 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_restserver.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1119 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_timesync.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     8232 2018-09-07 09:01:39.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_tracker.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    18022 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_param.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2964 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_gopro.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     6732 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    31024 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/magical_ui.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3043 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/glrenderer.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     8116 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/wxvehicle.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/data/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      683 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/data/quadcopter.mtl
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     9420 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/data/arrow.obj
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   456031 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/data/quadcopter.obj
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      422 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/data/arrow.mtl
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     8622 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/wxgeodesicgrid.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1389 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_test.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    15488 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cmdlong.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2060 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_antenna.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2951 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mode.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      926 2018-09-30 22:36:33.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_layout.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    14039 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_dataflash_logger.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    12594 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_firmware.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    10619 2019-07-18 01:22:16.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_adsb.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    12739 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fence.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    37537 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/__init__.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     9339 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/mp_slipmap.py
+-rwxrwxr-x   0 tridge    (1000) tridge    (1000)     3983 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/mp_elevation.py
+-rwxrwxr-x   0 tridge    (1000) tridge    (1000)     1479 2016-04-27 06:39:39.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/elev_check.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    22787 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/mp_slipmap_util.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1658 2018-09-30 22:36:33.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/hawk.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      287 2018-06-08 00:11:39.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/flag.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      303 2018-06-08 00:11:39.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/rallypoint.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      316 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/redantenna.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4128 2018-07-13 07:41:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/greensub.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1124 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/barrell.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2557 2013-09-17 07:00:02.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/copter.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2001 2018-09-30 22:36:33.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/migbird.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5413 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/loading.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      563 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/greenrover.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1058 2018-09-30 22:36:33.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/cloud.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      431 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/greensinglecopter.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      432 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/bluesinglecopter.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1869 2013-02-21 06:14:28.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/iconWarning32.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      880 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/ramp.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      430 2018-06-08 00:11:39.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/bluecopter.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      616 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/hoop.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      429 2018-06-08 00:11:39.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/greencopter.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2963 2018-07-13 07:41:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/bluesub.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1339 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/home.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2329 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/greenplane.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      614 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/redrover.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      471 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/greenheli.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     6903 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/unavailable.jpg
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      453 2018-06-08 00:11:39.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/redcopter.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3207 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/redplane.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2346 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/orangeplane.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      312 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/blueantenna.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3641 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/camera-small-red.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1522 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/redheli.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      479 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/redsinglecopter.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      383 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/redboat.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      395 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/blueboat.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      612 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/bluerover.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2386 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/blueplane.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3903 2018-07-13 07:41:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/redsub.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      314 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/greenantenna.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1871 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/blueheli.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2260 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/purpleplane.png
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    23042 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/mp_tile.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    27809 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/mp_slipmap_ui.py
+-rwxrwxr-x   0 tridge    (1000) tridge    (1000)     7427 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/GAreader.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    17373 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/srtm.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4873 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_devop.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3560 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_tuneopt.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     6748 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cameraview.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     6012 2018-09-30 22:36:33.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_arm.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     7703 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_calibration.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    24836 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_console.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     1353 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/__init__.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_app/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      457 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_app/bluemarble.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     9218 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_app/index.html
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   108839 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_app/modestmaps.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      880 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_app/drone-md.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2339 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_app/bing.js
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      603 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_app/drone-sm.png
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     1971 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_server.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     5079 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4938 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/controls.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3380 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/findjoy.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      890 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/xbox-360.yml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     1588 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/Logitech_WingMan_3D.yml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      852 2017-09-20 02:44:05.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/great-planes.yml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      396 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/taranis.yml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1555 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/logitech-dual-action.yml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      490 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/cypress-spektrum.yml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      866 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/carolbox-usb.yml
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     1215 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/logicool-f310.yml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      827 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/saili-simulator.yml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      574 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/sony-playstation.yml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1711 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/xboxdrv-mode2.yml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     8607 2018-09-07 09:01:39.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_gimbal.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)       17 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/__init__.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     1297 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/textconsole.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     5107 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/wxconsole_ui.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      171 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/wx_processguard.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      940 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/dumpstacks.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/optparse_gui/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    12088 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/optparse_gui/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    14175 2018-10-17 07:13:35.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/optparse_gui/saved.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4900 2014-05-09 05:09:49.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/optparse_gui/demo2.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1881 2013-12-19 04:53:14.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/optparse_gui/demo1.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     1608 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/wxhorizon.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    21938 2018-09-07 09:01:39.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/opengl.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     6166 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/live_graph_ui.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     2953 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/wxgrapheditor.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    12981 2019-07-18 01:22:19.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/mp_menu.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    21770 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/grapher.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      343 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/graphdefinition.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     2929 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/graph_ui.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     7711 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/wxsettings_ui.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      404 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/wxconsole_util.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    14531 2019-07-17 06:57:02.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/ntrip.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)       45 2018-10-15 04:40:55.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/testproc.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     7522 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/rline.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    13224 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/mp_checklist.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     6259 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/mp_module.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    17583 2018-10-17 07:11:31.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/mp_tabbedimage.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     1276 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/mp_widgets.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     6084 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/mp_settings.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/MacOS/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)       62 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/MacOS/__init__.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    72673 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/MacOS/backend_wx.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     5884 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/MacOS/backend_wxagg.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    17846 2019-07-18 01:22:16.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/MacOS/wxversion.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    18965 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/MacOS/backend_agg.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3598 2018-09-30 22:36:33.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/mp_substitute.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1688 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/wxhorizon_util.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11795 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/wavefront.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     4318 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/win_layout.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     2165 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/multiproc.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    10123 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/geodesic_grid.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     3609 2019-04-08 08:01:12.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/wxconsole.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)     3201 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/live_graph.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     3976 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/mav_fft.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/ANUGA/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     9935 2018-05-22 23:55:27.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/ANUGA/lat_long_UTM_conversion.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)        0 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/ANUGA/__init__.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     6427 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/ANUGA/redfearn.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    16586 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/ANUGA/geo_reference.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      206 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/wx_util.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     2595 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/wxsettings.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    32242 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/wxhorizon_ui.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    20348 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/mp_image.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      635 2014-05-17 03:18:14.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/mav_param.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    12111 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/mp_util.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      235 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/lib/wx_loader.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4556 2018-09-30 22:36:33.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_speech.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     2362 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_messagerate.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4240 2016-08-22 23:01:20.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_rc.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    14965 2019-07-18 01:22:19.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misc.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    17132 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_genobstacles.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2705 2018-05-31 03:57:37.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_follow.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fieldcheck/
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    16692 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fieldcheck/__init__.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      132 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fieldcheck/springvalley-foamy-fence.txt
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      962 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fieldcheck/cmac-foamy-mission-ccw.txt
+-rw-r--r--   0 tridge    (1000) tridge    (1000)       60 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fieldcheck/springvalley-foamy-rally.txt
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      132 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fieldcheck/cmac-foamy-fence.txt
+-rw-r--r--   0 tridge    (1000) tridge    (1000)       59 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fieldcheck/cmac-foamy-rally.txt
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      962 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fieldcheck/cmac-foamy-mission-cw.txt
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      962 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fieldcheck/springvalley-foamy-mission-ccw.txt
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      962 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fieldcheck/springvalley-foamy-mission-cw.txt
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5594 2017-05-08 04:49:31.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_terrain.py
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misseditor/
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     1038 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misseditor/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2907 2018-10-13 01:17:37.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misseditor/button_renderer.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2253 2018-10-13 01:17:37.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misseditor/me_defines.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1750 2018-10-13 01:17:37.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misseditor/me_event.py
+-rwxr-xr-x   0 tridge    (1000) tridge    (1000)    33161 2019-07-03 10:35:54.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misseditor/missionEditorFrame.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    13792 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misseditor/mission_editor.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    30091 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_link.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    15977 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_kmlread.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2237 2017-05-10 10:36:13.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_txload.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    13352 2018-12-21 10:26:06.000000 MAVProxy-1.8.9/MAVProxy/modules/mavproxy_asterix.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)    49437 2019-07-18 01:22:19.000000 MAVProxy-1.8.9/MAVProxy/mavproxy.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)       38 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/setup.cfg
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     1381 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/PKG-INFO
+-rw-r--r--   0 tridge    (1000) tridge    (1000)     4070 2019-07-29 06:27:23.000000 MAVProxy-1.8.9/setup.py
+-rw-r--r--   0 tridge    (1000) tridge    (1000)      640 2019-06-10 20:41:38.000000 MAVProxy-1.8.9/README.md
+drwxr-xr-x   0 tridge    (1000) tridge    (1000)        0 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy.egg-info/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)       47 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy.egg-info/requires.txt
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)        1 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy.egg-info/dependency_links.txt
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)        9 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy.egg-info/top_level.txt
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1381 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy.egg-info/PKG-INFO
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    73142 2019-07-29 06:27:52.000000 MAVProxy-1.8.9/MAVProxy.egg-info/SOURCES.txt
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)        1 2013-11-19 04:00:46.000000 MAVProxy-1.8.9/MAVProxy.egg-info/zip-safe
```

### Comparing `MAVProxy-1.8.8/MAVProxy/tools/graphs/mavgraphs.xml` & `MAVProxy-1.8.9/MAVProxy/tools/graphs/mavgraphs.xml`

 * *Files 4% similar despite different names*

#### Comparing `MAVProxy-1.8.8/MAVProxy/tools/graphs/mavgraphs.xml` & `MAVProxy-1.8.9/MAVProxy/tools/graphs/mavgraphs.xml`

```diff
@@ -178,22 +178,25 @@
 For a well tuned aircraft PIDR.Des should match the smoothed IMU.GyrX value. 
 If PIDR.I has a constant positive value then it means the aircraft is trimmed to roll to the left side, and the integrator is learning the aileron offset needed to keep the aircraft level. If PIDR.I has a constant negative value then the aircraft is trimmed a bit to the right.</description>
     <expression>PIDR.Des PIDR.P PIDR.I PIDR.D lowpass(degrees(IMU.GyrX),&quot;gx&quot;,0.9)</expression>
   </graph>
   <graph name="Sensors/Compass/Compare Predicted">
     <description/>
     <expression>MAG.MagX expected_mag(GPS,ATT).x MAG.MagY expected_mag(GPS,ATT).y MAG.MagZ expected_mag(GPS,ATT).z</expression>
+    <expression>RAW_IMU.xmag expected_mag(GPS_RAW_INT,ATTITUDE).x RAW_IMU.ymag expected_mag(GPS_RAW_INT,ATTITUDE).y RAW_IMU.zmag expected_mag(GPS_RAW_INT,ATTITUDE).z</expression>
   </graph>
   <graph name="Sensors/Compass/Compare Predicted2">
     <description/>
     <expression>MAG2.MagX expected_mag(GPS,ATT).x MAG2.MagY expected_mag(GPS,ATT).y MAG2.MagZ expected_mag(GPS,ATT).z</expression>
+    <expression>SCALED_IMU2.xmag expected_mag(GPS_RAW_INT,ATTITUDE).x SCALED_IMU2.ymag expected_mag(GPS_RAW_INT,ATTITUDE).y SCALED_IMU2.zmag expected_mag(GPS_RAW_INT,ATTITUDE).z</expression>
   </graph>
   <graph name="Sensors/Compass/Compare Predicted3">
     <description/>
     <expression>MAG3.MagX expected_mag(GPS,ATT).x MAG3.MagY expected_mag(GPS,ATT).y MAG3.MagZ expected_mag(GPS,ATT).z</expression>
+    <expression>SCALED_IMU3.xmag expected_mag(GPS_RAW_INT,ATTITUDE).x SCALED_IMU3.ymag expected_mag(GPS_RAW_INT,ATTITUDE).y SCALED_IMU3.zmag expected_mag(GPS_RAW_INT,ATTITUDE).z</expression>
   </graph>
   <graph name="Sensors/Compass/EarthField Error EK2 Lane1">
     <description/>
     <expression>earth_field_error(GPS,NKF2).x earth_field_error(GPS,NKF2).y earth_field_error(GPS,NKF2).z</expression>
   </graph>
   <graph name="Sensors/Compass/EarthField Error EK2 Lane2">
     <description/>
@@ -211,8 +214,20 @@
     <description/>
     <expression>PIDY.P PIDY.I PIDY.D</expression>
   </graph>
   <graph name="Copter/PID/PIDA">
     <description/>
     <expression>PIDA.P PIDA.I PIDA.D</expression>
   </graph>
+  <graph name="SITL/SIM RollRate vs GyrX">
+    <description/>
+    <expression>IMU.GyrX sim_body_rates(SIM).x</expression>
+  </graph>
+  <graph name="SITL/SIM PitchRate vs GyrY">
+    <description/>
+    <expression>IMU.GyrY sim_body_rates(SIM).y</expression>
+  </graph>
+  <graph name="SITL/SIM YawRate vs GyrZ">
+    <description/>
+    <expression>IMU.GyrZ sim_body_rates(SIM).z</expression>
+  </graph>
 </graphs>
```

### Comparing `MAVProxy-1.8.8/MAVProxy/tools/graphs/ekf3Graphs.xml` & `MAVProxy-1.8.9/MAVProxy/tools/graphs/ekf3Graphs.xml`

 * *Files 0% similar despite different names*

#### Comparing `MAVProxy-1.8.8/MAVProxy/tools/graphs/ekf3Graphs.xml` & `MAVProxy-1.8.9/MAVProxy/tools/graphs/ekf3Graphs.xml`

```diff
@@ -188,15 +188,15 @@
     <description>Wind Velocity NE</description>
     <expression>XKF2.VWN XKF2.VWE XKF7.VWN XKF7.VWE</expression>
     <expression>EKF3.VWN EKF3.VWE XKF2.VWN XKF2.VWE</expression>
     <expression>EKF3.VWN EKF3.VWE</expression>
   </graph>
   <graph name="EKF/Wind Speed and Direction">
     <description>Wind Velocity NE</description>
-    <expression>sqrt(sqrt(XKF2.VWN**2+XKF2.VWE**2) wrap_360(degrees(atan2(-XKF2.VWE,-XKF2.VWN))):2 sqrt(XKF7.VWN**2+XKF7.VWE**2) wrap_360(degrees(atan2(-XKF7.VWE,-XKF7.VWN))):2</expression>
+    <expression>sqrt(XKF2.VWN**2+XKF2.VWE**2) wrap_360(degrees(atan2(-XKF2.VWE,-XKF2.VWN))):2 sqrt(XKF7.VWN**2+XKF7.VWE**2) wrap_360(degrees(atan2(-XKF7.VWE,-XKF7.VWN))):2</expression>
     <expression>sqrt(EKF3.VWN**2+EKF3.VWE**2) wrap_360(degrees(atan2(-EKF3.VWE,-EKF3.VWN))):2 sqrt(XKF2.VWN**2+XKF2.VWE**2) wrap_360(degrees(atan2(-XKF2.VWE,-XKF2.VWN))):2</expression>
     <expression>sqrt(EKF3.VWN**2+EKF3.VWE**2) wrap_360(degrees(atan2(-EKF3.VWE,-EKF3.VWN))):2</expression>
   </graph>
   <graph name="EKF/Accel Bias">
     <description>Accel Bias</description>
     <expression>XKF2.AZbias XKF7.AZbias</expression>
     <expression>EKF3.AZ1bias EKF3.AZ2bias EKF3.Ratio:2 XKF2.AZbias</expression>
```

### Comparing `MAVProxy-1.8.8/MAVProxy/tools/graphs/ekfGraphs.xml` & `MAVProxy-1.8.9/MAVProxy/tools/graphs/ekfGraphs.xml`

 * *Files 0% similar despite different names*

#### Comparing `MAVProxy-1.8.8/MAVProxy/tools/graphs/ekfGraphs.xml` & `MAVProxy-1.8.9/MAVProxy/tools/graphs/ekfGraphs.xml`

```diff
@@ -188,15 +188,15 @@
     <description>Wind Velocity NE</description>
     <expression>NKF2.VWN NKF2.VWE NKF7.VWN NKF7.VWE</expression>
     <expression>EKF2.VWN EKF2.VWE NKF2.VWN NKF2.VWE</expression>
     <expression>EKF2.VWN EKF2.VWE</expression>
   </graph>
   <graph name="EKF/Wind Speed and Direction">
     <description>Wind Velocity NE</description>
-    <expression>sqrt(sqrt(NKF2.VWN**2+NKF2.VWE**2) wrap_360(degrees(atan2(-NKF2.VWE,-NKF2.VWN))):2 sqrt(NKF7.VWN**2+NKF7.VWE**2) wrap_360(degrees(atan2(-NKF7.VWE,-NKF7.VWN))):2</expression>
+    <expression>sqrt(NKF2.VWN**2+NKF2.VWE**2) wrap_360(degrees(atan2(-NKF2.VWE,-NKF2.VWN))):2 sqrt(NKF7.VWN**2+NKF7.VWE**2) wrap_360(degrees(atan2(-NKF7.VWE,-NKF7.VWN))):2</expression>
     <expression>sqrt(EKF2.VWN**2+EKF2.VWE**2) wrap_360(degrees(atan2(-EKF2.VWE,-EKF2.VWN))):2 sqrt(NKF2.VWN**2+NKF2.VWE**2) wrap_360(degrees(atan2(-NKF2.VWE,-NKF2.VWN))):2</expression>
     <expression>sqrt(EKF2.VWN**2+EKF2.VWE**2) wrap_360(degrees(atan2(-EKF2.VWE,-EKF2.VWN))):2</expression>
   </graph>
   <graph name="EKF/Accel Bias">
     <description>Accel Bias</description>
     <expression>NKF2.AZbias NKF7.AZbias</expression>
     <expression>EKF2.AZ1bias EKF2.AZ2bias EKF2.Ratio:2 NKF2.AZbias</expression>
```

### Comparing `MAVProxy-1.8.8/MAVProxy/tools/graphs/mavgraphs2.xml` & `MAVProxy-1.8.9/MAVProxy/tools/graphs/mavgraphs2.xml`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/tools/MAVExplorer.py` & `MAVProxy-1.8.9/MAVProxy/tools/MAVExplorer.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/tools/mavflightview.py` & `MAVProxy-1.8.9/MAVProxy/tools/mavflightview.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,14 +359,16 @@
                 (lat, lng) = (m.Alat*1.0e-7, m.Alng*1.0e-7)
             elif type in ['AHR2', 'POS', 'CHEK']:
                 (lat, lng) = (m.Lat, m.Lng)
             elif type == 'AHRS2':
                 (lat, lng) = (m.lat*1.0e-7, m.lng*1.0e-7)
             elif type == 'ORGN':
                 (lat, lng) = (m.Lat, m.Lng)
+            elif type == 'SIM':
+                (lat, lng) = (m.Lat, m.Lng)
             else:
                 lat = m.lat * 1.0e-7
                 lng = m.lon * 1.0e-7
 
             # automatically add new types to instances
             if type not in instances:
                 instances[type] = len(instances)
```

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_log.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_log.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_DGPS.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_DGPS.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_horizon.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_horizon.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_HIL.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_HIL.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_nsh.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_nsh.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_relay.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_relay.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_help.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_help.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_output.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_output.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_battery.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_battery.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_checklist.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_checklist.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,34 +70,34 @@
         '''beforeEngineList - Waypoints Loaded'''
         if type == 'HEARTBEAT':
             if self.module('wp').wploader.count() == 0:
                 self.checklist.set_check("Waypoints Loaded", 0)
             else:
                 self.checklist.set_check("Waypoints Loaded", 1)
 
-		'''beforeTakeoffList - Compass active'''
+        '''beforeTakeoffList - Compass active'''
         if type == 'GPS_RAW':
             if math.fabs(msg.hdg - master.field('VFR_HUD', 'heading', '-')) < 10 or math.fabs(msg.hdg - master.field('VFR_HUD', 'heading', '-')) > 355:
                 self.checklist.set_check("Compass active", 1)
             else:
                 self.checklist.set_check("Compass active", 0)
 
-		'''beforeCruiseList - Airspeed > 10 m/s , Altitude > 30 m'''
+        '''beforeCruiseList - Airspeed > 10 m/s , Altitude > 30 m'''
         if type == 'VFR_HUD':
             rel_alt = master.field('GLOBAL_POSITION_INT', 'relative_alt', 0) * 1.0e-3
             if rel_alt > 30:
                 self.checklist.set_check("Altitude > 30 m", 1)
             else:
                 self.checklist.set_check("Altitude > 30 m", 0)
             if msg.airspeed > 10 or msg.groundspeed > 10:
                 self.checklist.set_check("Airspeed > 10 m/s", 1)
             else:
                 self.checklist.set_check("Airspeed > 10 m/s", 0)
 
-		'''beforeEngineList - IMU'''
+        '''beforeEngineList - IMU'''
         if type in ['SYS_STATUS']:
             sensors = { 'AS'  : mavutil.mavlink.MAV_SYS_STATUS_SENSOR_DIFFERENTIAL_PRESSURE,
                         'MAG' : mavutil.mavlink.MAV_SYS_STATUS_SENSOR_3D_MAG,
                         'INS' : mavutil.mavlink.MAV_SYS_STATUS_SENSOR_3D_ACCEL | mavutil.mavlink.MAV_SYS_STATUS_SENSOR_3D_GYRO,
                         'AHRS' : mavutil.mavlink.MAV_SYS_STATUS_AHRS}
             bits = sensors['INS']
             present = ((msg.onboard_control_sensors_enabled & bits) == bits)
```

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_auxopt.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_auxopt.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_system_time.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_system_time.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cmac_check/__init__.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fieldcheck/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,181 +3,120 @@
 CMAC mission control
 Peter Barker
 
 based on
 
 CUAV mission control
 Andrew Tridgell
+
+TODO:
+ - ensure parameters are correct
+ - add check that battery is within tolerances (chemistry issues...)
+ - autodetect numcells being incorrect
 '''
 
 import math
 import os
 import time
 
 from MAVProxy.modules.lib import mp_module
+from MAVProxy.modules.lib.mp_settings import MPSettings
+from MAVProxy.modules.lib.mp_settings import MPSetting
+
 from pymavlink import mavutil
 from MAVProxy.modules.lib import mp_util
 
 import pkg_resources
 
-CMAC_LOCATION = mavutil.location(-35.363261, 149.165230, 584, 353)
-
 if mp_util.has_wxpython:
     from MAVProxy.modules.lib.mp_menu import MPMenuItem
     from MAVProxy.modules.lib.mp_menu import MPMenuSubMenu
 
-
-class CMACModule(mp_module.MPModule):
-    def __init__(self, mpstate):
-        super(CMACModule, self).__init__(mpstate,
-                                         "CMAC",
-                                         "CMAC Checks",
-                                         public=True)
-        self.rate_period = mavutil.periodic_event(1.0/15)
+class FieldCheck(object):
+    def __init__(self):
         self.is_armed = False
-        self.done_map_menu = False
-
-        from MAVProxy.modules.lib.mp_settings import MPSettings, MPSetting
-        self.cmac_settings = MPSettings(
-            [
-                MPSetting('fence_maxdist', float, 1000,
-                          'Max FencePoint Distance from south-CMAC'),
-                MPSetting('wp_maxdist', float, 500,
-                          'Max WayPoint Distance from south-CMAC'),
-                MPSetting('rally_maxdist', float, 200,
-                          'Max Rally Distance from south-CMAC'),
-            ])
-        self.add_completion_function('(CMACCHECKSETTING)',
-                                     self.cmac_settings.completion)
-        self.add_command('cmaccheck',
-                         self.cmd_cmaccheck,
-                         'cmac check control',
-                         ['check',
-                          'set (CMACCHECKSETTING)'])
 
         self.last_fence_fetch = 0
         self.last_mission_fetch = 0
         self.last_rally_fetch = 0
         self.done_heartbeat_check = 0
 
-        self.check()
+        # an altitude should always be within a few metres of when disarmed:
+        self.disarmed_alt = 584
+        self.rate_period = mavutil.periodic_event(1.0/15)
+
+        self.done_map_menu = False
+
+    def close_to(self, loc1):
+        ret = self.get_distance(loc1, self.location)
+        print("Distance to %s: %um" % (self.lc_name, ret))
+        return ret < 100
 
     # swiped from ArduPilot's common.py:
     def get_distance(self, loc1, loc2):
         """Get ground distance between two locations."""
         dlat = loc2.lat - loc1.lat
         try:
             dlong = loc2.lng - loc1.lng
         except AttributeError:
             dlong = loc2.lon - loc1.lon
 
         return math.sqrt((dlat*dlat) + (dlong*dlong)) * 1.113195e5
 
-    def check_map_menu(self):
-        # make the initial map menu
-        if not mp_util.has_wxpython:
-            return
-        if self.done_map_menu:
-            if not self.module('map'):
-                self.done_map_menu = False
-            return
-
-        if self.module('map'):
-            self.menu = MPMenuSubMenu('CMAC', items=[
-                MPMenuItem('Load foamy mission CW',
-                           'Load foamy mission CW',
-                           '# cmaccheck loadFoamyMissionCW'),
-                MPMenuItem('Load foamy mission CCW',
-                           'Load foamy mission CCW',
-                           '# cmaccheck loadFoamyMissionCCW'),
-                MPMenuItem('Load rally points',
-                           'Load rally points',
-                           '# cmaccheck loadRally'),
-                MPMenuItem('Load foamy fence',
-                           'Load foamy fence',
-                           '# cmaccheck loadFoamyFence'),
-            ])
-            self.module('map').add_menu(self.menu)
-            self.done_map_menu = True
+    def flightdata_filepath(self, filename):
+        if os.path.exists(filename):
+            return filename
+        return pkg_resources.resource_filename(__name__, filename)
 
     def loadRally(self):
-        filename = "cmac-foamy-rally.txt"
-        filepath = pkg_resources.resource_filename(__name__, filename)
-        if os.path.exists(filepath):
-            rallymod = self.module('rally')
-            rallymod.cmd_rally(["load", filepath])
+        filepath = self.flightdata_filepath(self.fc_settings.rally_filename)
+        rallymod = self.module('rally')
+        rallymod.cmd_rally(["load", filepath])
 
     def loadFoamyFence(self):
-        filename = "cmac-foamy-fence.txt"
-        filepath = pkg_resources.resource_filename(__name__, filename)
-        if os.path.exists(filepath):
-            fencemod = self.module('fence')
-            fencemod.cmd_fence(["load", filepath])
+        filepath = self.flightdata_filepath(self.fc_settings.fence_filename)
+        fencemod = self.module('fence')
+        fencemod.cmd_fence(["load", filepath])
 
     def loadFoamyMission(self, filename):
-        filepath = pkg_resources.resource_filename(__name__, filename)
+        filepath = self.flightdata_filepath(filename)
         wpmod = self.module('wp')
         wpmod.cmd_wp(["load", filepath])
 
     def loadFoamyMissionCW(self):
-        self.loadFoamyMission("cmac-foamy-mission-cw.txt")
+        self.loadFoamyMission(self.fc_settings.mission_filename_cw)
 
     def loadFoamyMissionCCW(self):
-        self.loadFoamyMission("cmac-foamy-mission-ccw.txt")
-
-    def cmd_cmaccheck(self, args):
-        '''handle cmaccheck commands'''
-        usage = 'Usage: cmaccheck <set>'
-        if len(args) == 0:
-            print(usage)
-            return
-        if args[0] == "set":
-            self.cmac_settings.command(args[1:])
-        elif args[0] == "loadFoamyMissionCW":
-            self.loadFoamyMissionCW()
-        elif args[0] == "loadFoamyMissionCCW":
-            self.loadFoamyMissionCCW()
-        elif args[0] == "loadFoamyFence":
-            self.loadFoamyFence()
-        elif args[0] == "loadRally":
-            self.loadRally()
-        elif args[0] == "check":
-            self.check()
-        else:
-            print(usage)
-            return
+        self.loadFoamyMission(self.fc_settings.mission_filename_ccw)
 
     def whinge(self, message):
-        self.console.writeln("CMAC: %s" % (message,))
+        self.console.writeln("FC:%s %s" % (self.lc_name, message,))
 
     def check_parameters(self):
         '''check key parameters'''
         want_values = {
             "FENCE_ACTION": 4,
             "FENCE_MAXALT": 80,
             "THR_FAILSAFE": 1,
             "FS_SHORT_ACTN": 0,
             "FS_LONG_ACTN": 1,
         }
 
+        ret = True
         for key in want_values.keys():
             want = want_values[key]
             got = self.mav_param.get(key, None)
             if got is None:
                 self.whinge("No param %s" % key)
-                return False
+                ret = False
             if got != want:
                 self.whinge('%s should be %f (not %s)' % (key, want, got))
-                return False
-
-        return True
+                ret = False
 
-    def idle_task(self):
-        '''run periodic tasks'''
-        self.check_map_menu()
+        return ret
 
     def check_fence_location(self):
         fencemod = self.module('fence')
         if fencemod is None:
             self.whinge("Fence module not loaded")
             return False
         if not fencemod.have_list:
@@ -195,16 +134,16 @@
         if count < 6:
             self.whinge("Too few fence points")
             return False
         ret = True
         for i in range(fencemod.fenceloader.count()):
             p = fencemod.fenceloader.point(i)
             loc = mavutil.location(p.lat, p.lng)
-            dist = self.get_distance(CMAC_LOCATION, loc)
-            if dist > self.cmac_settings.fence_maxdist:
+            dist = self.get_distance(self.location, loc)
+            if dist > self.fc_settings.fence_maxdist:
                 self.whinge("Fencepoint %i too far away (%fm)" % (i, dist))
                 ret = False
         return ret
 
     def check_rally(self):
         rallymod = self.module('rally')
         if rallymod is None:
@@ -222,33 +161,34 @@
             return False
 
         count = rallymod.rallyloader.rally_count()
         if count < 1:
             self.whinge("Too few rally points")
             return False
 
+        rtl_loiter_radius = self.mav_param.get("RTL_RADIUS", None)
+        if rtl_loiter_radius is None or rtl_loiter_radius == 0:
+            rtl_loiter_radius = self.mav_param.get("WP_LOITER_RAD")
+        if rtl_loiter_radius is None:
+            self.whinge("No RTL loiter radius available")
+            return False
+
         ret = True
         for i in range(count):
             r = rallymod.rallyloader.rally_point(i)
             loc = mavutil.location(r.lat/10000000.0, r.lng/10000000.0)
-            dist = self.get_distance(CMAC_LOCATION, loc)
-            if dist > self.cmac_settings.rally_maxdist:
+            dist = self.get_distance(self.location, loc)
+            if dist > self.fc_settings.rally_maxdist:
                 self.whinge("Rally Point %i too far away (%fm)" % (i, dist))
                 ret = False
 
-                # ensure we won't loiter over the runway when doing
-                # rally loitering:
-            v = self.mav_param.get("RTL_RADIUS", None)
-            if v is None or v == 0:
-                v = self.mav_param.get("WP_LOITER_RAD")
-            if v is None:
-                self.whinge("No RTL loiter radius available")
-                ret = False
-#            print("dist=%f v=%f", dist, v)
-            if dist < v+30:  # add a few metres of slop
+            # ensure we won't loiter over the runway when doing
+            # rally loitering:
+#            print("dist=%f rtl_loiter_radius=%f", dist, rtl_loiter_radius)
+            if dist < rtl_loiter_radius+30:  # add a few metres of slop
                 self.whinge("Rally Point %i too close (%fm)" % (i, dist))
                 ret = False
 
         return ret
 
     def check_fence_health(self):
         try:
@@ -274,14 +214,29 @@
         ret = True
         if not self.check_fence_health():
             ret = False
         if not self.check_fence_location():
             ret = False
         return ret
 
+    def check_altitude(self):
+        if self.is_armed:
+            return True
+        try:
+            gpi = self.master.messages['GLOBAL_POSITION_INT']
+        except Exception:
+            return False
+        max_delta = 10
+        current_alt = gpi.alt / 1000
+        if abs(current_alt - self.disarmed_alt) > max_delta:
+            self.whinge("Altitude (%f) not within %fm of %fm" %
+                        (current_alt, max_delta, self.disarmed_alt))
+            return False
+        return True
+
     def check_mission(self):
         wpmod = self.module('wp')
         if wpmod is None:
             self.whinge("No waypoint module")
             return False
         count = wpmod.wploader.count()
         if count == 0:
@@ -305,16 +260,16 @@
                 # skip home
                 continue
             w = wpmod.wploader.wp(i)
             if w.command not in [mavutil.mavlink.MAV_CMD_NAV_WAYPOINT,
                                  mavutil.mavlink.MAV_CMD_NAV_LAND]:
                 continue
             loc = mavutil.location(w.x, w.y)
-            dist = self.get_distance(CMAC_LOCATION, loc)
-            if dist > self.cmac_settings.wp_maxdist:
+            dist = self.get_distance(self.location, loc)
+            if dist > self.fc_settings.wp_maxdist:
                 self.whinge("Waypoint %i too far away (%fm)" % (i, dist))
                 ret = False
         return ret
 
     def check_status(self):
         try:
             hb = self.master.messages['HEARTBEAT']
@@ -328,15 +283,14 @@
             if mc.seq > 1:
                 self.whinge('Incorrect WP %u' % mc.seq)
                 return False
         return True
 
     def check(self):
         success = True
-        self.check_map_menu()
 
         if self.master.messages.get('HEARTBEAT') is None:
             self.whinge("Waiting for heartbeat")
             success = False
             return
         if not self.check_status():
             success = False
@@ -344,14 +298,16 @@
             success = False
         if not self.check_fence():
             success = False
         if not self.check_mission():
             success = False
         if not self.check_rally():
             success = False
+        if not self.check_altitude():
+            success = False
         if not success:
             self.whinge("CHECKS BAD")
             return
         if not self.is_armed:
             self.whinge("CHECKS GOOD")
 
     def mavlink_packet(self, m):
@@ -360,11 +316,168 @@
             if self.master.messages.get('HEARTBEAT') is not None:
                 self.check()
                 self.done_heartbeat_check = True
 
         if self.rate_period.trigger():
             self.check()
 
+    def check_map_menu(self):
+        # make the initial map menu
+        if not mp_util.has_wxpython:
+            return
+        if self.done_map_menu:
+            if not self.module('map'):
+                self.done_map_menu = False
+            return
+
+        if self.module('map'):
+            self.menu = MPMenuSubMenu('FieldCheck', items=[
+                MPMenuItem('Load foamy mission CW',
+                           'Load foamy mission CW',
+                           '# fieldcheck loadFoamyMissionCW'),
+                MPMenuItem('Load foamy mission CCW',
+                           'Load foamy mission CCW',
+                           '# fieldcheck loadFoamyMissionCCW'),
+                MPMenuItem('Load rally points',
+                           'Load rally points',
+                           '# fieldcheck loadRally'),
+                MPMenuItem('Load foamy fence',
+                           'Load foamy fence',
+                           '# fieldcheck loadFoamyFence'),
+            ])
+            self.module('map').add_menu(self.menu)
+            self.done_map_menu = True
+
+    def idle_task(self):
+        self.check_map_menu()
+
+    def FC_MPSetting(self, name, atype, default, description):
+        xname = "fc_%s_%s" % (self.lc_name, name)
+        return MPSetting(name, atype, default, description)
+
+    def select(self):
+        self.fc_settings = MPSettings(
+            [
+                self.FC_MPSetting('fence_maxdist',
+                                  float,
+                                  1000,
+                                  'Max FencePoint Distance from location'),
+                self.FC_MPSetting('wp_maxdist',
+                                  float,
+                                  500,
+                                  'Max WayPoint Distance from location'),
+                self.FC_MPSetting('rally_maxdist',
+                                  float,
+                                  200,
+                                  'Max Rally Distance from location'),
+                self.FC_MPSetting('rally_filename',
+                                  str,
+                                  "%s-foamy-rally.txt" % self.lc_name,
+                                  "%s Rally Point File" % self.lc_name),
+                self.FC_MPSetting('fence_filename',
+                                  str,
+                                  "%s-foamy-fence.txt" % self.lc_name,
+                                  "%s Fence File" % self.lc_name),
+                self.FC_MPSetting('mission_filename_cw',
+                                  str,
+                                  "%s-foamy-mission-cw.txt" % self.lc_name,
+                                  "%s Mission (CW) File" % self.lc_name),
+                self.FC_MPSetting('mission_filename_ccw',
+                                  str,
+                                  "%s-foamy-mission-ccw.txt" % self.lc_name,
+                                  "%s Mission (CCW) File" % self.lc_name),
+            ])
+        self.x.add_completion_function('(FIELDCHECKCHECKSETTING)',
+                                       self.fc_settings.completion)
+        self.x.add_command('fieldcheck',
+                           self.cmd_fieldcheck,
+                           'field check control',
+                           ['check',
+                            'set (FIELDCHECKSETTING)'])
+
+    def cmd_fieldcheck(self, args):
+        '''handle fieldcheck commands'''
+        usage = 'Usage: fieldcheck <set>'
+        if len(args) == 0:
+            print(usage)
+            return
+        if args[0] == "set":
+            self.fc_settings.command(args[1:])
+        elif args[0] == "loadFoamyMissionCW":
+            self.loadFoamyMissionCW()
+        elif args[0] == "loadFoamyMissionCCW":
+            self.loadFoamyMissionCCW()
+        elif args[0] == "loadFoamyFence":
+            self.loadFoamyFence()
+        elif args[0] == "loadRally":
+            self.loadRally()
+        elif args[0] == "check":
+            self.check()
+        else:
+            print(usage)
+            return
+
+class FieldCMAC(FieldCheck):
+    lc_name = "cmac"
+    location = mavutil.location(-35.363261, 149.165230, 584, 353)
+
+class FieldSpringValley(FieldCheck):
+    location = mavutil.location(-35.281315, 149.005329, 581, 280)
+    lc_name = "springvalley"
+
+class FieldCheckModule(mp_module.MPModule):
+    def __init__(self, mpstate):
+
+        super(FieldCheckModule, self).__init__(mpstate,
+                                               "FieldCheck",
+                                               "FieldCheck Checks",
+                                               public=True)
+
+        self.fields = [
+            FieldCMAC(),
+            FieldSpringValley(),
+        ]
+
+        self.field = None
+
+    def select_field(self, field):
+        self.field = field
+        self.field.master = self.master
+        self.field.mav_param = self.mav_param
+        self.field.console = self.console
+        self.field.module = self.module
+        self.field.x = self
+        self.field.select()
+
+    def whinge(self, message):
+        self.console.writeln("FC: %s" % (message,))
+
+    def try_select_field(self, loc):
+        for field in self.fields:
+            if field.close_to(loc):
+                self.whinge("Selecting field (%s)" % field.lc_name)
+                self.select_field(field)
+
+
+    def idle_task(self):
+        '''run periodic tasks'''
+        if self.field is not None:
+            self.field.idle_task()
+
+    def mavlink_packet(self, m):
+        '''handle an incoming mavlink packet'''
+        if self.field is None:
+            # attempt to select field automatically based on location
+            mtype = m.get_type()
+            if mtype == "GPS_RAW_INT":
+                if m.fix_type >= 3:
+                    lat = m.lat
+                    lon = m.lon
+                    here = mavutil.location(lat*1e-7, lon*1e-7, 0, 0)
+                    self.try_select_field(here)
+        if self.field is None:
+            return
+        self.field.mavlink_packet(m)
 
 def init(mpstate):
     '''initialise module'''
-    return CMACModule(mpstate)
+    return FieldCheckModule(mpstate)
```

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cmac_check/cmac-foamy-mission-ccw.txt` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fieldcheck/cmac-foamy-mission-ccw.txt`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cmac_check/cmac-foamy-mission-cw.txt` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fieldcheck/cmac-foamy-mission-cw.txt`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_GPSInput.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_GPSInput.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_sensors.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_sensors.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_followtest.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_followtest.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/__init__.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/__init__.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/sc_SonyQX1.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/sc_SonyQX1.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/sc_main.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/sc_main.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/sc_ExifWriter.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/sc_ExifWriter.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/sc_video.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/sc_video.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/sc_config.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/sc_config.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/sc_webcam.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/sc_webcam.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_smartcamera/ssdp.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_smartcamera/ssdp.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_gasheli.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_gasheli.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_rcsetup.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_rcsetup.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_ppp.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_ppp.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_message.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_message.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/__init__.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/__init__.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/templates/settings_menu.html` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/templates/settings_menu.html`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/templates/index.html` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/templates/settings_general.html` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/templates/settings_general.html`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/templates/context_menu.html` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/templates/context_menu.html`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/config.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/config.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/lighterShared.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/lighterShared.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/BaseLayerPicker/lighter.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/BaseLayerPicker/lighter.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/BaseLayerPicker/BaseLayerPicker.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/BaseLayerPicker/BaseLayerPicker.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Timeline/Timeline.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Timeline/Timeline.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/InfoBox/InfoBoxDescription.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/InfoBox/InfoBoxDescription.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/InfoBox/InfoBox.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/InfoBox/InfoBox.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Animation/lighter.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Animation/lighter.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Animation/Animation.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Animation/Animation.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Geocoder/Geocoder.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Geocoder/Geocoder.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/lighter.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/lighter.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Cesium3DTilesInspector/Cesium3DTilesInspector.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Cesium3DTilesInspector/Cesium3DTilesInspector.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/shared.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/shared.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/ProjectionPicker/ProjectionPicker.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/ProjectionPicker/ProjectionPicker.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Viewer/Viewer.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Viewer/Viewer.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/NavigationHelpButton/lighter.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/NavigationHelpButton/lighter.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/NavigationHelpButton/NavigationHelpButton.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/NavigationHelpButton/NavigationHelpButton.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/SceneModePicker/SceneModePicker.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/SceneModePicker/SceneModePicker.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TerrainProviders/Ellipsoid.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TerrainProviders/Ellipsoid.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TerrainProviders/STK.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TerrainProviders/STK.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TimelineIcons.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/TimelineIcons.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/esriWorldImagery.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/esriWorldImagery.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/naturalEarthII.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/naturalEarthII.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapboxStreets.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapboxStreets.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/bingAerial.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/bingAerial.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/openStreetMap.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/openStreetMap.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/stamenToner.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/stamenToner.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/esriNationalGeographic.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/esriNationalGeographic.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/bingRoads.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/bingRoads.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapboxTerrain.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapboxTerrain.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/bingAerialLabels.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/bingAerialLabels.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/esriWorldStreetMap.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/esriWorldStreetMap.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapQuestOpenStreetMap.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapQuestOpenStreetMap.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapboxSatellite.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/mapboxSatellite.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/blackMarble.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/blackMarble.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/stamenWatercolor.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/ImageryProviders/stamenWatercolor.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchZoom.svg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchZoom.svg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/Mouse.svg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/Mouse.svg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/MouseMiddle.svg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/MouseMiddle.svg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/MouseRight.svg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/MouseRight.svg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchRotate.svg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchRotate.svg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchDrag.svg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchDrag.svg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/MouseLeft.svg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/MouseLeft.svg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchTilt.svg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/TouchTilt.svg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/Touch.svg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/NavigationHelp/Touch.svg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/info-loading.gif` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/Images/info-loading.gif`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumWidget/CesiumWidget.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumWidget/CesiumWidget.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumInspector/CesiumInspector.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/CesiumInspector/CesiumInspector.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/widgets.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Widgets/widgets.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Cesium.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Cesium.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/cesiumWorkerBootstrapper.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/cesiumWorkerBootstrapper.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolylineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolylineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createSphereGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createSphereGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/transcodeCRNToDXT.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/transcodeCRNToDXT.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipseOutlineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipseOutlineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCorridorGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCorridorGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createFrustumGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createFrustumGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createRectangleGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createRectangleGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createVerticesFromGoogleEarthEnterpriseBuffer.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createVerticesFromGoogleEarthEnterpriseBuffer.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolygonGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolygonGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createFrustumOutlineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createFrustumOutlineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCylinderGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCylinderGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/upsampleQuantizedTerrainMesh.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/upsampleQuantizedTerrainMesh.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createVerticesFromHeightmap.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createVerticesFromHeightmap.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/combineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/combineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createSphereOutlineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createSphereOutlineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/decodeGoogleEarthEnterprisePacket.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/decodeGoogleEarthEnterprisePacket.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCylinderOutlineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCylinderOutlineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolylineVolumeOutlineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolylineVolumeOutlineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCorridorOutlineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCorridorOutlineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createBoxOutlineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createBoxOutlineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/transferTypedArrayTest.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/transferTypedArrayTest.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createSimplePolylineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createSimplePolylineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createBoxGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createBoxGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createVerticesFromQuantizedTerrainMesh.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createVerticesFromQuantizedTerrainMesh.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createWallGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createWallGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCircleGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCircleGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipsoidGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipsoidGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipsoidOutlineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipsoidOutlineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipseGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createEllipseGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createWallOutlineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createWallOutlineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createRectangleOutlineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createRectangleOutlineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolygonOutlineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolygonOutlineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolylineVolumeGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createPolylineVolumeGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCircleOutlineGeometry.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Workers/createCircleOutlineGeometry.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/ThirdParty/Workers/deflate.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/ThirdParty/Workers/deflate.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/ThirdParty/Workers/inflate.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/ThirdParty/Workers/inflate.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_0.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_0.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_18.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_18.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_3.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_3.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_15.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_15.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_12.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_12.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_14.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_14.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_6.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_6.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_26.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_26.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_1.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_1.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_13.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_13.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_25.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_25.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_4.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_4.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_22.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_22.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_20.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_20.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_21.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_21.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_11.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_11.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_10.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_10.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_27.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_27.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_19.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_19.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_23.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_23.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_9.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_9.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_17.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_17.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_8.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_8.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_24.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_24.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_7.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_7.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_16.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_16.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_2.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_2.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_5.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/IAU2006_XYS/IAU2006_XYS_5.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/approximateTerrainHeights.json` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/approximateTerrainHeights.json`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/0/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/0/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/1/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/0/1/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/1.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/1.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/3.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/3.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/2.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/7/2.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/1.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/1.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/3.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/3.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/2.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/3/2.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/1.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/1.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/3.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/3.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/2.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/4/2.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/1.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/1.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/3.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/3.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/2.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/0/2.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/1.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/1.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/3.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/3.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/2.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/2/2.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/1.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/1.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/3.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/3.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/2.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/5/2.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/1.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/1.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/3.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/3.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/2.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/1/2.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/1.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/1.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/3.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/3.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/2.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/2/6/2.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/tilemapresource.xml` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/tilemapresource.xml`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/3/1.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/3/1.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/3/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/3/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/0/1.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/0/1.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/0/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/0/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/2/1.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/2/1.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/2/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/2/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/1/1.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/1/1.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/1/0.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/NaturalEarthII/1/1/0.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/water.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/water.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/star.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/star.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/laundry.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/laundry.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bakery.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bakery.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/building.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/building.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/america-football.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/america-football.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/grocery.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/grocery.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/london-underground.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/london-underground.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/fire-station.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/fire-station.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/roadblock.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/roadblock.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/airfield.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/airfield.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/alcohol-shop.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/alcohol-shop.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/city.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/city.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/campsite.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/campsite.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-metro.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-metro.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cesium.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cesium.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-light.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-light.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/zoo.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/zoo.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/college.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/college.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/park2.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/park2.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bank.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bank.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/golf.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/golf.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/emergency-telephone.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/emergency-telephone.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/minefield.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/minefield.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/square.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/square.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/police.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/police.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/soccer.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/soccer.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/dog-park.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/dog-park.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/baseball.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/baseball.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/gift.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/gift.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/swimming.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/swimming.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/ferry.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/ferry.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/harbor.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/harbor.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/music.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/music.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/art-gallery.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/art-gallery.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/industrial.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/industrial.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/telephone.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/telephone.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/airport.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/airport.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-underground.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-underground.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bicycle.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bicycle.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/village.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/village.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cafe.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cafe.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/hairdresser.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/hairdresser.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/basketball.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/basketball.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/square-stroked.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/square-stroked.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/religious-jewish.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/religious-jewish.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/restaurant.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/restaurant.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/skiing.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/skiing.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/warehouse.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/warehouse.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/mobilephone.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/mobilephone.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/monument.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/monument.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/car.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/car.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/garden.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/garden.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/tennis.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/tennis.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/town-hall.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/town-hall.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/logging.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/logging.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/oil-well.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/oil-well.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/beer.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/beer.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/scooter.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/scooter.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/polling-place.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/polling-place.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/hospital.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/hospital.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/triangle.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/triangle.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/entrance.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/entrance.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/post.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/post.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/school.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/school.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bar.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bar.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/library.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/library.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/star-stroked.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/star-stroked.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/pharmacy.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/pharmacy.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/heliport.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/heliport.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/marker.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/marker.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/danger.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/danger.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/chemist.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/chemist.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/waste-basket.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/waste-basket.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/heart.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/heart.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cricket.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cricket.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cemetery.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cemetery.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/camera.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/camera.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bus.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/bus.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/museum.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/museum.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/clothing-store.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/clothing-store.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/place-of-worship.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/place-of-worship.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/wetland.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/wetland.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/commercial.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/commercial.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/parking-garage.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/parking-garage.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/fast-food.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/fast-food.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/town.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/town.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/toilets.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/toilets.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/circle-stroked.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/circle-stroked.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/embassy.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/embassy.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/slaughterhouse.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/slaughterhouse.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/circle.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/circle.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/theatre.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/theatre.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cross.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cross.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-above.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rail-above.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/farm.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/farm.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/ice-cream.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/ice-cream.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/suitcase.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/suitcase.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/religious-christian.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/religious-christian.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/marker-stroked.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/marker-stroked.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/dam.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/dam.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/playground.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/playground.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/religious-muslim.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/religious-muslim.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/pitch.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/pitch.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/land-use.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/land-use.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/triangle-stroked.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/triangle-stroked.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/parking.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/parking.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/prison.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/prison.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/lighthouse.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/lighthouse.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/park.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/park.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/lodging.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/lodging.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/shop.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/shop.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/fuel.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/fuel.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cinema.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/cinema.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rocket.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/rocket.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/disability.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/maki/disability.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/waterNormals.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/waterNormals.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_pz.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_pz.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_px.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_px.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_mx.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_mx.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_py.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_py.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_mz.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_mz.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_my.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/SkyBox/tycho2t3_80_my.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/waterNormalsSmall.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/waterNormalsSmall.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/moonSmall.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/Build/Cesium/Assets/Textures/moonSmall.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/favicon-32x32.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/cesium.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/cesium.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/third_party/font-awesome.min.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/third_party/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/third_party/bootstrap.min.css` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/css/third_party/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/blu-blank.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/blu-blank.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/ylw-blank.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/ylw-blank.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/R.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/R.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/websocket.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/websocket.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/hud.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/hud.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/cesium_setup.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/cesium_setup.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/wp.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/wp.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/context_menu.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/context_menu.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/settings.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/settings.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/core.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/core.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/tether.min.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/tether.min.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/bootstrap.min.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/jquery-3.2.1.min.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/js/third_party/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.woff2` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.eot` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.ttf` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.svg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/FontAwesome.otf` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.woff` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/pointers/move.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/pointers/move.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/models/rat.gltf` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/models/rat.gltf`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/static/DST/models/rat.glb` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/static/DST/models/rat.glb`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/cesium_web_server.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/cesium_web_server.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cesium/app/cesium_web_server.py~` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cesium/app/cesium_web_server.py~`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_signing.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_signing.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_serial.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_serial.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_example.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         super(example, self).__init__(mpstate, "example", "")
         self.status_callcount = 0
         self.boredom_interval = 10 # seconds
         self.last_bored = time.time()
 
         self.packets_mytarget = 0
         self.packets_othertarget = 0
-        self.verbose = False
 
         self.example_settings = mp_settings.MPSettings(
             [ ('verbose', bool, False),
           ])
         self.add_command('example', self.cmd_example, "example module", ['status','set (LOGSETTING)'])
 
     def usage(self):
```

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_wp.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_wp.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_msg.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_msg.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_rally.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_rally.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_GPS.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_GPS.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_heliplane.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_heliplane.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_graph.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_graph.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_restserver.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_restserver.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_timesync.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_timesync.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_tracker.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_tracker.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_param.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_param.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_gopro.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_gopro.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/__init__.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/__init__.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/magical_ui.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/magical_ui.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/glrenderer.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/glrenderer.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/wxvehicle.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/wxvehicle.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/data/quadcopter.mtl` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/data/quadcopter.mtl`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/data/arrow.obj` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/data/arrow.obj`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/data/quadcopter.obj` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/data/quadcopter.obj`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_magical/wxgeodesicgrid.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_magical/wxgeodesicgrid.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_test.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_test.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cmdlong.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cmdlong.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_antenna.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_antenna.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mode.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mode.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_layout.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_layout.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_dataflash_logger.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_dataflash_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 libraries/DataFlash/DataFlash_MAVLink.*
 '''
 
 import os
 import os.path
 from pymavlink import mavutil
 import errno
+import sys
 
 from MAVProxy.modules.lib import mp_module
 import time
 from MAVProxy.modules.lib import mp_settings
 
 
 class dataflash_logger(mp_module.MPModule):
@@ -54,15 +55,15 @@
             [('verbose', bool, False),
              ('df_target_system', int, 0),
              ('df_target_component', int, mavutil.mavlink.MAV_COMP_ID_LOG)]
         )
         self.add_command('dataflash_logger',
                          self.cmd_dataflash_logger,
                          "dataflash logging control",
-                         ['status', 'start', 'stop', 'set (LOGSETTING)'])
+                         ['status', 'start', 'stop', 'rotate', 'set (LOGSETTING)'])
         self.add_completion_function('(LOGSETTING)',
                                      self.log_settings.completion)
 
     def usage(self):
         '''show help on a command line options'''
         return "Usage: dataflash_logger <status|start|stop|set>"
 
@@ -75,14 +76,16 @@
         elif args[0] == "stop":
             self.sender = None
             self.stopped = True
         elif args[0] == "start":
             self.stopped = False
         elif args[0] == "set":
             self.log_settings.command(args[1:])
+        elif args[0] == "rotate":
+            self.rotate_log()
         else:
             print(self.usage())
 
     def _dataflash_dir(self, mpstate):
         '''returns directory path to store DF logs in.  May be relative'''
         return mpstate.status.logdir
 
@@ -94,15 +97,18 @@
             fh = open(ll_filepath, 'rb')
             log_cnt = int(fh.read()) + 1
             fh.close()
         else:
             log_cnt = 1
 
         self.lastlog_file = open(ll_filepath, 'w+b')
-        self.lastlog_file.write(log_cnt.__str__())
+        if sys.version_info[0] >= 3:
+            self.lastlog_file.write(str.encode(log_cnt.__str__()))
+        else:
+            self.lastlog_file.write(log_cnt.__str__())
         self.lastlog_file.close()
 
         return os.path.join(self.dataflash_dir, '%u.BIN' % (log_cnt,))
 
     def start_new_log(self):
         '''open a new dataflash log, reset state'''
         filename = self.new_log_filepath()
@@ -254,14 +260,40 @@
         target_comp = self.log_settings.df_target_component
         self.master.mav.remote_log_block_status_send(
             target_sys,
             target_comp,
             mavutil.mavlink.MAV_REMOTE_LOG_DATA_BLOCK_START,
             1)
 
+    def rotate_log(self):
+        '''send a start packet and rotate log'''
+        now = time.time()
+        self.time_last_start_packet_sent = now
+
+        if self.log_settings.verbose:
+            print("DFLogger: rotating")
+
+        target_sys = self.log_settings.df_target_system
+        target_comp = self.log_settings.df_target_component
+
+        for i in range(3):
+            # send 3 stop packets
+            self.master.mav.remote_log_block_status_send(
+                target_sys,
+                target_comp,
+                mavutil.mavlink.MAV_REMOTE_LOG_DATA_BLOCK_STOP,
+                1)
+        
+        self.master.mav.remote_log_block_status_send(
+            target_sys,
+            target_comp,
+            mavutil.mavlink.MAV_REMOTE_LOG_DATA_BLOCK_START,
+            1)
+        self.start_new_log()
+
     def packet_is_for_me(self, m):
         '''returns true if this packet is appropriately addressed'''
         if m.target_system != self.master.mav.srcSystem:
             return False
         if m.target_component != self.master.mav.srcComponent:
             return False
         # if have a sender we can also check the source address:
@@ -316,15 +348,15 @@
             if self.stopped:
                 # send a stop packet @1Hz until the other end gets the idea:
                 self.tell_sender_to_stop(m)
                 return
 
             if self.sender is not None:
                 size = len(m.data)
-                data = ''.join(str(chr(x)) for x in m.data[:size])
+                data = bytearray(m.data[:size])
                 ofs = size*(m.seqno)
                 self.logfile.seek(ofs)
                 self.logfile.write(data)
 
                 if m.seqno in self.missing_blocks:
                     if self.log_settings.verbose:
                         print("DFLogger: Got missing block: %d" % (m.seqno,))
```

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_firmware.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_firmware.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_adsb.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_adsb.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,34 +7,46 @@
 from math import *
 
 from MAVProxy.modules.lib import mp_module
 from MAVProxy.modules.lib import mp_settings
 from pymavlink import mavutil
 
 obc_icons = {
-    0 : 'greenplane.png',
-    1 : 'greenplane.png',
-    2 : 'cloud.png',
-    3 : 'migbird.png',
-    4 : 'hawk.png'
+    100 : 'greenplane.png',
+    101 : 'greenplane.png',
+    102 : 'cloud.png',
+    103 : 'migbird.png',
+    104 : 'hawk.png'
 }
 
 obc_radius = {
-    0 : 300,
-    1 : 300,
-    2 : 173,
-    3 : 100,
-    4 : 200
+    100 : 300,
+    101 : 300,
+    102 : 173,
+    103 : 100,
+    104 : 200
 }
     
-def get_threat_radius(obc_type):
+def get_threat_radius(m):
+
+    if m.emitter_type == 255:
+        ''' objectAvoidance Database item, squawk contains radius in cm'''
+        return m.squawk * 0.01
     '''get threat radius for an OBC item'''
-    if obc_type in obc_radius:
-        return obc_radius[obc_type]
-    return 0
+    return obc_radius.get(m.emitter_type,0)
+
+
+def get_threat_icon(m, default_icon):
+
+    if m.emitter_type == 255:
+        ''' objectAvoidance Database item, do not draw an icon'''
+        return None
+    '''get threat radius for an OBC item, else the true ADSB icon'''
+    return obc_icons.get(m.emitter_type, default_icon)
+
 
 class ADSBVehicle(object):
     '''a generic ADS-B threat'''
 
     def __init__(self, id, state):
         self.id = id
         self.state = state
@@ -182,26 +194,26 @@
             if id not in self.threat_vehicles.keys():  # check to see if the vehicle is in the dict
                 # if not then add it
                 self.threat_vehicles[id] = ADSBVehicle(id=id, state=m.to_dict())
                 for mp in self.module_matching('map*'):
                     from MAVProxy.modules.lib import mp_menu
                     from MAVProxy.modules.mavproxy_map import mp_slipmap
                     self.threat_vehicles[id].menu_item = mp_menu.MPMenuItem(name=id, returnkey=None)
-                    if m.emitter_type >= 100 and m.emitter_type-100 in obc_icons:
-                        icon = mp.map.icon(obc_icons[m.emitter_type-100])
-                        threat_radius = get_threat_radius(m.emitter_type-100)
-                    else:
-                        icon = mp.map.icon(self.threat_vehicles[id].icon)
-                        threat_radius = 0
-                    popup = mp_menu.MPMenuSubMenu('ADSB', items=[self.threat_vehicles[id].menu_item])
-                    # draw the vehicle on the map
-                    mp.map.add_object(mp_slipmap.SlipIcon(id, (m.lat * 1e-7, m.lon * 1e-7),
-                                                                    icon, layer=3, rotation=m.heading*0.01, follow=False,
-                                                                    trail=mp_slipmap.SlipTrail(colour=(0, 255, 255)),
-                                                                    popup_menu=popup))
+
+                    threat_radius = get_threat_radius(m)
+                    selected_icon = get_threat_icon(m, self.threat_vehicles[id].icon)
+                    
+                    if selected_icon is not None:
+                        # draw the vehicle on the map
+                        popup = mp_menu.MPMenuSubMenu('ADSB', items=[self.threat_vehicles[id].menu_item])
+                        icon = mp.map.icon(selected_icon)
+                        mp.map.add_object(mp_slipmap.SlipIcon(id, (m.lat * 1e-7, m.lon * 1e-7),
+                                                    icon, layer=3, rotation=m.heading*0.01, follow=False,
+                                                    trail=mp_slipmap.SlipTrail(colour=(0, 255, 255)),
+                                                    popup_menu=popup))
                     if threat_radius > 0:
                         mp.map.add_object(mp_slipmap.SlipCircle(id+":circle", 3,
                                                     (m.lat * 1e-7, m.lon * 1e-7),
                                                     threat_radius, (0, 255, 255), linewidth=1))
             else:  # the vehicle is in the dict
                 # update the dict entry
                 self.threat_vehicles[id].update(m.to_dict(), self.get_time())
```

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_fence.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_fence.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/__init__.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/__init__.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/mp_slipmap.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/mp_slipmap.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/mp_elevation.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/mp_elevation.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/elev_check.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/elev_check.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/mp_slipmap_util.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/mp_slipmap_util.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/hawk.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/hawk.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/greensub.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/greensub.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/barrell.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/barrell.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/copter.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/copter.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/migbird.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/migbird.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/loading.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/loading.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/greenrover.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/greenrover.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/cloud.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/cloud.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/iconWarning32.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/iconWarning32.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/ramp.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/ramp.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/hoop.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/hoop.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/bluesub.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/bluesub.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/home.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/home.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/greenplane.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/greenplane.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/redrover.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/redrover.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/unavailable.jpg` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/unavailable.jpg`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/redplane.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/redplane.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/orangeplane.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/orangeplane.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/camera-small-red.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/camera-small-red.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/redheli.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/redheli.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/bluerover.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/bluerover.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/blueplane.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/blueplane.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/redsub.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/redsub.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/blueheli.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/blueheli.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/data/purpleplane.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/data/purpleplane.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/mp_tile.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/mp_tile.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/mp_slipmap_ui.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/mp_slipmap_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,14 +544,16 @@
     def on_mouse_wheel(self, event):
         '''handle mouse wheel zoom changes'''
         rotation = event.GetWheelRotation() / event.GetWheelDelta()
         if rotation > 0:
             zoom = 1.0/(1.1 * rotation)
         elif rotation < 0:
             zoom = 1.1 * (-rotation)
+        else:
+            return
         self.change_zoom(zoom)
         self.redraw_map()
 
     def selected_objects(self, pos):
         '''return a list of matching objects for a position'''
         state = self.state
         selected = []
```

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/GAreader.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/GAreader.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_map/srtm.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_map/srtm.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_devop.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_devop.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_tuneopt.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_tuneopt.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_cameraview.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_cameraview.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_arm.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_arm.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_calibration.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_calibration.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_console.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_console.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/__init__.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/__init__.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_app/index.html` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_app/index.html`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_app/modestmaps.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_app/modestmaps.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_app/drone-md.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_app/drone-md.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_app/bing.js` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_app/bing.js`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_app/drone-sm.png` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_app/drone-sm.png`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_mmap/mmap_server.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_mmap/mmap_server.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/__init__.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/__init__.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/controls.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/controls.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/findjoy.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/findjoy.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/xbox-360.yml` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/xbox-360.yml`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/Logitech_WingMan_3D.yml` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/Logitech_WingMan_3D.yml`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/great-planes.yml` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/great-planes.yml`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/logitech-dual-action.yml` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/logitech-dual-action.yml`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/carolbox-usb.yml` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/carolbox-usb.yml`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/logicool-f310.yml` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/logicool-f310.yml`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/saili-simulator.yml` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/saili-simulator.yml`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/sony-playstation.yml` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/sony-playstation.yml`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_joystick/joysticks/xboxdrv-mode2.yml` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_joystick/joysticks/xboxdrv-mode2.yml`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_gimbal.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_gimbal.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/textconsole.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/textconsole.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/wxconsole_ui.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/wxconsole_ui.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/dumpstacks.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/dumpstacks.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/optparse_gui/__init__.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/optparse_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/optparse_gui/saved.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/optparse_gui/saved.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/optparse_gui/demo2.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/optparse_gui/demo2.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/optparse_gui/demo1.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/optparse_gui/demo1.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/wxhorizon.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/wxhorizon.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/opengl.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/opengl.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/live_graph_ui.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/live_graph_ui.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/wxgrapheditor.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/wxgrapheditor.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/mp_menu.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/mp_menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,16 +96,19 @@
 
     def IsChecked(self):
         '''return true if item is checked'''
         return self.checked
 
     def _append(self, menu):
         '''append this menu item to a menu'''
-        menu.AppendCheckItem(self.id(), self.name, self.description)
-        menu.Check(self.id(), self.checked)
+        try:
+            menu.AppendCheckItem(self.id(), self.name, self.description)
+            menu.Check(self.id(), self.checked)
+        except Exception:
+            pass
 
     def __str__(self):
         return "MPMenuCheckbox(%s,%s,%s,%s)" % (self.name, self.description, self.returnkey, str(self.checked))
 
 class MPMenuRadio(MPMenuItem):
     '''a MP menu item as a radio item'''
     def __init__(self, name, description='', returnkey=None, selected=None, items=[], handler=None):
```

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/grapher.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/grapher.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/graph_ui.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/graph_ui.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/wxsettings_ui.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/wxsettings_ui.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/rline.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/rline.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/mp_checklist.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/mp_checklist.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/mp_module.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/mp_module.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/mp_tabbedimage.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/mp_tabbedimage.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/mp_widgets.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/mp_widgets.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/mp_settings.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/mp_settings.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/MacOS/backend_wx.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/MacOS/backend_wx.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/MacOS/backend_wxagg.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/MacOS/backend_wxagg.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/MacOS/wxversion.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/MacOS/wxversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -496,31 +496,31 @@
 
     # Try asking for multiple versions
     test(["2.5.2", "2.5.3", "2.6"])
 
     try:
         # expecting an error on this one
         test("2.9")
-    except VersionError, e:
+    except VersionError as e:
         print("Asked for 2.9:\t got Exception:", e)
 
     # check for exception when incompatible versions are requested
     try:
         select("2.4")
         select("2.5")
-    except VersionError, e:
+    except     VersionError as e:
         print("Asked for incompatible versions, got Exception:", e)
 
     _EM_DEBUG=1
     testEM("2.6")
     testEM("2.6-unicode")
     testEM("2.6-unicode", True)
     try:
         testEM("2.9")
-    except VersionError, e:
+    except     VersionError as e:
         print("EM: Asked for 2.9:\t got Exception:", e)
 
     # cleanup
     for name in names:
         d = os.path.join('/tmp', name)
         os.rmdir(os.path.join(d, 'wx'))
         os.rmdir(d)
```

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/MacOS/backend_agg.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/MacOS/backend_agg.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/mp_substitute.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/mp_substitute.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/wxhorizon_util.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/wxhorizon_util.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/wavefront.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/wavefront.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/win_layout.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/win_layout.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/multiproc.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/multiproc.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/geodesic_grid.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/geodesic_grid.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/wxconsole.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/wxconsole.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/live_graph.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/live_graph.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/mav_fft.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/mav_fft.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/ANUGA/lat_long_UTM_conversion.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/ANUGA/lat_long_UTM_conversion.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/ANUGA/redfearn.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/ANUGA/redfearn.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/ANUGA/geo_reference.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/ANUGA/geo_reference.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/wxsettings.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/wxsettings.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/wxhorizon_ui.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/wxhorizon_ui.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/mp_image.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/mp_image.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/mav_param.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/mav_param.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/lib/mp_util.py` & `MAVProxy-1.8.9/MAVProxy/modules/lib/mp_util.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_speech.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_speech.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_messagerate.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_messagerate.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_rc.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_rc.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misc.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -75,23 +75,26 @@
         self.add_command('reboot', self.cmd_reboot, "reboot autopilot")
         self.add_command('time', self.cmd_time, "show autopilot time")
         self.add_command('shell', self.cmd_shell, "run shell command")
         self.add_command('changealt', self.cmd_changealt, "change target altitude")
         self.add_command('land', self.cmd_land, "auto land")
         self.add_command('repeat', self.cmd_repeat, "repeat a command at regular intervals",
                          ["<add|remove|clear>"])
-        self.add_command('version', self.cmd_version, "show version")
+        self.add_command('version', self.cmd_version, "fetch autopilot version")
+        self.add_command('capabilities', self.cmd_capabilities, "fetch autopilot capabilities")
         self.add_command('rcbind', self.cmd_rcbind, "bind RC receiver")
         self.add_command('led', self.cmd_led, "control board LED")
         self.add_command('oreoled', self.cmd_oreoled, "control OreoLEDs")
         self.add_command('playtune', self.cmd_playtune, "play tune remotely")
         self.add_command('devid', self.cmd_devid, "show device names from parameter IDs")
         self.add_command('gethome', self.cmd_gethome, "get HOME_POSITION")
         self.add_command('flashbootloader', self.cmd_flashbootloader, "flash bootloader (dangerous)")
         self.add_command('lockup_autopilot', self.cmd_lockup_autopilot, "lockup autopilot")
+        self.add_command('batreset', self.cmd_battery_reset, "reset battery remaining")
+        self.add_command('setorigin', self.cmd_setorigin, "set global origin")
         self.repeats = []
 
     def altitude_difference(self, pressure1, pressure2, ground_temp):
         '''calculate barometric altitude'''
         scaling = pressure2 / pressure1
         temp = ground_temp + 273.15
         return 153.8462 * temp * (1.0 - math.exp(0.190259 * math.log(scaling)))
@@ -149,15 +152,26 @@
         if len(args) > 0 and args[0] == 'IREALLYMEANIT':
             print("Sending lockup command")
             self.master.mav.command_long_send(self.settings.target_system, self.settings.target_component,
                                               mavutil.mavlink.MAV_CMD_PREFLIGHT_REBOOT_SHUTDOWN, 0,
                                               42, 24, 71, 93, 0, 0, 0)
         else:
             print("Invalid lockup command")
-        
+
+    def cmd_battery_reset(self, args):
+        '''reset battery remaining'''
+        mask = -1
+        remaining_pct = 100
+        if len(args) > 0:
+            mask = int(args[0])
+        if len(args) > 1:
+            remaining_pct = int(args[1])
+        self.master.mav.command_long_send(self.settings.target_system, self.settings.target_component,
+                                          mavutil.mavlink.MAV_CMD_BATTERY_RESET, 0,
+                                              mask, remaining_pct, 0, 0, 0, 0, 0)
 
     def cmd_time(self, args):
         '''show autopilot time'''
         tusec = self.master.field('SYSTEM_TIME', 'time_unix_usec', 0)
         if tusec == 0:
             print("No SYSTEM_TIME time available")
             return
@@ -191,20 +205,25 @@
                                               mavutil.mavlink.MAV_CMD_DO_GO_AROUND,
                                               0, 0, 0, 0, 0, 0, 0, 0)
         else:
             print("Usage: land [abort]")
 
     def cmd_version(self, args):
         '''show version'''
+        self.master.mav.autopilot_version_request_send(self.settings.target_system,
+                                                       self.settings.target_component)
+
+    def cmd_capabilities(self, args):
+        '''show capabilities'''
         self.master.mav.command_long_send(self.settings.target_system,
                                           self.settings.target_component,
                                           mavutil.mavlink.MAV_CMD_REQUEST_AUTOPILOT_CAPABILITIES,
                                           0,
                                           1, 0, 0, 0, 0, 0, 0)
-
+        
     def cmd_rcbind(self, args):
         '''start RC bind'''
         if len(args) < 1:
             print("Usage: rcbind <dsmmode>")
             return
         self.master.mav.command_long_send(self.settings.target_system,
                                           self.settings.target_component,
@@ -315,14 +334,29 @@
         '''decode device IDs from parameters'''
         for p in self.mav_param.keys():
             if p.startswith('COMPASS_DEV_ID'):
                 mp_util.decode_devid(self.mav_param[p], p)
             if p.startswith('INS_') and p.endswith('_ID'):
                 mp_util.decode_devid(self.mav_param[p], p)
 
+    def cmd_setorigin(self, args):
+        '''set global origin'''
+        if len(args) < 3:
+            print("Usage: setorigin LAT(deg) LON(deg) ALT(m)")
+            return
+        lat = float(args[0])
+        lon = float(args[1])
+        alt = float(args[2])
+        print("Setting origin to: ", lat, lon, alt)
+        self.master.mav.set_gps_global_origin_send(
+            self.settings.target_system,
+            lat*10000000, # lat
+            lon*10000000, # lon
+            alt*1000) # param7
+                
     def idle_task(self):
         '''called on idle'''
         for r in self.repeats:
             if r.event.trigger():
                 self.mpstate.functions.process_stdin(r.cmd, immediate=True)
 
 def init(mpstate):
```

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_genobstacles.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_genobstacles.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_follow.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_follow.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_terrain.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_terrain.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misseditor/__init__.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misseditor/__init__.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misseditor/button_renderer.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misseditor/button_renderer.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misseditor/me_defines.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misseditor/me_defines.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misseditor/me_event.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misseditor/me_event.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misseditor/missionEditorFrame.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misseditor/missionEditorFrame.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_misseditor/mission_editor.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_misseditor/mission_editor.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_link.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_link.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_kmlread.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_kmlread.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_txload.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_txload.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/modules/mavproxy_asterix.py` & `MAVProxy-1.8.9/MAVProxy/modules/mavproxy_asterix.py`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy/mavproxy.py` & `MAVProxy-1.8.9/MAVProxy/mavproxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         self.vehicle_type = None
         self.vehicle_name = None
         from MAVProxy.modules.lib.mp_settings import MPSettings, MPSetting
         self.settings = MPSettings(
             [ MPSetting('link', int, 1, 'Primary Link', tab='Link', range=(0,4), increment=1),
               MPSetting('streamrate', int, 4, 'Stream rate link1', range=(-1,500), increment=1),
               MPSetting('streamrate2', int, 4, 'Stream rate link2', range=(-1,500), increment=1),
-              MPSetting('heartbeat', int, 1, 'Heartbeat rate', range=(0,100), increment=1),
+              MPSetting('heartbeat', float, 1, 'Heartbeat rate (Hz)', range=(0,100), increment=0.1),
               MPSetting('mavfwd', bool, True, 'Allow forwarded control'),
               MPSetting('mavfwd_rate', bool, False, 'Allow forwarded rate control'),
               MPSetting('shownoise', bool, True, 'Show non-MAVLink data'),
               MPSetting('baudrate', int, opts.baudrate, 'baudrate for new links', range=(0,10000000), increment=1),
               MPSetting('rtscts', bool, opts.rtscts, 'enable flow control'),
               MPSetting('select_timeout', float, 0.01, 'select timeout'),
 
@@ -1132,14 +1132,21 @@
 
     if opts.speech:
         # start the speech-dispatcher early, so it doesn't inherit any ports from
         # modules/mavutil
         load_module('speech')
 
     serial_list = mavutil.auto_detect_serial(preferred_list=preferred_ports)
+    serial_list.sort(key=lambda x: x.device)
+
+    # remove OTG2 ports for dual CDC
+    if len(serial_list) == 2 and serial_list[0].device.startswith("/dev/serial/by-id"):
+        if serial_list[0].device[:-1] == serial_list[1].device[0:-1]:
+            serial_list.pop(1)
+
     if not opts.master:
         print('Auto-detected serial ports are:')
         for port in serial_list:
               print("%s" % port)
 
     # container for status information
     mpstate.settings.target_system = opts.TARGET_SYSTEM
```

### Comparing `MAVProxy-1.8.8/PKG-INFO` & `MAVProxy-1.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: MAVProxy
-Version: 1.8.8
+Version: 1.8.9
 Summary: MAVProxy MAVLink ground station
 Home-page: https://github.com/ArduPilot/MAVProxy
 Author: Andrew Tridgell
 Author-email: andrew@tridgell.net
 License: GPLv3
 Description: A MAVLink protocol proxy and ground station. MAVProxy
         is oriented towards command line operation, and is suitable for embedding in
```

### Comparing `MAVProxy-1.8.8/setup.py` & `MAVProxy-1.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup
 import os, platform
 
-version = "1.8.8"
+version = "1.8.9"
 
 def package_files(directory):
     paths = []
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join('..', path, filename))
     return paths
 
 package_data = ['modules/mavproxy_map/data/*.jpg', 
                 'modules/mavproxy_map/data/*.png',
                 'modules/mavproxy_mmap/mmap_app/*',
                 'modules/mavproxy_joystick/joysticks/*.yml',
                 'modules/mavproxy_magical/data/*.mtl',
                 'modules/mavproxy_magical/data/*.obj',
-                'modules/mavproxy_cmac_check/*.txt',
+                'modules/mavproxy_fieldcheck/*.txt',
                 'tools/graphs/*.xml',
 ]
 
 package_data.extend(package_files('MAVProxy/modules/mavproxy_cesium/app'))
 
 # note that we do not include all the real dependencies here (like matplotlib etc)
 # as that breaks the pip install. It seems that pip is not smart enough to
@@ -65,15 +65,15 @@
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 2.7',
         'Topic :: Scientific/Engineering'],
       license='GPLv3',
       packages=['MAVProxy',
                 'MAVProxy.modules',
-                'MAVProxy.modules.mavproxy_cmac_check',
+                'MAVProxy.modules.mavproxy_fieldcheck',
                 'MAVProxy.modules.mavproxy_map',
                 'MAVProxy.modules.mavproxy_mmap',
                 'MAVProxy.modules.mavproxy_misseditor',
                 'MAVProxy.modules.mavproxy_smartcamera',
                 'MAVProxy.modules.mavproxy_cesium',
                 'MAVProxy.modules.mavproxy_joystick',
                 'MAVProxy.modules.mavproxy_magical',
```

### Comparing `MAVProxy-1.8.8/README.md` & `MAVProxy-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `MAVProxy-1.8.8/MAVProxy.egg-info/PKG-INFO` & `MAVProxy-1.8.9/MAVProxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: MAVProxy
-Version: 1.8.8
+Version: 1.8.9
 Summary: MAVProxy MAVLink ground station
 Home-page: https://github.com/ArduPilot/MAVProxy
 Author: Andrew Tridgell
 Author-email: andrew@tridgell.net
 License: GPLv3
 Description: A MAVLink protocol proxy and ground station. MAVProxy
         is oriented towards command line operation, and is suitable for embedding in
```

### Comparing `MAVProxy-1.8.8/MAVProxy.egg-info/SOURCES.txt` & `MAVProxy-1.8.9/MAVProxy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -403,14 +403,15 @@
 MAVProxy/modules/lib/mp_module.py
 MAVProxy/modules/lib/mp_settings.py
 MAVProxy/modules/lib/mp_substitute.py
 MAVProxy/modules/lib/mp_tabbedimage.py
 MAVProxy/modules/lib/mp_util.py
 MAVProxy/modules/lib/mp_widgets.py
 MAVProxy/modules/lib/multiproc.py
+MAVProxy/modules/lib/ntrip.py
 MAVProxy/modules/lib/opengl.py
 MAVProxy/modules/lib/rline.py
 MAVProxy/modules/lib/testproc.py
 MAVProxy/modules/lib/textconsole.py
 MAVProxy/modules/lib/wavefront.py
 MAVProxy/modules/lib/win_layout.py
 MAVProxy/modules/lib/wx_loader.py
@@ -767,19 +768,23 @@
 MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/blu-blank.png
 MAVProxy/modules/mavproxy_cesium/app/static/DST/wp_icons/ylw-blank.png
 MAVProxy/modules/mavproxy_cesium/app/templates/context_menu.html
 MAVProxy/modules/mavproxy_cesium/app/templates/index.html
 MAVProxy/modules/mavproxy_cesium/app/templates/settings_general.html
 MAVProxy/modules/mavproxy_cesium/app/templates/settings_menu.html
 MAVProxy/modules/mavproxy_cesium/app/templates/settings_model.html
-MAVProxy/modules/mavproxy_cmac_check/__init__.py
-MAVProxy/modules/mavproxy_cmac_check/cmac-foamy-fence.txt
-MAVProxy/modules/mavproxy_cmac_check/cmac-foamy-mission-ccw.txt
-MAVProxy/modules/mavproxy_cmac_check/cmac-foamy-mission-cw.txt
-MAVProxy/modules/mavproxy_cmac_check/cmac-foamy-rally.txt
+MAVProxy/modules/mavproxy_fieldcheck/__init__.py
+MAVProxy/modules/mavproxy_fieldcheck/cmac-foamy-fence.txt
+MAVProxy/modules/mavproxy_fieldcheck/cmac-foamy-mission-ccw.txt
+MAVProxy/modules/mavproxy_fieldcheck/cmac-foamy-mission-cw.txt
+MAVProxy/modules/mavproxy_fieldcheck/cmac-foamy-rally.txt
+MAVProxy/modules/mavproxy_fieldcheck/springvalley-foamy-fence.txt
+MAVProxy/modules/mavproxy_fieldcheck/springvalley-foamy-mission-ccw.txt
+MAVProxy/modules/mavproxy_fieldcheck/springvalley-foamy-mission-cw.txt
+MAVProxy/modules/mavproxy_fieldcheck/springvalley-foamy-rally.txt
 MAVProxy/modules/mavproxy_joystick/__init__.py
 MAVProxy/modules/mavproxy_joystick/controls.py
 MAVProxy/modules/mavproxy_joystick/findjoy.py
 MAVProxy/modules/mavproxy_joystick/joysticks/Logitech_WingMan_3D.yml
 MAVProxy/modules/mavproxy_joystick/joysticks/carolbox-usb.yml
 MAVProxy/modules/mavproxy_joystick/joysticks/cypress-spektrum.yml
 MAVProxy/modules/mavproxy_joystick/joysticks/great-planes.yml
```

