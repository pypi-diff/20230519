# Comparing `tmp/sense-emu-1.1.tar.gz` & `tmp/sense-emu-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sense-emu-1.1.tar", last modified: Mon Jul  9 12:18:42 2018, max compression
+gzip compressed data, was "sense-emu-1.2.1.tar", last modified: Fri May 19 11:14:06 2023, max compression
```

## Comparing `sense-emu-1.1.tar` & `sense-emu-1.2.1.tar`

### file list

```diff
@@ -1,60 +1,59 @@
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2018-07-09 12:18:42.000000 sense-emu-1.1/
--rw-r--r--   0 dave      (1000) dave      (1000)      260 2017-10-05 16:08:18.000000 sense-emu-1.1/MANIFEST.in
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2018-07-09 12:18:42.000000 sense-emu-1.1/sense_emu.egg-info/
--rw-r--r--   0 dave      (1000) dave      (1000)       56 2018-07-09 12:18:41.000000 sense-emu-1.1/sense_emu.egg-info/requires.txt
--rw-r--r--   0 dave      (1000) dave      (1000)     2770 2018-07-09 12:18:41.000000 sense-emu-1.1/sense_emu.egg-info/PKG-INFO
--rw-r--r--   0 dave      (1000) dave      (1000)      165 2018-07-09 12:18:41.000000 sense-emu-1.1/sense_emu.egg-info/entry_points.txt
--rw-r--r--   0 dave      (1000) dave      (1000)        1 2018-07-09 12:18:41.000000 sense-emu-1.1/sense_emu.egg-info/dependency_links.txt
--rw-r--r--   0 dave      (1000) dave      (1000)     1314 2018-07-09 12:18:42.000000 sense-emu-1.1/sense_emu.egg-info/SOURCES.txt
--rw-r--r--   0 dave      (1000) dave      (1000)       10 2018-07-09 12:18:41.000000 sense-emu-1.1/sense_emu.egg-info/top_level.txt
--rw-r--r--   0 dave      (1000) dave      (1000)     2770 2018-07-09 12:18:42.000000 sense-emu-1.1/PKG-INFO
--rw-r--r--   0 dave      (1000) dave      (1000)     2712 2017-10-05 16:08:18.000000 sense-emu-1.1/setup.py
--rw-r--r--   0 dave      (1000) dave      (1000)       38 2018-07-09 12:18:42.000000 sense-emu-1.1/setup.cfg
--rw-r--r--   0 dave      (1000) dave      (1000)     1330 2017-10-05 16:08:18.000000 sense-emu-1.1/README.rst
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2018-07-09 12:18:42.000000 sense-emu-1.1/sense_emu/
--rw-r--r--   0 dave      (1000) dave      (1000)     2454 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/configparser.py
--rw-r--r--   0 dave      (1000) dave      (1000)     6891 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/pressure.py
--rw-r--r--   0 dave      (1000) dave      (1000)     4053 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/play.py
--rw-r--r--   0 dave      (1000) dave      (1000)   100403 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/sense_emu.png
--rw-r--r--   0 dave      (1000) dave      (1000)     6057 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/lock.py
--rw-r--r--   0 dave      (1000) dave      (1000)    12199 2018-07-06 19:33:13.000000 sense-emu-1.1/sense_emu/imu.py
--rw-r--r--   0 dave      (1000) dave      (1000)     2194 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/sense_emu_gui.png
--rw-r--r--   0 dave      (1000) dave      (1000)     5415 2018-07-05 11:55:48.000000 sense-emu-1.1/sense_emu/screen.py
--rw-r--r--   0 dave      (1000) dave      (1000)    27995 2018-07-05 23:49:27.000000 sense-emu-1.1/sense_emu/sense_hat.py
--rw-r--r--   0 dave      (1000) dave      (1000)    39138 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/orientation.png
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2018-07-09 12:18:42.000000 sense-emu-1.1/sense_emu/locale/
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2018-07-09 12:18:42.000000 sense-emu-1.1/sense_emu/locale/en_US/
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2018-07-09 12:18:42.000000 sense-emu-1.1/sense_emu/locale/en_US/LC_MESSAGES/
--rw-r--r--   0 dave      (1000) dave      (1000)     9357 2018-07-07 13:06:17.000000 sense-emu-1.1/sense_emu/locale/en_US/LC_MESSAGES/sense-emu.mo
--rw-r--r--   0 dave      (1000) dave      (1000)    16734 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/stick.py
--rw-r--r--   0 dave      (1000) dave      (1000)     5794 2018-07-07 12:34:35.000000 sense-emu-1.1/sense_emu/record.py
--rw-r--r--   0 dave      (1000) dave      (1000)     7118 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/humidity.py
--rw-r--r--   0 dave      (1000) dave      (1000)     4063 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/dump.py
--rw-r--r--   0 dave      (1000) dave      (1000)    21520 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/pixel_grid.png
--rw-r--r--   0 dave      (1000) dave      (1000)     2991 2018-07-06 15:12:27.000000 sense-emu-1.1/sense_emu/__init__.py
--rw-r--r--   0 dave      (1000) dave      (1000)     7882 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/RTIMU.py
--rw-r--r--   0 dave      (1000) dave      (1000)    12828 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/prefs_dialog.ui
--rw-r--r--   0 dave      (1000) dave      (1000)    30323 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/main_window.ui
--rw-r--r--   0 dave      (1000) dave      (1000)      708 2018-07-05 11:47:35.000000 sense-emu-1.1/sense_emu/gschemas.compiled
--rw-r--r--   0 dave      (1000) dave      (1000)     2560 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/common.py
--rw-r--r--   0 dave      (1000) dave      (1000)    10394 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/terminal.py
--rw-r--r--   0 dave      (1000) dave      (1000)    34466 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/sense_emu_gui.svg
--rw-r--r--   0 dave      (1000) dave      (1000)     1652 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/menu.ui
--rw-r--r--   0 dave      (1000) dave      (1000)    37018 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/gui.py
--rw-r--r--   0 dave      (1000) dave      (1000)      908 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/sense_hat_text.png
--rwxr-xr-x   0 dave      (1000) dave      (1000)     3168 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/i18n.py
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2018-07-09 12:18:42.000000 sense-emu-1.1/sense_emu/examples/
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2018-07-09 12:18:42.000000 sense-emu-1.1/sense_emu/examples/intermediate/
--rw-r--r--   0 dave      (1000) dave      (1000)     2256 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/examples/intermediate/bar_graph.py
--rw-r--r--   0 dave      (1000) dave      (1000)     1229 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/examples/intermediate/rainbow.py
--rw-r--r--   0 dave      (1000) dave      (1000)      649 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/examples/intermediate/joystick_loop.py
--rw-r--r--   0 dave      (1000) dave      (1000)      580 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/examples/intermediate/plumb_line.py
--rw-r--r--   0 dave      (1000) dave      (1000)     1853 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/examples/intermediate/line_graph.py
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2018-07-09 12:18:42.000000 sense-emu-1.1/sense_emu/examples/advanced/
--rw-r--r--   0 dave      (1000) dave      (1000)      764 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/examples/advanced/joystick_events.py
--rw-r--r--   0 dave      (1000) dave      (1000)     2435 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/examples/advanced/sensor_menu.py
-drwxr-xr-x   0 dave      (1000) dave      (1000)        0 2018-07-09 12:18:42.000000 sense-emu-1.1/sense_emu/examples/basic/
--rw-r--r--   0 dave      (1000) dave      (1000)      213 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/examples/basic/temperature.py
--rw-r--r--   0 dave      (1000) dave      (1000)      282 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/examples/basic/humidity.py
--rw-r--r--   0 dave      (1000) dave      (1000)       92 2017-10-05 16:08:18.000000 sense-emu-1.1/sense_emu/sense_hat_text.txt
--rw-r--r--   0 dave      (1000) dave      (1000)    45648 2017-10-05 16:08:18.000000 sense-emu-1.1/LICENSE.txt
+drwxr-xr-x   0 geraint   (1001) geraint   (1001)        0 2023-05-19 11:14:06.322603 sense-emu-1.2.1/
+-rw-r--r--   0 geraint   (1001) geraint   (1001)    45648 2023-05-19 11:03:25.000000 sense-emu-1.2.1/LICENSE.txt
+-rw-r--r--   0 geraint   (1001) geraint   (1001)       39 2023-05-19 11:03:25.000000 sense-emu-1.2.1/MANIFEST.in
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     2959 2023-05-19 11:14:06.326603 sense-emu-1.2.1/PKG-INFO
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     1330 2023-05-19 11:03:25.000000 sense-emu-1.2.1/README.rst
+drwxr-xr-x   0 geraint   (1001) geraint   (1001)        0 2023-05-19 11:14:06.314603 sense-emu-1.2.1/sense_emu/
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     7728 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/RTIMU.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     2882 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/__init__.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     2540 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/common.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     3707 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/dump.py
+drwxr-xr-x   0 geraint   (1001) geraint   (1001)        0 2023-05-19 11:14:06.294603 sense-emu-1.2.1/sense_emu/examples/
+drwxr-xr-x   0 geraint   (1001) geraint   (1001)        0 2023-05-19 11:14:06.318603 sense-emu-1.2.1/sense_emu/examples/advanced/
+-rw-r--r--   0 geraint   (1001) geraint   (1001)      764 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/examples/advanced/joystick_events.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     2435 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/examples/advanced/sensor_menu.py
+drwxr-xr-x   0 geraint   (1001) geraint   (1001)        0 2023-05-19 11:14:06.322603 sense-emu-1.2.1/sense_emu/examples/basic/
+-rw-r--r--   0 geraint   (1001) geraint   (1001)      282 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/examples/basic/humidity.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)      213 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/examples/basic/temperature.py
+drwxr-xr-x   0 geraint   (1001) geraint   (1001)        0 2023-05-19 11:14:06.322603 sense-emu-1.2.1/sense_emu/examples/intermediate/
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     2256 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/examples/intermediate/bar_graph.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)      649 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/examples/intermediate/joystick_loop.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     1853 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/examples/intermediate/line_graph.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)      580 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/examples/intermediate/plumb_line.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     1229 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/examples/intermediate/rainbow.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)      812 2023-05-19 11:03:45.000000 sense-emu-1.2.1/sense_emu/gschemas.compiled
+-rw-r--r--   0 geraint   (1001) geraint   (1001)    36649 2023-05-19 11:03:45.000000 sense-emu-1.2.1/sense_emu/gui.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     6957 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/humidity.py
+-rwxr-xr-x   0 geraint   (1001) geraint   (1001)     2827 2023-05-19 11:03:29.000000 sense-emu-1.2.1/sense_emu/i18n.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)    11954 2023-05-19 11:03:29.000000 sense-emu-1.2.1/sense_emu/imu.py
+drwxr-xr-x   0 geraint   (1001) geraint   (1001)        0 2023-05-19 11:14:06.294603 sense-emu-1.2.1/sense_emu/locale/
+drwxr-xr-x   0 geraint   (1001) geraint   (1001)        0 2023-05-19 11:14:06.294603 sense-emu-1.2.1/sense_emu/locale/en_US/
+drwxr-xr-x   0 geraint   (1001) geraint   (1001)        0 2023-05-19 11:14:06.322603 sense-emu-1.2.1/sense_emu/locale/en_US/LC_MESSAGES/
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     9258 2023-05-19 11:11:33.000000 sense-emu-1.2.1/sense_emu/locale/en_US/LC_MESSAGES/sense-emu.mo
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     5804 2023-05-19 11:03:29.000000 sense-emu-1.2.1/sense_emu/lock.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)    30555 2023-05-19 11:03:27.000000 sense-emu-1.2.1/sense_emu/main_window.ui
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     1652 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/menu.ui
+-rw-r--r--   0 geraint   (1001) geraint   (1001)    39138 2023-05-19 11:03:29.000000 sense-emu-1.2.1/sense_emu/orientation.png
+-rw-r--r--   0 geraint   (1001) geraint   (1001)    21520 2023-05-19 11:03:27.000000 sense-emu-1.2.1/sense_emu/pixel_grid.png
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     3903 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/play.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)    13743 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/prefs_dialog.ui
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     6747 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/pressure.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     5643 2023-05-19 11:03:29.000000 sense-emu-1.2.1/sense_emu/record.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     5354 2023-05-19 11:03:27.000000 sense-emu-1.2.1/sense_emu/screen.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)   100403 2023-05-19 11:03:45.000000 sense-emu-1.2.1/sense_emu/sense_emu.png
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     2194 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/sense_emu_gui.png
+-rw-r--r--   0 geraint   (1001) geraint   (1001)    34466 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/sense_emu_gui.svg
+-rw-r--r--   0 geraint   (1001) geraint   (1001)    27713 2023-05-19 11:03:45.000000 sense-emu-1.2.1/sense_emu/sense_hat.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)      908 2023-05-19 11:03:45.000000 sense-emu-1.2.1/sense_emu/sense_hat_text.png
+-rw-r--r--   0 geraint   (1001) geraint   (1001)       92 2023-05-19 11:03:29.000000 sense-emu-1.2.1/sense_emu/sense_hat_text.txt
+-rw-r--r--   0 geraint   (1001) geraint   (1001)    16505 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/stick.py
+-rw-r--r--   0 geraint   (1001) geraint   (1001)    10182 2023-05-19 11:03:28.000000 sense-emu-1.2.1/sense_emu/terminal.py
+drwxr-xr-x   0 geraint   (1001) geraint   (1001)        0 2023-05-19 11:14:06.318603 sense-emu-1.2.1/sense_emu.egg-info/
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     2959 2023-05-19 11:14:06.000000 sense-emu-1.2.1/sense_emu.egg-info/PKG-INFO
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     1298 2023-05-19 11:14:06.000000 sense-emu-1.2.1/sense_emu.egg-info/SOURCES.txt
+-rw-r--r--   0 geraint   (1001) geraint   (1001)        1 2023-05-19 11:14:06.000000 sense-emu-1.2.1/sense_emu.egg-info/dependency_links.txt
+-rw-r--r--   0 geraint   (1001) geraint   (1001)      165 2023-05-19 11:14:06.000000 sense-emu-1.2.1/sense_emu.egg-info/entry_points.txt
+-rw-r--r--   0 geraint   (1001) geraint   (1001)       75 2023-05-19 11:14:06.000000 sense-emu-1.2.1/sense_emu.egg-info/requires.txt
+-rw-r--r--   0 geraint   (1001) geraint   (1001)       10 2023-05-19 11:14:06.000000 sense-emu-1.2.1/sense_emu.egg-info/top_level.txt
+-rw-r--r--   0 geraint   (1001) geraint   (1001)     1946 2023-05-19 11:14:06.326603 sense-emu-1.2.1/setup.cfg
+-rw-r--r--   0 geraint   (1001) geraint   (1001)      175 2023-05-19 11:03:45.000000 sense-emu-1.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sense-emu-1.1/sense_emu.egg-info/PKG-INFO` & `sense-emu-1.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: sense-emu
-Version: 1.1
+Version: 1.2.1
 Summary: The Raspberry Pi Sense HAT Emulator library
-Home-page: http://sense-emu.readthedocs.io/
+Home-page: https://sense-emu.readthedocs.io/
 Author: Raspberry Pi Foundation
 Author-email: info@raspberrypi.org
-License: GNU General Public License v2 or later (GPLv2+)
+License: GPL-2.0-or-later
+Project-URL: Documentation, https://sense-emu.readthedocs.io/
+Project-URL: Source Code, https://github.com/astro-pi/python-sense-emu
+Project-URL: Issue Tracker, https://github.com/astro-pi/python-sense-emu/issues
 Description: .. -*- rst -*-
         
         ==================
         Sense HAT Emulator
         ==================
         
         This package emulates the Raspberry Pi `Sense HAT`_. An interactive GTK
@@ -35,16 +38,16 @@
         .. _bug tracker: https://github.com/RPi-Distro/python-sense-emu/issues
         .. _documentation: https://sense-emu.readthedocs.io
         .. _PyPI: https://pypi.python.org/pypi/sense_emu/
         .. _LGPL version 2.1: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
         .. _GPL version 2.0: https://www.gnu.org/licenses/old-licenses/gpl-2.0.html
         
         
-Keywords: raspberrypi,sense,hat
-Platform: ALL
+Keywords: raspberrypi sense hat
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: POSIX :: Linux
@@ -52,9 +55,9 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Scientific/Engineering
-Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: test
```

### Comparing `sense-emu-1.1/sense_emu.egg-info/SOURCES.txt` & `sense-emu-1.2.1/sense_emu.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 sense_emu/RTIMU.py
 sense_emu/__init__.py
 sense_emu/common.py
-sense_emu/configparser.py
 sense_emu/dump.py
 sense_emu/gschemas.compiled
 sense_emu/gui.py
 sense_emu/humidity.py
 sense_emu/i18n.py
 sense_emu/imu.py
 sense_emu/lock.py
```

### Comparing `sense-emu-1.1/PKG-INFO` & `sense-emu-1.2.1/sense_emu.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: sense-emu
-Version: 1.1
+Version: 1.2.1
 Summary: The Raspberry Pi Sense HAT Emulator library
-Home-page: http://sense-emu.readthedocs.io/
+Home-page: https://sense-emu.readthedocs.io/
 Author: Raspberry Pi Foundation
 Author-email: info@raspberrypi.org
-License: GNU General Public License v2 or later (GPLv2+)
+License: GPL-2.0-or-later
+Project-URL: Documentation, https://sense-emu.readthedocs.io/
+Project-URL: Source Code, https://github.com/astro-pi/python-sense-emu
+Project-URL: Issue Tracker, https://github.com/astro-pi/python-sense-emu/issues
 Description: .. -*- rst -*-
         
         ==================
         Sense HAT Emulator
         ==================
         
         This package emulates the Raspberry Pi `Sense HAT`_. An interactive GTK
@@ -35,16 +38,16 @@
         .. _bug tracker: https://github.com/RPi-Distro/python-sense-emu/issues
         .. _documentation: https://sense-emu.readthedocs.io
         .. _PyPI: https://pypi.python.org/pypi/sense_emu/
         .. _LGPL version 2.1: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
         .. _GPL version 2.0: https://www.gnu.org/licenses/old-licenses/gpl-2.0.html
         
         
-Keywords: raspberrypi,sense,hat
-Platform: ALL
+Keywords: raspberrypi sense hat
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: POSIX :: Linux
@@ -52,9 +55,9 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Scientific/Engineering
-Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: test
```

### Comparing `sense-emu-1.1/README.rst` & `sense-emu-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `sense-emu-1.1/sense_emu/pressure.py` & `sense-emu-1.2.1/sense_emu/pressure.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-nstr = str
-str = type('')
-
 import sys
 import os
 import io
 import mmap
 import errno
 from struct import Struct
 from collections import namedtuple
@@ -42,24 +33,24 @@
 from .common import clamp
 
 
 # See LPS25H data-sheet for details of register values
 PRESSURE_FACTOR = 4096
 TEMP_OFFSET = 37
 TEMP_FACTOR = 480
-PRESSURE_DATA = Struct(nstr(
+PRESSURE_DATA = Struct(
     '@'   # native mode
     'B'   # pressure sensor type
     '6p'  # pressure sensor name
     'l'   # P_REF
     'l'   # P_OUT
     'h'   # T_OUT
     'B'   # P_VALID
     'B'   # T_VALID
-    ))
+)
 
 PressureData = namedtuple('PressureData',
     ('type', 'name', 'P_REF', 'P_OUT', 'T_OUT', 'P_VALID', 'T_VALID'))
 
 
 def pressure_filename():
     """
@@ -83,30 +74,31 @@
     Opens the file representing the state of the pressure sensors. The
     file-like object is returned.
 
     If the file already exists we simply make sure it is the right size. If
     the file does not already exist, it is created and zeroed.
     """
     try:
-        # Attempt to open the IMU's device file and ensure it's the right size
+        # Attempt to open the pressure device's file and ensure it's the right
+        # size
         fd = io.open(pressure_filename(), 'r+b', buffering=0)
         fd.seek(PRESSURE_DATA.size)
         fd.truncate()
     except IOError as e:
-        # If the screen's device file doesn't exist, create it with reasonable
-        # initial values
+        # If the pressure device's file doesn't exist, create it with
+        # reasonable initial values
         if e.errno == errno.ENOENT:
             fd = io.open(pressure_filename(), 'w+b', buffering=0)
             fd.write(b'\x00' * PRESSURE_DATA.size)
         else:
             raise
     return fd
 
 
-class PressureServer(object):
+class PressureServer:
     def __init__(self, simulate_noise=True):
         self._random = Random()
         self._fd = init_pressure()
         self._map = mmap.mmap(self._fd.fileno(), 0, access=mmap.ACCESS_WRITE)
         data = self._read()
         if data.type != 3:
             self._write(PressureData(3, b'LPS25H', 0, 0, 0, 0, 0))
@@ -116,16 +108,16 @@
             self._pressure = data.P_OUT / 4096
             self._temperature = data.T_OUT / 480 + 42.5
         self._noise_thread = None
         self._noise_event = Event()
         self._noise_write()
         # The queue lengths are selected to accurately represent the response
         # time of the sensors
-        self._pressures = np.full((25,), self._pressure, dtype=np.float)
-        self._temperatures = np.full((25,), self._temperature, dtype=np.float)
+        self._pressures = np.full((25,), self._pressure, dtype=float)
+        self._temperatures = np.full((25,), self._temperature, dtype=float)
         self.simulate_noise = simulate_noise
 
     def close(self):
         if self._fd:
             self.simulate_noise = False
             self._map.close()
             self._fd.close()
@@ -200,9 +192,7 @@
             temperature = self.temperature
         self._write(self._read()._replace(
             P_VALID=not isnan(pressure),
             T_VALID=not isnan(temperature),
             P_OUT=0 if isnan(pressure) else int(clamp(pressure, 260, 1260) * PRESSURE_FACTOR),
             T_OUT=0 if isnan(temperature) else int((clamp(temperature, -30, 105) - TEMP_OFFSET) * TEMP_FACTOR),
             ))
-
-
```

### Comparing `sense-emu-1.1/sense_emu/play.py` & `sense-emu-1.2.1/sense_emu/play.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,28 +12,19 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-str = type('')
-
 import os
 import logging
 import argparse
 import datetime as dt
 from time import time, sleep
-from struct import Struct
 
 from . import __version__
 from .i18n import _
 from .terminal import TerminalApplication, FileType
 from .common import HEADER_REC, DATA_REC, DataRecord
 from .imu import IMUServer
 from .pressure import PressureServer
```

### Comparing `sense-emu-1.1/sense_emu/sense_emu.png` & `sense-emu-1.2.1/sense_emu/sense_emu.png`

 * *Files identical despite different names*

### Comparing `sense-emu-1.1/sense_emu/lock.py` & `sense-emu-1.2.1/sense_emu/lock.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,22 +12,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-str = type('')
-
 import sys
 import os
 import io
 import errno
 from time import time, sleep
 
 
@@ -89,15 +81,15 @@
     else:
         if os.path.exists('/dev/shm'):
             return os.path.join('/dev/shm', fname)
         else:
             return os.path.join('/tmp', fname)
 
 
-class EmulatorLock(object):
+class EmulatorLock:
     def __init__(self, name):
         self._filename = lock_filename()
         self.name = name # XXX not currently used
 
     def __enter__(self):
         self.acquire()
         return self
@@ -127,24 +119,24 @@
         by anything wishing to read the registers and wanting to ensure there's
         something driving them (i.e. any consumer of SenseHat).
 
         Returns ``True`` if the lock was acquired before *timeout* seconds
         elapsed, or ``False`` otherwise. If *timeout* is ``None`` (the default)
         wait indefinitely.
         """
+        # XXX Either add a "launch" param to this method, or add a launch
+        # method to the class so that consumers can use the lock to launch
+        # an appropriate emulation
         end = time()
-        if timeout is None:
-            wait = 0.1
-        else:
+        if timeout is not None:
             end += timeout
-            wait = max(0, timeout / 10)
         while not self._is_held() or self._is_stale():
             if time() > end:
                 return False
-            sleep(wait)
+            sleep(0.1)
         return True
 
     @property
     def mine(self):
         """
         Returns True if the current process holds the lock.
         """
@@ -179,17 +171,9 @@
                 return int(lockfile.readline().decode('ascii').strip())
             except ValueError:
                 return None
             finally:
                 lockfile.close()
 
     def _write_pid(self):
-        try:
-            lockfile = io.open(self._filename, 'x')
-        except ValueError as e:
-            # We're on py2.x or 3.2
-            mode = 0o666
-            lockfile = os.fdopen(os.open(
-                self._filename, os.O_CREAT | os.O_EXCL | os.O_WRONLY, mode), 'w')
-        lockfile.write('%d\n' % os.getpid())
-        lockfile.close()
-
+        with io.open(self._filename, 'x', encoding='ascii') as lockfile:
+            lockfile.write('%d\n' % os.getpid())
```

### Comparing `sense-emu-1.1/sense_emu/imu.py` & `sense-emu-1.2.1/sense_emu/imu.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-nstr = str
-str = type('')
-
 import sys
 import os
 import io
 import mmap
 import time
 import errno
 import subprocess
@@ -43,26 +34,27 @@
 
 
 # See LSM9DS1 data-sheet for details of register values
 ACCEL_FACTOR = 4081.6327
 GYRO_FACTOR = 57.142857
 COMPASS_FACTOR = 7142.8571
 ORIENT_FACTOR = 5214.1892
-IMU_DATA = Struct(nstr(
+IMU_DATA = Struct(
     '@'   # native mode
     'B'   # IMU sensor type
     '20p' # IMU sensor name
     'Q'   # timestamp
     'hhh' # OUT_X_G, OUT_Y_G, OUT_Z_G
     'hhh' # OUT_X_XL, OUT_Y_XL, OUT_Z_XL
     'hhh' # OUT_X_M, OUT_Y_M, OUT_Z_M
     'hhh' # Orientation X, Y, Z
-    ))
+)
 
-IMUData = namedtuple('IMUData', ('type', 'name', 'timestamp', 'accel', 'gyro', 'compass', 'orient'))
+IMUData = namedtuple('IMUData', (
+    'type', 'name', 'timestamp', 'accel', 'gyro', 'compass', 'orient'))
 
 
 def imu_filename():
     """
     Return the filename used to represent the state of the emulated sense HAT's
     IMU sensors. On UNIX we try ``/dev/shm`` then fall back to ``/tmp``; on
     Windows we use whatever ``%TEMP%`` contains.
@@ -88,33 +80,31 @@
     """
     try:
         # Attempt to open the IMU's device file and ensure it's the right size
         fd = io.open(imu_filename(), 'r+b', buffering=0)
         fd.seek(IMU_DATA.size)
         fd.truncate()
     except IOError as e:
-        # If the screen's device file doesn't exist, create it with reasonable
+        # If the IMU device's file doesn't exist, create it with reasonable
         # initial values
         if e.errno == errno.ENOENT:
             fd = io.open(imu_filename(), 'w+b', buffering=0)
             fd.write(b'\x00' * IMU_DATA.size)
         else:
             raise
     return fd
 
 
 # Find the best available time-source for the timestamp() function. The best
 # source will preferably be monotonic, and high-resolution
 try:
     _time = time.monotonic # 3.3+ (only guaranteed in 3.5+)
 except AttributeError:
-    try:
-        _time = time.perf_counter # 3.3+
-    except AttributeError:
-        _time = time.time # fallback for 2.7
+    _time = time.perf_counter # 3.3+
+
 def timestamp():
     """
     Returns a timestamp as an integer number of microseconds after some
     arbitrary basis (only comparisons of consecutive calls are meaningful).
     """
     return int(_time() * 1000000)
 
@@ -123,15 +113,15 @@
 V = lambda x, y, z: np.array((x, y, z))
 O = V(0, 0, 0)
 X = V(1, 0, 0)
 Y = V(0, 1, 0)
 Z = V(0, 0, 1)
 
 
-class IMUServer(object):
+class IMUServer:
     def __init__(self, simulate_world=True):
         self._random = Random()
         self._fd = init_imu()
         self._map = mmap.mmap(self._fd.fileno(), 0, access=mmap.ACCESS_WRITE)
         data = self._read()
         self._gravity = Z
         self._north = 0.33 * X
@@ -151,17 +141,17 @@
         self._world_thread = None
         self._world_event = Event()
         self._world_iter = self._world_state()
         self._world_write()
         # These queue lengths were arbitrarily selected to smooth the action of
         # the orientation sliders in the GUI; they bear no particular relation
         # to the hardware
-        self._gyros = np.full((10, 3), self._gyro, dtype=np.float)
-        self._accels = np.full((10, 3), self._accel, dtype=np.float)
-        self._comps = np.full((10, 3), self._compass, dtype=np.float)
+        self._gyros = np.full((10, 3), self._gyro, dtype=float)
+        self._accels = np.full((10, 3), self._accel, dtype=float)
+        self._comps = np.full((10, 3), self._compass, dtype=float)
         self.simulate_world = simulate_world
 
     def close(self):
         if self._fd:
             self.simulate_world = False
             self._map.close()
             self._fd.close()
@@ -343,8 +333,7 @@
                 ),
             orient=V(
                 int(clamp(orient[0], -180, 180) * ORIENT_FACTOR),
                 int(clamp(orient[1], -180, 180) * ORIENT_FACTOR),
                 int(clamp(orient[2], -180, 180) * ORIENT_FACTOR),
                 )
             ))
-
```

### Comparing `sense-emu-1.1/sense_emu/sense_emu_gui.png` & `sense-emu-1.2.1/sense_emu/sense_emu_gui.png`

 * *Files identical despite different names*

### Comparing `sense-emu-1.1/sense_emu/screen.py` & `sense-emu-1.2.1/sense_emu/screen.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,23 +12,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-nstr = str
-str = type('')
-
 import sys
 import os
 import io
 import errno
 import mmap
 import struct
 from threading import Thread, Event
@@ -78,15 +69,15 @@
             fd.write(b'\x00\x00' * 64)
             fd.write(b''.join(chr(i).encode('ascii') for i in GAMMA_DEFAULT))
         else:
             raise
     return fd
 
 
-class ScreenClient(object):
+class ScreenClient:
     def __init__(self):
         self._fd = init_screen()
         self._map = mmap.mmap(self._fd.fileno(), 0, access=mmap.ACCESS_READ)
         # Construct arrays representing the LED states (_screen) and the user
         # controlled gamma lookup table (_gamma)
         self._screen = np.frombuffer(self._map, dtype=np.uint16, count=64).reshape((8, 8))
         self._gamma = np.frombuffer(self._map, dtype=np.uint8, count=32, offset=128)
@@ -115,14 +106,15 @@
     def _touch_run(self):
         # "touch" the screen's frame-buffer once a second. This ensures that
         # the screen always updates at least once a second and works around the
         # issue that screen updates can be lost due to lack of resolution of
         # the file modification timestamps. Unfortunately, futimes(3) is not
         # universally supported, and only available in Python 3.3+ so this gets
         # a bit convoluted...
+        # FIXME only need 3.3+ support now; work out which bits are 2.7 and excise
         touch = lambda: os.utime(self._fd.fileno())
         try:
             if os.utime in os.supports_fd:
                 touch()
             else:
                 raise NotImplementedError
         except (AttributeError, NotImplementedError) as e:
@@ -145,8 +137,7 @@
         a = np.take(self._gamma, a)
         a = np.take(self._gamma_rgbled, a)
         return a
 
     @property
     def timestamp(self):
         return os.fstat(self._fd.fileno()).st_mtime
-
```

### Comparing `sense-emu-1.1/sense_emu/sense_hat.py` & `sense-emu-1.2.1/sense_emu/sense_hat.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,49 +12,38 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
-#!/usr/bin/python
-
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-nstr = str
-str = type('')
-
 import struct
 import io
 import os
 import sys
 import math
 import time
 import numpy as np
 import shutil
 import glob
 import array
 import struct
-import subprocess
+import subprocess as sp
 import warnings
 from PIL import Image  # pillow
 from copy import deepcopy
 
 
 from . import RTIMU
 from .lock import EmulatorLock
 from .stick import SenseStick
 from .screen import init_screen, GAMMA_DEFAULT, GAMMA_LOW
 
 
-class SenseHat(object):
+class SenseHat:
     """
     The main interface the Raspberry Pi Sense HAT.
 
     This class provides properties to query the various sensors on the Sense
     HAT (:attr:`temp`, :attr:`pressure`, :attr:`humidity`, :attr:`gyro`, etc.)
     and methods to control the LED "screen" on the HAT (:meth:`set_pixel`,
     :meth:`set_pixels`).
@@ -85,25 +74,25 @@
             imu_settings_file='RTIMULib',
             text_assets='sense_hat_text'
         ):
 
         lock = EmulatorLock('sense_emu')
         if not lock.wait(1):
             warnings.warn(Warning('No emulator detected; spawning sense_emu_gui'))
-            with io.open(os.devnull, 'r+b') as devnull:
-                try:
-                    setpgrp = os.setpgrp
-                except AttributeError:
-                    setpgrp = None
-                # setpgrp is called to spawn a new process group, ensuring
-                # that signals from the interpreter (e.g. the user pressing
-                # Ctrl+C) don't get sent to the emulator too
-                subprocess.Popen(['sense_emu_gui'], preexec_fn=setpgrp,
-                                 stdin=devnull, stdout=devnull, stderr=devnull,
-                                 close_fds=True)
+            try:
+                setpgrp = os.setpgrp
+            except AttributeError:
+                setpgrp = None
+            # setpgrp is called to spawn a new process group, ensuring that
+            # signals from the interpreter (e.g. the user pressing Ctrl+C)
+            # don't get sent to the emulator too
+            sp.Popen(
+                ['sense_emu_gui'], preexec_fn=setpgrp,
+                stdin=sp.DEVNULL, stdout=sp.DEVNULL, stderr=sp.DEVNULL,
+                close_fds=True)
 
         self._fb_device = self._get_fb_device()
         if self._fb_device is None:
             raise OSError('Cannot detect %s device' % self.SENSE_HAT_FB_NAME)
 
         # 0 is With B+ HDMI port facing downwards
         pix_map0 = np.array([
@@ -551,30 +540,30 @@
         self.set_pixels(coloured_pixels)
         self._rotation = previous_rotation
 
     @property
     def gamma(self):
         with open(self._fb_device, 'rb') as f:
             f.seek(128)
-            return struct.unpack(nstr('32B'), f.read(32))
+            return struct.unpack('32B', f.read(32))
 
     @gamma.setter
     def gamma(self, buffer):
-        if len(buffer) is not 32:
+        if len(buffer) != 32:
             raise ValueError('Gamma array must be of length 32')
 
         if not all(b <= 31 for b in buffer):
             raise ValueError('Gamma values must be bewteen 0 and 31')
 
         if not isinstance(buffer, array.array):
-            buffer = array.array(nstr('B'), buffer)
+            buffer = array.array('B', buffer)
 
         with open(self._fb_device, 'rb+') as f:
             f.seek(128)
-            f.write(struct.pack(nstr('32B'), *buffer))
+            f.write(struct.pack('32B', *buffer))
 
     def gamma_reset(self):
         """
         Resets the LED matrix gamma correction to default
         """
         self.gamma = GAMMA_DEFAULT
```

### Comparing `sense-emu-1.1/sense_emu/orientation.png` & `sense-emu-1.2.1/sense_emu/orientation.png`

 * *Files identical despite different names*

### Comparing `sense-emu-1.1/sense_emu/locale/en_US/LC_MESSAGES/sense-emu.mo` & `sense-emu-1.2.1/sense_emu/locale/en_US/LC_MESSAGES/sense-emu.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-07-07 13:35+0100\n"
 "PO-Revision-Date: 2016-08-17 10:49+0100\n"
 "Last-Translator: Dave Jones <dave@waveform.org.uk>\n"
 "Language-Team: English\n"
 "Language: en_US\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -94,17 +93,14 @@
 
 msgid "Invalid magic number at start of input"
 msgstr "Invalid magic number at start of input"
 
 msgid "Joystick"
 msgstr "Joystick"
 
-msgid "No such attribute %r"
-msgstr "No such attribute %r"
-
 msgid "Orientation"
 msgstr "Orientation"
 
 msgid "Orientation scale"
 msgstr "Orientation scale"
 
 msgid "Pitch"
```

### Comparing `sense-emu-1.1/sense_emu/stick.py` & `sense-emu-1.2.1/sense_emu/stick.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,39 +12,27 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-native_str = str
-str = type('')
-
 import io
 import os
 import sys
 import glob
 import errno
 import struct
 import select
 import inspect
 import socket
 from functools import wraps
 from collections import namedtuple
 from threading import Thread, Event
-try:
-    from queue import Queue, Empty
-except:
-    from Queue import Queue, Empty # py2.x
+from queue import Queue, Empty
 from time import sleep
 
 
 DIRECTION_UP     = 'up'
 DIRECTION_DOWN   = 'down'
 DIRECTION_LEFT   = 'left'
 DIRECTION_RIGHT  = 'right'
@@ -141,20 +129,20 @@
     thread.daemon = True
     thread.start()
     # Construct file object on top of the socket which we'll return as the
     # result
     return client.makefile('rb', 0)
 
 
-class SenseStick(object):
+class SenseStick:
     """
     Represents the joystick on the Sense HAT.
     """
     SENSE_HAT_EVDEV_NAME = 'Raspberry Pi Sense HAT Joystick'
-    EVENT_FORMAT = native_str('llHHI')
+    EVENT_FORMAT = 'llHHI'
     EVENT_SIZE = struct.calcsize(EVENT_FORMAT)
 
     EV_KEY = 0x01
 
     STATE_RELEASE = 0
     STATE_PRESS = 1
     STATE_HOLD = 2
@@ -414,15 +402,15 @@
 
     @direction_any.setter
     def direction_any(self, value):
         self._callbacks['*'] = self._wrap_callback(value)
         self._start_stop_thread()
 
 
-class StickServer(object):
+class StickServer:
     def __init__(self):
         family, sock_type, addr = stick_address()
         server = socket.socket(family, sock_type)
         if family == socket.AF_UNIX:
             try:
                 # Kill any pre-existing socket
                 os.unlink(addr)
```

### Comparing `sense-emu-1.1/sense_emu/record.py` & `sense-emu-1.2.1/sense_emu/record.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,29 +12,19 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>
 
-
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-str = type('')
-
 import os
 import logging
 import argparse
 from threading import Thread, Event
 from time import time, sleep
-from struct import Struct
 
 from . import __version__
 from .i18n import _
 from .terminal import TerminalApplication, FileType
 from .common import HEADER_REC, DATA_REC
```

### Comparing `sense-emu-1.1/sense_emu/humidity.py` & `sense-emu-1.2.1/sense_emu/humidity.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,23 +12,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-nstr = str
-str = type('')
-
 import sys
 import os
 import io
 import mmap
 import errno
 from struct import Struct
 from collections import namedtuple
@@ -41,15 +32,15 @@
 
 from .common import clamp
 
 
 # See HTS221 data-sheet for details of register values
 HUMIDITY_FACTOR = 256
 TEMP_FACTOR = 64
-HUMIDITY_DATA = Struct(nstr(
+HUMIDITY_DATA = Struct(
     '@'   # native mode
     'B'   # humidity sensor type
     '6p'  # humidity sensor name
     'B'   # H0
     'B'   # H1
     'H'   # T0
     'H'   # T1
@@ -57,20 +48,20 @@
     'h'   # H1_OUT
     'h'   # T0_OUT
     'h'   # T1_OUT
     'h'   # H_OUT
     'h'   # T_OUT
     'B'   # H_VALID
     'B'   # T_VALID
-    ))
+)
 
 HumidityData = namedtuple('HumidityData', (
     'type', 'name', 'H0', 'H1', 'T0', 'T1', 'H0_OUT', 'H1_OUT',
     'T0_OUT', 'T1_OUT', 'H_OUT', 'T_OUT', 'H_VALID', 'T_VALID')
-    )
+)
 
 
 def humidity_filename():
     """
     Return the filename used to represent the state of the emulated sense HAT's
     humidity sensor. On UNIX we try ``/dev/shm`` then fall back to ``/tmp``; on
     Windows we use whatever ``%TEMP%`` contains
@@ -97,25 +88,25 @@
     try:
         # Attempt to open the humidity sensor's file and ensure it's the right
         # size
         fd = io.open(humidity_filename(), 'r+b', buffering=0)
         fd.seek(HUMIDITY_DATA.size)
         fd.truncate()
     except IOError as e:
-        # If the screen's device file doesn't exist, create it with reasonable
-        # initial values
+        # If the humidity device's file doesn't exist, create it with
+        # reasonable initial values
         if e.errno == errno.ENOENT:
             fd = io.open(humidity_filename(), 'w+b', buffering=0)
             fd.write(b'\x00' * HUMIDITY_DATA.size)
         else:
             raise
     return fd
 
 
-class HumidityServer(object):
+class HumidityServer:
     def __init__(self, simulate_noise=True):
         self._random = Random()
         self._fd = init_humidity()
         self._map = mmap.mmap(self._fd.fileno(), 0, access=mmap.ACCESS_WRITE)
         data = self._read()
         if data.type != 2:
             self._write(HumidityData(2, b'HTS221', 0, 100, 0, 100, 0, 25600, 0, 6400, 0, 0, 0, 0))
@@ -125,16 +116,16 @@
             self._humidity = data.H_OUT / HUMIDITY_FACTOR
             self._temperature = data.T_OUT / TEMP_FACTOR
         self._noise_thread = None
         self._noise_event = Event()
         self._noise_write()
         # The queue lengths are selected to accurately represent the response
         # time of the sensors
-        self._humidities = np.full((10,), self._humidity, dtype=np.float)
-        self._temperatures = np.full((31,), self._temperature, dtype=np.float)
+        self._humidities = np.full((10,), self._humidity, dtype=float)
+        self._temperatures = np.full((31,), self._temperature, dtype=float)
         self.simulate_noise = simulate_noise
 
     def close(self):
         if self._fd:
             self.simulate_noise = False
             self._map.close()
             self._fd.close()
```

### Comparing `sense-emu-1.1/sense_emu/dump.py` & `sense-emu-1.2.1/sense_emu/dump.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,31 +12,21 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-str = type('')
-
-
 import sys
 import os
 import csv
 import logging
 import argparse
 import datetime as dt
-from time import time, sleep
-from struct import Struct
+from time import time
 
 from . import __version__
 from .i18n import _
 from .terminal import TerminalApplication, FileType
 from .common import HEADER_REC, DATA_REC, DataRecord
 
 
@@ -50,19 +40,15 @@
             '--timestamp-format', action='store', default='%Y-%m-%dT%H:%M:%S.%f', metavar='FMT',
             help=_('the format to use when outputting the record timestamp '
             '(default: %(default)s)'))
         self.parser.add_argument(
             '--header', action='store_true', default=False,
             help=_('if specified, output column headers'))
         self.parser.add_argument('input', type=FileType('rb'))
-        # Eurgh ... csv module under Python 2 only outputs byte-strings
-        if sys.version_info.major == 2:
-            self.parser.add_argument('output', type=FileType('wb'))
-        else:
-            self.parser.add_argument('output', type=FileType('w', encoding='utf-8'))
+        self.parser.add_argument('output', type=FileType('w', encoding='utf-8'))
 
     def source(self, f):
         logging.info(_('Reading header'))
         magic, ver, offset = HEADER_REC.unpack(f.read(HEADER_REC.size))
         if magic != b'SENSEHAT':
             raise IOError(_('Invalid magic number at start of input'))
         if ver != 1:
```

### Comparing `sense-emu-1.1/sense_emu/pixel_grid.png` & `sense-emu-1.2.1/sense_emu/pixel_grid.png`

 * *Files 1% similar despite different names*

#### sng

```diff
@@ -2,21 +2,21 @@
 IHDR {
     width: 512; height: 512; bitdepth: 8;
     using color alpha;
 }
 bKGD {red: 255;  green: 255;  blue: 255;}
 pHYs {xpixels: 13437; ypixels: 13437; per: meter;}  # (341 dpi)
 tIME {
-    # 13 Sep 2016 15:05:00 GMT
-    year:   2016
+    #  2 Sep 2021 23:36:05 GMT
+    year:   2021
     month:  9
-    day:    13
-    hour:   15
-    minute: 5
-    second: 0
+    day:    2
+    hour:   23
+    minute: 36
+    second: 5
 }
 tEXt {
     keyword: "Comment";
     text: "Created with GIMP";
 }
 IMAGE {
     pixels hex
```

### Comparing `sense-emu-1.1/sense_emu/__init__.py` & `sense-emu-1.2.1/sense_emu/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,21 +14,14 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
 "The Raspberry Pi Sense HAT Emulator library"
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-
 import sys
 
 from .sense_hat import SenseHat, SenseHat as AstroPi
 from .stick import (
     SenseStick,
     InputEvent,
     DIRECTION_UP,
@@ -38,15 +31,15 @@
     DIRECTION_MIDDLE,
     ACTION_PRESSED,
     ACTION_RELEASED,
     ACTION_HELD,
     )
 
 __project__      = 'sense-emu'
-__version__      = '1.1'
+__version__      = '1.2.1'
 __author__       = 'Raspberry Pi Foundation'
 __author_email__ = 'info@raspberrypi.org'
 __url__          = 'http://sense-emu.readthedocs.io/'
 __platforms__    = ['ALL']
 
 __classifiers__ = [
     'Development Status :: 5 - Production/Stable',
@@ -93,9 +86,7 @@
         'sense_play = sense_emu.play:app',
         'sense_csv = sense_emu.dump:app',
         ],
     'gui_scripts': [
         'sense_emu_gui = sense_emu.gui:main',
         ],
     }
-
-
```

### Comparing `sense-emu-1.1/sense_emu/RTIMU.py` & `sense-emu-1.2.1/sense_emu/RTIMU.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,40 +12,30 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-nstr = str
-str = type('')
-
-
 import mmap
 from time import time
 
 import numpy as np
 
 from .pressure import init_pressure, PRESSURE_DATA, PressureData, PRESSURE_FACTOR, TEMP_FACTOR, TEMP_OFFSET
 from .humidity import init_humidity, HUMIDITY_DATA, HumidityData
 from .imu import init_imu, IMU_DATA, IMUData, ACCEL_FACTOR, GYRO_FACTOR, COMPASS_FACTOR, ORIENT_FACTOR
 
 
-class Settings(object):
+class Settings:
     def __init__(self, path):
         self.path = path
 
 
-class RTIMU(object):
+class RTIMU:
     def __init__(self, settings):
         self.settings = settings
         self._fd = init_imu()
         self._map = mmap.mmap(self._fd.fileno(), 0, access=mmap.ACCESS_READ)
         self._last_data = None
         self._imu_data = {
             'accel':            (0.0, 0.0, 0.0),
@@ -248,9 +238,7 @@
                 )
 
     def humidityType(self):
         return self._read().type
 
     def humidityName(self):
         return self._read().name.decode('ascii')
-
-
```

### Comparing `sense-emu-1.1/sense_emu/prefs_dialog.ui` & `sense-emu-1.2.1/sense_emu/prefs_dialog.ui`

 * *Files 5% similar despite different names*

#### Comparing `sense-emu-1.1/sense_emu/prefs_dialog.ui` & `sense-emu-1.2.1/sense_emu/prefs_dialog.ui`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- Generated with glade 3.18.3 
+<!-- Generated with glade 3.22.2 
 
 sense_emu_gui - An emulator for the Raspberry Pi Sense HAT
 Copyright (C) 2016 Raspberry Pi Foundation
 
 This program is free software; you can redistribute it and/or
 modify it under the terms of the GNU General Public License
 as published by the Free Software Foundation; either version 2
@@ -18,31 +18,33 @@
 along with this program; if not, write to the Free Software
 Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 Author: Dave Jones
 
 -->
 <interface domain="sense-emu">
-  <requires lib="gtk+" version="3.4"/>
+  <requires lib="gtk+" version="3.18"/>
   <!-- interface-license-type gplv2 -->
   <!-- interface-name sense_emu_gui -->
   <!-- interface-description An emulator for the Raspberry Pi Sense HAT -->
   <!-- interface-copyright 2016 Raspberry Pi Foundation -->
   <!-- interface-authors Dave Jones -->
   <object class="GtkAdjustment" id="screen_fps">
     <property name="lower">1</property>
     <property name="upper">60</property>
     <property name="value">25</property>
     <property name="step_increment">1</property>
     <property name="page_increment">5</property>
   </object>
-  <object class="GtkDialog" id="window">
+  <template class="PrefsDialog" parent="GtkDialog">
     <property name="can_focus">False</property>
-    <property name="resizable">False</property>
     <property name="type_hint">dialog</property>
+    <child type="titlebar">
+      <placeholder/>
+    </child>
     <child internal-child="vbox">
       <object class="GtkBox" id="dialog_vbox">
         <property name="visible">True</property>
         <property name="can_focus">False</property>
         <property name="margin_left">6</property>
         <property name="margin_right">6</property>
         <property name="margin_top">6</property>
@@ -56,28 +58,29 @@
             <property name="layout_style">end</property>
             <child>
               <object class="GtkButton" id="close_button">
                 <property name="label">gtk-close</property>
                 <property name="visible">True</property>
                 <property name="can_focus">True</property>
                 <property name="can_default">True</property>
+                <property name="has_default">True</property>
                 <property name="receives_default">False</property>
                 <property name="use_stock">True</property>
                 <signal name="clicked" handler="close_clicked" swapped="no"/>
               </object>
               <packing>
                 <property name="expand">True</property>
                 <property name="fill">True</property>
                 <property name="position">1</property>
               </packing>
             </child>
           </object>
           <packing>
             <property name="expand">False</property>
-            <property name="fill">False</property>
+            <property name="fill">True</property>
             <property name="position">0</property>
           </packing>
         </child>
         <child>
           <object class="GtkGrid" id="root_grid">
             <property name="visible">True</property>
             <property name="can_focus">False</property>
@@ -111,30 +114,28 @@
             <child>
               <object class="GtkCheckButton" id="env_check">
                 <property name="label" translatable="yes">Environment sensors</property>
                 <property name="visible">True</property>
                 <property name="can_focus">True</property>
                 <property name="receives_default">False</property>
                 <property name="tooltip_text" translatable="yes">When checked, the emulator will continually simulate &quot;noise&quot; on the environment sensors (the temperature, pressure, and humidity sliders)</property>
-                <property name="xalign">0</property>
                 <property name="draw_indicator">True</property>
               </object>
               <packing>
                 <property name="left_attach">1</property>
                 <property name="top_attach">3</property>
               </packing>
             </child>
             <child>
               <object class="GtkCheckButton" id="imu_check">
                 <property name="label" translatable="yes">Inertial measurement unit</property>
                 <property name="visible">True</property>
                 <property name="can_focus">True</property>
                 <property name="receives_default">False</property>
                 <property name="tooltip_text" translatable="yes">When checked, the emulator will constantly simulate accelerometer (gravity induced), gyroscope (rate of change), and magnetometer (relative North) values based on the yaw, pitch, and roll sliders</property>
-                <property name="xalign">0</property>
                 <property name="draw_indicator">True</property>
               </object>
               <packing>
                 <property name="left_attach">1</property>
                 <property name="top_attach">4</property>
               </packing>
             </child>
@@ -193,15 +194,14 @@
             <child>
               <object class="GtkRadioButton" id="orientation_balance">
                 <property name="label">-180° ⋯⋯ 0° ⋯⋯ 180°</property>
                 <property name="visible">True</property>
                 <property name="can_focus">True</property>
                 <property name="receives_default">False</property>
                 <property name="tooltip_text" translatable="yes">When selected, the orientation sliders will have a minimum of -180°, a mid-point at 0°, and a maximum of 180°</property>
-                <property name="xalign">0</property>
                 <property name="active">True</property>
                 <property name="draw_indicator">True</property>
                 <signal name="toggled" handler="orientation_changed" swapped="no"/>
               </object>
               <packing>
                 <property name="left_attach">1</property>
                 <property name="top_attach">0</property>
@@ -210,15 +210,14 @@
             <child>
               <object class="GtkRadioButton" id="orientation_circle">
                 <property name="label">0° ⋯⋯ 180° ⋯⋯ 360°</property>
                 <property name="visible">True</property>
                 <property name="can_focus">True</property>
                 <property name="receives_default">False</property>
                 <property name="tooltip_text" translatable="yes">When selected, the orientation sliders will have a minimum of 0°, a mid-point at 180°, and a maximum of 360°</property>
-                <property name="xalign">0</property>
                 <property name="active">True</property>
                 <property name="draw_indicator">True</property>
                 <property name="group">orientation_balance</property>
                 <signal name="toggled" handler="orientation_changed" swapped="no"/>
               </object>
               <packing>
                 <property name="left_attach">1</property>
@@ -228,29 +227,52 @@
             <child>
               <object class="GtkRadioButton" id="orientation_modulo">
                 <property name="label">180° ⋯⋯ 360|0° ⋯⋯ 180°</property>
                 <property name="visible">True</property>
                 <property name="can_focus">True</property>
                 <property name="receives_default">False</property>
                 <property name="tooltip_text" translatable="yes">When selected, the orientation sliders will have a minimum of 180°, a mid-point at 0° (immediately after 359°), and a maximum of 180°</property>
-                <property name="xalign">0</property>
                 <property name="active">True</property>
                 <property name="draw_indicator">True</property>
                 <property name="group">orientation_balance</property>
                 <signal name="toggled" handler="orientation_changed" swapped="no"/>
               </object>
               <packing>
                 <property name="left_attach">1</property>
                 <property name="top_attach">2</property>
               </packing>
             </child>
+            <child>
+              <object class="GtkLabel" id="editor_label">
+                <property name="visible">True</property>
+                <property name="can_focus">False</property>
+                <property name="label" translatable="yes">Editor command</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left_attach">0</property>
+                <property name="top_attach">6</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkEntry" id="editor_entry">
+                <property name="visible">True</property>
+                <property name="can_focus">True</property>
+                <property name="hexpand">True</property>
+                <property name="placeholder_text" translatable="yes">editor %s</property>
+              </object>
+              <packing>
+                <property name="left_attach">1</property>
+                <property name="top_attach">6</property>
+              </packing>
+            </child>
           </object>
           <packing>
             <property name="expand">False</property>
-            <property name="fill">True</property>
+            <property name="fill">False</property>
             <property name="position">1</property>
           </packing>
         </child>
       </object>
     </child>
-  </object>
+  </template>
 </interface>
```

### Comparing `sense-emu-1.1/sense_emu/main_window.ui` & `sense-emu-1.2.1/sense_emu/main_window.ui`

 * *Files 0% similar despite different names*

#### Comparing `sense-emu-1.1/sense_emu/main_window.ui` & `sense-emu-1.2.1/sense_emu/main_window.ui`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- Generated with glade 3.18.3 
+<!-- Generated with glade 3.22.2 
 
 sense_emu_gui - An emulator for the Raspberry Pi Sense HAT
 Copyright (C) 2016 Raspberry Pi Foundation
 
 This program is free software; you can redistribute it and/or
 modify it under the terms of the GNU General Public License
 as published by the Free Software Foundation; either version 2
@@ -18,15 +18,15 @@
 along with this program; if not, write to the Free Software
 Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 Author: Dave Jones
 
 -->
 <interface domain="sense-emu">
-  <requires lib="gtk+" version="3.8"/>
+  <requires lib="gtk+" version="3.18"/>
   <!-- interface-license-type gplv2 -->
   <!-- interface-name sense_emu_gui -->
   <!-- interface-description An emulator for the Raspberry Pi Sense HAT -->
   <!-- interface-copyright 2016 Raspberry Pi Foundation -->
   <!-- interface-authors Dave Jones -->
   <object class="GtkAdjustment" id="humidity">
     <property name="upper">100</property>
@@ -68,17 +68,22 @@
   <object class="GtkAdjustment" id="yaw">
     <property name="lower">-180</property>
     <property name="upper">180</property>
     <property name="step_increment">1</property>
     <property name="page_increment">15</property>
     <signal name="value-changed" handler="orientation_changed" swapped="no"/>
   </object>
-  <object class="GtkApplicationWindow" id="window">
+  <template class="MainWindow" parent="GtkApplicationWindow">
     <property name="can_focus">False</property>
     <property name="title" translatable="yes">Sense HAT Emulator</property>
+    <signal name="size-allocate" handler="window_resized" swapped="no"/>
+    <signal name="window-state-event" handler="window_state_changed" swapped="no"/>
+    <child type="titlebar">
+      <placeholder/>
+    </child>
     <child>
       <object class="GtkGrid" id="root_grid">
         <property name="visible">True</property>
         <property name="can_focus">False</property>
         <property name="margin_left">6</property>
         <property name="margin_right">6</property>
         <property name="margin_top">6</property>
@@ -615,9 +620,9 @@
             <property name="left_attach">0</property>
             <property name="top_attach">2</property>
             <property name="width">3</property>
           </packing>
         </child>
       </object>
     </child>
-  </object>
+  </template>
 </interface>
```

### Comparing `sense-emu-1.1/sense_emu/common.py` & `sense-emu-1.2.1/sense_emu/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,58 +12,49 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-nstr = str
-str = type('')
-
 import io
 import errno
 from struct import Struct
 from collections import namedtuple
 
 
 # Structures for sense_rec and sense_play
-HEADER_REC = Struct(nstr(
+HEADER_REC = Struct(
     '='  # native order, standard sizing
     '8s' # magic number ("SENSEHAT")
     'b'  # version number (1)
     '7x' # padding
     'd'  # initial timestamp
-    ))
+)
 
-DATA_REC = Struct(nstr(
+DATA_REC = Struct(
     '='   # native order, standard sizing
     'd'   # timestamp
     'dd'  # pressure+temp readings
     'dd'  # humidity+temp readings
     'ddd' # raw accelerometer readings
     'ddd' # raw gyro readings
     'ddd' # raw compass readings
     'ddd' # calculated pose
-    ))
+)
 
 DataRecord = namedtuple('DataRecord', (
     'timestamp',
     'pressure', 'ptemp',
     'humidity', 'htemp',
     'ax', 'ay', 'az',
     'gx', 'gy', 'gz',
     'cx', 'cy', 'cz',
     'ox', 'oy', 'oz',
-    ))
+))
 
 
 def clamp(value, min_value, max_value):
     """
     Return *value* clipped to the range *min_value* to *max_value* inclusive.
     """
     return min(max_value, max(min_value, value))
@@ -71,20 +62,21 @@
 
 def slow_pi():
     """
     Returns ``True`` if the local hardware is a Raspberry Pi with a slow
     processor, specifically a BCM2835. This is used to determine defaults for
     the simulation's processing.
     """
+    # FIXME this won't work with modern kernels that all like the hardware as
+    # BCM2835; use /proc/device-tree/model and parse SoC bits
     try:
         cpu = ''
         with io.open('/proc/cpuinfo', 'r') as f:
             for line in f:
                 if line.startswith('Hardware'):
                     cpu = line.split(':', 1)[1].strip()
                     break
         return cpu in ('BCM2835', 'BCM2708')
     except IOError as e:
         if e.errno == errno.ENOENT:
             return False
         raise
-
```

### Comparing `sense-emu-1.1/sense_emu/terminal.py` & `sense-emu-1.2.1/sense_emu/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,32 +20,24 @@
 Defines base classes for command line utilities.
 
 This module define a TerminalApplication class which provides common facilities
 to command line applications: a help screen, universal file globbing, response
 file handling, and common logging configuration and options.
 """
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-str = type('')
-
 import sys
 import io
 import os
 import argparse
 import textwrap
 import logging
 import locale
 import traceback
+import configparser
 
-from . import configparser
 from .i18n import init_i18n, _
 
 try:
     # Optionally import argcomplete (for auto-completion) if it's installed
     import argcomplete
 except ImportError:
     argcomplete = None
@@ -57,18 +49,17 @@
 init_i18n()
 _CONSOLE = logging.StreamHandler(sys.stderr)
 _CONSOLE.setFormatter(logging.Formatter('%(message)s'))
 _CONSOLE.setLevel(logging.DEBUG)
 logging.getLogger().addHandler(_CONSOLE)
 
 
-class FileType(object):
+class FileType:
     # Variant of argparse.FileType that handles binary stdin/stdout streams
-    # correctly under Python 3, and handles encoded text files correctly under
-    # Python 2
+    # correctly under Python 3
     def __init__(self, mode='r', bufsize=-1, encoding=None, errors=None):
         self._mode = mode
         self._bufsize = bufsize
         self._encoding = encoding
         self._errors = errors
 
     def __call__(self, string):
@@ -100,15 +91,15 @@
         kwargs = [('encoding', self._encoding), ('errors', self._errors)]
         args_str = ', '.join([repr(arg) for arg in args if arg != -1] +
                              ['%s=%r' % (kw, arg) for kw, arg in kwargs
                               if arg is not None])
         return '%s(%s)' % (type(self).__name__, args_str)
 
 
-class TerminalApplication(object):
+class TerminalApplication:
     """
     Base class for command line applications.
 
     This class provides command line parsing, file globbing, response file
     handling and common logging configuration for command line utilities.
     Descendent classes should override the main() method to implement their
     main body, and __init__() if they wish to extend the command line options.
@@ -253,9 +244,7 @@
                 for msg in line.rstrip().split('\n'):
                     logging.critical(msg.replace('%', '%%'))
             return 1
 
     def main(self, args):
         "Called as the main body of the utility"
         raise NotImplementedError
-
-
```

### Comparing `sense-emu-1.1/sense_emu/sense_emu_gui.svg` & `sense-emu-1.2.1/sense_emu/sense_emu_gui.svg`

 * *Files identical despite different names*

### Comparing `sense-emu-1.1/sense_emu/menu.ui` & `sense-emu-1.2.1/sense_emu/menu.ui`

 * *Files identical despite different names*

### Comparing `sense-emu-1.1/sense_emu/gui.py` & `sense-emu-1.2.1/sense_emu/gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,31 +12,22 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-nstr = str
-str = type('')
-
-
 import io
 import os
 import sys
 import atexit
 import struct
 import math
 import errno
+import shlex
 import subprocess
 import webbrowser
 import datetime as dt
 from time import time, sleep
 from threading import Thread, Lock, Event
 
 import gi
@@ -57,28 +48,29 @@
 from .stick import StickServer, SenseStick
 from .lock import EmulatorLock
 from .common import HEADER_REC, DATA_REC, DataRecord, slow_pi
 
 
 def main():
     init_i18n()
-    # threads_init isn't required since PyGObject 3.10.2, but just in case
-    # we're on something ancient...
-    GObject.threads_init()
     app = EmuApplication()
     app.run(sys.argv)
 
 
 def load_image(filename, format='png'):
     loader = GdkPixbuf.PixbufLoader.new_with_type(format)
     loader.write(pkg_resources.resource_string(__name__, filename))
     loader.close()
     return loader.get_pixbuf()
 
 
+def load_ui(filename):
+    return pkg_resources.resource_string(__name__, filename)
+
+
 class EmuApplication(Gtk.Application):
     def __init__(self, *args, **kwargs):
         super(EmuApplication, self).__init__(
                 *args, application_id='org.raspberrypi.sense_emu_gui',
                 flags=Gio.ApplicationFlags.HANDLES_COMMAND_LINE,
                 **kwargs)
         GLib.set_application_name(_('Sense HAT Emulator'))
@@ -117,38 +109,38 @@
         make_action('help',    self.on_help)
         make_action('about',   self.on_about)
         make_action('quit',    self.on_quit)
 
         builder = Gtk.Builder(translation_domain=__project__)
         builder.add_from_string(
             pkg_resources.resource_string(__name__, 'menu.ui').decode('utf-8'))
-        self.props.menubar = builder.get_object('app-menu')
+        self.set_menubar(builder.get_object('app-menu'))
 
         # Construct the open examples sub-menu
         for directory, label in [
                 # I18N: Easy examples
                 ('basic',        _('Simple')),
                 # I18N: Intermediate skill examples
                 ('intermediate', _('Intermediate')),
                 # I18N: Difficult examples
                 ('advanced',     _('Advanced')),
                 ]:
             examples = Gio.Menu.new()
             # NOTE: The use of literal "/" below is correct; resource paths
             # are not file-system paths and always use "/"
-            for example in sorted(
-                    pkg_resources.resource_listdir(__name__, 'examples/%s' % directory)):
+            for example in sorted(pkg_resources.resource_listdir(
+                    __name__, 'examples/{directory}'.format(directory=directory))):
                 if example.endswith('.py'):
                     examples.append(
                         example.replace('_', '__'),
                         Gio.Action.print_detailed_name(
                             'app.example',
-                            GLib.Variant.new_string('%s/%s' % (directory, example))
-                            )
-                        )
+                            GLib.Variant.new_string(
+                                '{directory}/{example}'.format(
+                                    directory=directory, example=example))))
             builder.get_object('example-submenu').append_submenu(label, examples)
 
         # Construct the settings database and tweak initial value of
         # simulate-imu and simulate-env if we're running on a slow Pi, and the
         # user hasn't explicitly set a value yet
         if pkg_resources.resource_exists(__name__, 'gschemas.compiled'):
             source = Gio.SettingsSchemaSource.new_from_directory(
@@ -179,19 +171,19 @@
         if key == 'simulate-env':
             self.pressure.simulate_noise = settings.get_boolean(key)
             self.humidity.simulate_noise = settings.get_boolean(key)
         elif key == 'simulate-imu':
             self.imu.simulate_world = settings.get_boolean(key)
         elif key == 'orientation-scale':
             # Force the orientation sliders to redraw
-            self.window.ui.yaw_scale.queue_draw()
-            self.window.ui.pitch_scale.queue_draw()
-            self.window.ui.roll_scale.queue_draw()
+            self.window.yaw_scale.queue_draw()
+            self.window.pitch_scale.queue_draw()
+            self.window.roll_scale.queue_draw()
         elif key == 'screen-fps':
-            self.window.ui.screen_widget.screen_update_delay = 1 / settings.get_int(key)
+            self.window.screen_widget.screen_update_delay = 1 / settings.get_int(key)
 
     def do_shutdown(self):
         if self.lock.mine:
             self.lock.release()
             if self.window:
                 self.window.destroy()
                 self.window = None
@@ -232,15 +224,16 @@
         else:
             webbrowser.open(remote_help)
 
     def on_about(self, action, param):
         logo = load_image('sense_emu_gui.svg', format='svg')
         about_dialog = Gtk.AboutDialog(
             transient_for=self.window,
-            authors=['%s <%s>' % (__author__, __author_email__)],
+            authors=['{author} <{email}>'.format(author=__author__,
+                                                 email=__author_email__)],
             license_type=Gtk.License.GPL_2_0, logo=logo,
             version=__version__, website=__url__)
         about_dialog.run()
         about_dialog.destroy()
 
     def on_example(self, action, param):
         # NOTE: The use of a bare "/" below is correct: resource paths are
@@ -258,22 +251,20 @@
         # Write a note at the top of the file to explain things
         target.write("""\
 # This file has been written to your home directory for convenience. It is
 # saved as "{filename}"
 
 """.format(filename=filename))
         target.write(source.read().decode('utf-8'))
-        # Spawn IDLE; if this seems like a crazy way to spawn IDLE, you're
-        # right but it's also cross-platform and cross-version compatible
-        # (works on Py 2.x on Windows and UNIX, and Py 3.x on Windows and UNIX;
-        # almost any other variant fails for some combination)
-        subprocess.Popen([
-            sys.executable,
-            '-c', 'from idlelib.PyShell import main; main()',
-            filename])
+        cmd = self.settings.get_string('editor-command')
+        try:
+            cmd % 'foo'
+        except TypeError:
+            cmd = cmd + ' %s'
+        subprocess.Popen(shlex.split(cmd % shlex.quote(filename)))
 
     def on_play(self, action, param):
         open_dialog = Gtk.FileChooserDialog(
             transient_for=self.window,
             title=_('Select the recording to play'),
             action=Gtk.FileChooserAction.OPEN)
         open_dialog.add_button(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL)
@@ -296,32 +287,14 @@
         finally:
             prefs_dialog.destroy()
 
     def on_quit(self, action, param):
         self.quit()
 
 
-class BuilderUi(object):
-    def __init__(self, owner, filename):
-        # Load the GUI definitions (see __getattr__ for how we tie the loaded
-        # objects into instance variables) and connect all handlers to methods
-        # on this object
-        self._builder = Gtk.Builder(translation_domain=__project__)
-        self._builder.add_from_string(
-            pkg_resources.resource_string(__name__, filename).decode('utf-8'))
-        self._builder.connect_signals(owner)
-
-    def __getattr__(self, name):
-        result = self._builder.get_object(name)
-        if result is None:
-            raise AttributeError(_('No such attribute %r') % name)
-        setattr(self, name, result)
-        return result
-
-
 class ScreenWidget(Gtk.DrawingArea):
     __gtype_name__ = 'ScreenWidget'
 
     def __init__(self, *args, **kwargs):
         super(ScreenWidget, self).__init__(*args, **kwargs)
         self.set_has_window(True)
         self.set_size_request(265, 265)
@@ -495,177 +468,201 @@
                         break
 
     def do_destroy(self):
         self._stop.set()
         self._update_thread.join()
 
 
+@Gtk.Template(string=load_ui('main_window.ui'))
 class MainWindow(Gtk.ApplicationWindow):
+    __gtype_name__ = 'MainWindow'
+
+    screen_box = Gtk.Template.Child()
+
+    gyro_grid = Gtk.Template.Child()
+    roll_scale = Gtk.Template.Child()
+    pitch_scale = Gtk.Template.Child()
+    yaw_scale = Gtk.Template.Child()
+    roll = Gtk.Template.Child()
+    pitch = Gtk.Template.Child()
+    yaw = Gtk.Template.Child()
+
+    environ_box = Gtk.Template.Child()
+    humidity = Gtk.Template.Child()
+    pressure = Gtk.Template.Child()
+    temperature = Gtk.Template.Child()
+
+    joystick_box = Gtk.Template.Child()
+    left_button = Gtk.Template.Child()
+    right_button = Gtk.Template.Child()
+    up_button = Gtk.Template.Child()
+    down_button = Gtk.Template.Child()
+    enter_button = Gtk.Template.Child()
+
+    screen_rotate_label = Gtk.Template.Child()
+    screen_rotate_clockwise = Gtk.Template.Child()
+    screen_rotate_anticlockwise = Gtk.Template.Child()
+
+    play_box = Gtk.Template.Child()
+    play_label = Gtk.Template.Child()
+    play_progressbar = Gtk.Template.Child()
+
     def __init__(self, *args, **kwargs):
         super(MainWindow, self).__init__(*args, **kwargs)
 
-        # Build the UI; this is a bit round-about because of Gtk's weird UI
-        # handling. One can't just use a UI file to setup an existing Window
-        # instance (as in Qt); instead one must use a separate handler object
-        # (in which case overriding do_destroy is impossible) or construct a
-        # whole new Window, remove its components, add them to ourselves and
-        # then ditch the Window.
-        self._ui = BuilderUi(self, 'main_window.ui')
-        self.ui.window.remove(self.ui.root_grid)
-        self.add(self.ui.root_grid)
-        self.ui.window.destroy()
-
         # Set the window icon
         icon = load_image('sense_emu_gui.png')
         self.props.icon = icon
 
         # Set up the objects for the playback thread
         self._play_update_lock = Lock()
         self._play_update_id = 0
         self._play_event = Event()
         self._play_thread = None
         self._play_restore = (True, True, True)
 
         # Set up the custom screen widget
-        self.ui.screen_widget = ScreenWidget(visible=True, client=self.props.application.screen)
-        self.ui.screen_box.pack_start(self.ui.screen_widget, True, True, 0)
-        self.ui.screen_widget.show()
+        self.screen_widget = ScreenWidget(visible=True, client=self.props.application.screen)
+        self.screen_box.pack_start(self.screen_widget, True, True, 0)
+        self.screen_widget.show()
 
         # Set initial positions on sliders (and add some marks)
-        self.ui.pitch_scale.add_mark(0, Gtk.PositionType.BOTTOM, None)
-        self.ui.roll_scale.add_mark(0, Gtk.PositionType.BOTTOM, None)
-        self.ui.yaw_scale.add_mark(0, Gtk.PositionType.BOTTOM, None)
-        self.ui.roll.props.value = self.props.application.imu.orientation[0]
-        self.ui.pitch.props.value = self.props.application.imu.orientation[1]
-        self.ui.yaw.props.value = self.props.application.imu.orientation[2]
-        self.ui.humidity.props.value = self.props.application.humidity.humidity
-        self.ui.pressure.props.value = self.props.application.pressure.pressure
-        self.ui.temperature.props.value = self.props.application.humidity.temperature
+        self.pitch_scale.add_mark(0, Gtk.PositionType.BOTTOM, None)
+        self.roll_scale.add_mark(0, Gtk.PositionType.BOTTOM, None)
+        self.yaw_scale.add_mark(0, Gtk.PositionType.BOTTOM, None)
+        self.roll.props.value = self.props.application.imu.orientation[0]
+        self.pitch.props.value = self.props.application.imu.orientation[1]
+        self.yaw.props.value = self.props.application.imu.orientation[2]
+        self.humidity.props.value = self.props.application.humidity.humidity
+        self.pressure.props.value = self.props.application.pressure.pressure
+        self.temperature.props.value = self.props.application.humidity.temperature
 
         # Set up attributes for the joystick buttons
         self._stick_held_lock = Lock()
         self._stick_held_id = 0
-        self.ui.left_button.direction = SenseStick.KEY_LEFT
-        self.ui.right_button.direction = SenseStick.KEY_RIGHT
-        self.ui.up_button.direction = SenseStick.KEY_UP
-        self.ui.down_button.direction = SenseStick.KEY_DOWN
-        self.ui.enter_button.direction = SenseStick.KEY_ENTER
+        self.left_button.direction = SenseStick.KEY_LEFT
+        self.right_button.direction = SenseStick.KEY_RIGHT
+        self.up_button.direction = SenseStick.KEY_UP
+        self.down_button.direction = SenseStick.KEY_DOWN
+        self.enter_button.direction = SenseStick.KEY_ENTER
         self._stick_map = {
-            Gdk.KEY_Return: self.ui.enter_button,
-            Gdk.KEY_Left:   self.ui.left_button,
-            Gdk.KEY_Right:  self.ui.right_button,
-            Gdk.KEY_Up:     self.ui.up_button,
-            Gdk.KEY_Down:   self.ui.down_button,
+            Gdk.KEY_Return: self.enter_button,
+            Gdk.KEY_Left:   self.left_button,
+            Gdk.KEY_Right:  self.right_button,
+            Gdk.KEY_Up:     self.up_button,
+            Gdk.KEY_Down:   self.down_button,
             }
 
         # Set up attributes for the screen rotation controls
-        self.ui.screen_rotate_clockwise.angle = -90
-        self.ui.screen_rotate_anticlockwise.angle = 90
+        self.screen_rotate_clockwise.angle = -90
+        self.screen_rotate_anticlockwise.angle = 90
         self._stick_rotations = {
             SenseStick.KEY_LEFT:  SenseStick.KEY_UP,
             SenseStick.KEY_UP:    SenseStick.KEY_RIGHT,
             SenseStick.KEY_RIGHT: SenseStick.KEY_DOWN,
             SenseStick.KEY_DOWN:  SenseStick.KEY_LEFT,
             SenseStick.KEY_ENTER: SenseStick.KEY_ENTER,
             }
 
-        # Connect some handlers for window size and state
-        self._current_width = -1
-        self._current_height = -1
-        self._is_maximized = False
-        self.connect('size-allocate', self.window_resized)
-        self.connect('window-state-event', self.window_state_changed)
-
+    @Gtk.Template.Callback()
     def window_resized(self, widget, rect):
         if not self.is_maximized():
             self.props.application.settings.set_int('window-width', rect.width)
             self.props.application.settings.set_int('window-height', rect.height)
 
+    @Gtk.Template.Callback()
     def window_state_changed(self, widget, event):
         if event.type == Gdk.EventType.WINDOW_STATE:
             self.props.application.settings.set_boolean(
                 'window-maximized', event.new_window_state & Gdk.WindowState.MAXIMIZED)
         return False
 
-    @property
-    def ui(self):
-        return self._ui
-
     def do_destroy(self):
         try:
             self._play_stop()
         except AttributeError:
             # do_destroy gets called multiple times, and subsequent times lacks
             # the Python-added instance attributes
             pass
         Gtk.ApplicationWindow.do_destroy(self)
 
+    @Gtk.Template.Callback()
     def format_pressure(self, scale, value):
         return '%.1fmbar' % value
 
+    @Gtk.Template.Callback()
     def pressure_changed(self, adjustment):
         if not self._play_thread:
             self.props.application.pressure.set_values(
-                self.ui.pressure.props.value,
-                self.ui.temperature.props.value,
+                self.pressure.props.value,
+                self.temperature.props.value,
                 )
 
+    @Gtk.Template.Callback()
     def format_humidity(self, scale, value):
         return '%.1f%%' % value
 
+    @Gtk.Template.Callback()
     def humidity_changed(self, adjustment):
         if not self._play_thread:
             self.props.application.humidity.set_values(
-                self.ui.humidity.props.value,
-                self.ui.temperature.props.value,
+                self.humidity.props.value,
+                self.temperature.props.value,
                 )
 
+    @Gtk.Template.Callback()
     def format_temperature(self, scale, value):
         return '%.1f°C' % value
 
+    @Gtk.Template.Callback()
     def temperature_changed(self, adjustment):
         if not self._play_thread:
             self.pressure_changed(adjustment)
             self.humidity_changed(adjustment)
 
+    @Gtk.Template.Callback()
     def format_orientation(self, scale, value):
         mode = self.props.application.settings.get_string('orientation-scale')
         return '%.1f°' % (
             value       if mode == 'balance' else
             value + 180 if mode == 'circle' else
             value % 360 if mode == 'modulo' else
             999 # should never happen
             )
 
+    @Gtk.Template.Callback()
     def orientation_changed(self, adjustment):
         if not self._play_thread:
             self.props.application.imu.set_orientation((
-                self.ui.roll.props.value,
-                self.ui.pitch.props.value,
-                self.ui.yaw.props.value,
+                self.roll.props.value,
+                self.pitch.props.value,
+                self.yaw.props.value,
                 ))
 
+    @Gtk.Template.Callback()
     def stick_key_pressed(self, button, event):
         try:
             button = self._stick_map[event.keyval]
         except KeyError:
             return False
         else:
             self.stick_pressed(button, event)
             return True
 
+    @Gtk.Template.Callback()
     def stick_key_released(self, button, event):
         try:
             button = self._stick_map[event.keyval]
         except KeyError:
             return False
         else:
             self.stick_released(button, event)
             return True
 
+    @Gtk.Template.Callback()
     def stick_pressed(self, button, event):
         # When a button is double-clicked, GTK fires two pressed events for the
         # second click with no intervening released event (so there's one
         # pressed event for the first click, followed by a released event, then
         # two pressed events for the second click followed by a single released
         # event). This isn't documented, so it could be a bug, but it seems
         # more like a deliberate behaviour. Anyway, we work around the
@@ -676,14 +673,15 @@
             if self._stick_held_id:
                 return True
             self._stick_held_id = GLib.timeout_add(250, self.stick_held_first, button)
         self._stick_send(button.direction, SenseStick.STATE_PRESS)
         button.set_active(True)
         return True
 
+    @Gtk.Template.Callback()
     def stick_released(self, button, event):
         with self._stick_held_lock:
             if self._stick_held_id:
                 GLib.source_remove(self._stick_held_id)
                 self._stick_held_id = 0
         self._stick_send(button.direction, SenseStick.STATE_RELEASE)
         button.set_active(False)
@@ -698,28 +696,30 @@
     def stick_held(self, button):
         self._stick_send(button.direction, SenseStick.STATE_HOLD)
         return True
 
     def _stick_send(self, direction, action):
         tv_usec, tv_sec = math.modf(time())
         tv_usec *= 1000000
-        r = self.ui.screen_widget.props.rotation // 90
+        r = self.screen_widget.props.rotation // 90
         while r:
             direction = self._stick_rotations[direction]
             r -= 1
         event_rec = struct.pack(SenseStick.EVENT_FORMAT,
             int(tv_sec), int(tv_usec), SenseStick.EV_KEY, direction, action)
         self.props.application.stick.send(event_rec)
 
+    @Gtk.Template.Callback()
     def rotate_screen(self, button):
-        self.ui.screen_widget.props.rotation = (self.ui.screen_widget.props.rotation + button.angle) % 360
-        self.ui.screen_rotate_label.props.label = '%d°' % self.ui.screen_widget.props.rotation
+        self.screen_widget.props.rotation = (self.screen_widget.props.rotation + button.angle) % 360
+        self.screen_rotate_label.props.label = '%d°' % self.screen_widget.props.rotation
 
+    @Gtk.Template.Callback()
     def toggle_orientation(self, button):
-        self.ui.screen_widget.props.orientation = not self.ui.screen_widget.props.orientation
+        self.screen_widget.props.orientation = not self.screen_widget.props.orientation
 
     def _play_run(self, f):
         err = None
         try:
             # Calculate how many records are in the file; we'll use this later
             # when updating the progress bar
             rec_total = (f.seek(0, io.SEEK_END) - HEADER_REC.size) // DATA_REC.size
@@ -760,26 +760,27 @@
             # Get the main thread to re-enable the controls at the end of
             # playback
             GLib.idle_add(self._play_controls_finish, err)
 
     def _play_update_controls(self, fraction):
         with self._play_update_lock:
             self._play_update_id = 0
-        self.ui.play_progressbar.props.fraction = fraction
+        self.play_progressbar.props.fraction = fraction
         if not math.isnan(self.props.application.humidity.temperature):
-            self.ui.temperature.props.value = self.props.application.humidity.temperature
+            self.temperature.props.value = self.props.application.humidity.temperature
         if not math.isnan(self.props.application.pressure.pressure):
-            self.ui.pressure.props.value = self.props.application.pressure.pressure
+            self.pressure.props.value = self.props.application.pressure.pressure
         if not math.isnan(self.props.application.humidity.humidity):
-            self.ui.humidity.props.value = self.props.application.humidity.humidity
-        self.ui.yaw.props.value = math.degrees(self.props.application.imu.orientation[2])
-        self.ui.pitch.props.value = math.degrees(self.props.application.imu.orientation[1])
-        self.ui.roll.props.value = math.degrees(self.props.application.imu.orientation[0])
+            self.humidity.props.value = self.props.application.humidity.humidity
+        self.yaw.props.value = math.degrees(self.props.application.imu.orientation[2])
+        self.pitch.props.value = math.degrees(self.props.application.imu.orientation[1])
+        self.roll.props.value = math.degrees(self.props.application.imu.orientation[0])
         return False
 
+    @Gtk.Template.Callback()
     def play_stop_clicked(self, button):
         self._play_stop()
 
     def _play_stop(self):
         if self._play_thread:
             self._play_event.set()
             self._play_thread.join()
@@ -800,40 +801,40 @@
                 raise IOError(_('Incomplete data record at end of %s') % f.name)
             else:
                 data = DataRecord(*DATA_REC.unpack(buf))
                 yield data._replace(timestamp=data.timestamp + offset)
 
     def _play_controls_setup(self, filename):
         # Disable all the associated user controls while playing back
-        self.ui.environ_box.props.sensitive = False
-        self.ui.gyro_grid.props.sensitive = False
+        self.environ_box.props.sensitive = False
+        self.gyro_grid.props.sensitive = False
         # Disable simulation threads as we're going to manipulate the
         # values precisely
         self._play_restore = (
             self.props.application.pressure.simulate_noise,
             self.props.application.humidity.simulate_noise,
             self.props.application.imu.simulate_world,
             )
         self.props.application.pressure.simulate_noise = False
         self.props.application.humidity.simulate_noise = False
         self.props.application.imu.simulate_world = False
         # Show the playback bar
-        self.ui.play_label.props.label = _('Playing %s') % os.path.basename(filename)
-        self.ui.play_progressbar.props.fraction = 0.0
-        self.ui.play_box.props.visible = True
+        self.play_label.props.label = _('Playing %s') % os.path.basename(filename)
+        self.play_progressbar.props.fraction = 0.0
+        self.play_box.props.visible = True
 
     def _play_controls_finish(self, exc):
         # Reverse _play_controls_setup
-        self.ui.play_box.props.visible = False
+        self.play_box.props.visible = False
         ( self.props.application.pressure.simulate_noise,
             self.props.application.humidity.simulate_noise,
             self.props.application.imu.simulate_world,
             ) = self._play_restore
-        self.ui.environ_box.props.sensitive = True
-        self.ui.gyro_grid.props.sensitive = True
+        self.environ_box.props.sensitive = True
+        self.gyro_grid.props.sensitive = True
         self._play_thread = None
         # If an exception occurred in the background thread, display the
         # error in an appropriate dialog
         if exc:
             dialog = Gtk.MessageDialog(
                 transient_for=self,
                 message_type=Gtk.MessageType.ERROR,
@@ -848,45 +849,49 @@
         self._play_stop()
         self._play_controls_setup(filename)
         self._play_thread = Thread(target=self._play_run, args=(io.open(filename, 'rb'),))
         self._play_event.clear()
         self._play_thread.start()
 
 
+@Gtk.Template(string=load_ui('prefs_dialog.ui'))
 class PrefsDialog(Gtk.Dialog):
+    __gtype_name__ = 'PrefsDialog'
+
+    close_button = Gtk.Template.Child()
+
+    env_check = Gtk.Template.Child()
+    imu_check = Gtk.Template.Child()
+    screen_fps = Gtk.Template.Child()
+    editor_entry = Gtk.Template.Child()
+
+    orientation_balance = Gtk.Template.Child()
+    orientation_circle = Gtk.Template.Child()
+    orientation_modulo = Gtk.Template.Child()
+
     def __init__(self, *args, **kwargs):
         self.settings = kwargs.pop('settings')
         super(PrefsDialog, self).__init__(*args, **kwargs)
 
-        # See comments in MainWindow...
-        self._ui = BuilderUi(self, 'prefs_dialog.ui')
-        self.ui.window.remove(self.ui.dialog_vbox)
-        self.remove(self.get_content_area())
-        self.add(self.ui.dialog_vbox)
-        self.ui.window.destroy()
-
-        self.props.resizable = False
-        self.ui.close_button.grab_default()
         self.settings.bind(
-            'simulate-env', self.ui.env_check, 'active', Gio.SettingsBindFlags.DEFAULT)
+            'simulate-env', self.env_check, 'active', Gio.SettingsBindFlags.DEFAULT)
+        self.settings.bind(
+            'simulate-imu', self.imu_check, 'active', Gio.SettingsBindFlags.DEFAULT)
         self.settings.bind(
-            'simulate-imu', self.ui.imu_check, 'active', Gio.SettingsBindFlags.DEFAULT)
+            'screen-fps', self.screen_fps, 'value', Gio.SettingsBindFlags.DEFAULT)
         self.settings.bind(
-            'screen-fps', self.ui.screen_fps, 'value', Gio.SettingsBindFlags.DEFAULT)
-        self.ui.orientation_balance.value = 'balance'
-        self.ui.orientation_circle.value = 'circle'
-        self.ui.orientation_modulo.value = 'modulo'
+            'editor-command', self.editor_entry, 'text', Gio.SettingsBindFlags.DEFAULT)
+        self.orientation_balance.value = 'balance'
+        self.orientation_circle.value = 'circle'
+        self.orientation_modulo.value = 'modulo'
         s = self.settings.get_string('orientation-scale')
-        for c in self.ui.orientation_balance.get_group():
+        for c in self.orientation_balance.get_group():
             c.props.active = (c.value == s)
 
-    @property
-    def ui(self):
-        return self._ui
-
+    @Gtk.Template.Callback()
     def close_clicked(self, button):
         self.response(Gtk.ResponseType.ACCEPT)
 
+    @Gtk.Template.Callback()
     def orientation_changed(self, button):
         if button.props.active:
             self.settings.set_string('orientation-scale', button.value)
-
```

### Comparing `sense-emu-1.1/sense_emu/sense_hat_text.png` & `sense-emu-1.2.1/sense_emu/sense_hat_text.png`

 * *Files 17% similar despite different names*

#### sng

```diff
@@ -1,21 +1,21 @@
 #SNG: from stdin
 IHDR {
     width: 8; height: 640; bitdepth: 8;
     using color;
 }
 pHYs {xpixels: 2835; ypixels: 2835; per: meter;}  # (72 dpi)
 tIME {
-    # 18 Feb 2015 13:41:13 GMT
-    year:   2015
-    month:  2
-    day:    18
-    hour:   13
-    minute: 41
-    second: 13
+    #  2 Sep 2021 23:36:05 GMT
+    year:   2021
+    month:  9
+    day:    2
+    hour:   23
+    minute: 36
+    second: 5
 }
 tEXt {
     keyword: "Comment";
     text: "Created with GIMP";
 }
 IMAGE {
     pixels hex
```

### Comparing `sense-emu-1.1/sense_emu/i18n.py` & `sense-emu-1.2.1/sense_emu/i18n.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,22 +12,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>
 
-from __future__ import (
-    unicode_literals,
-    absolute_import,
-    print_function,
-    division,
-    )
-str = type('')
-
 import sys
 import locale
 import gettext as _gettext
 import atexit
 
 import pkg_resources
 
@@ -70,15 +62,10 @@
                 # to do here yet
                 return
         # Finally, set translation domain for Python's built-in gettext
         _gettext.bindtextdomain(__project__, localedir)
         _gettext.textdomain(__project__)
 
 
-if sys.version_info.major == 3:
-    gettext = _gettext.gettext
-    ngettext = _gettext.ngettext
-else:
-    gettext = lambda message: _gettext.gettext(message).decode('utf-8')
-    ngettext = lambda singular, plural, n: _gettext.ngettext(singular, plural, n).decode('utf-8')
+gettext = _gettext.gettext
+ngettext = _gettext.ngettext
 _ = gettext
-
```

### Comparing `sense-emu-1.1/sense_emu/examples/intermediate/bar_graph.py` & `sense-emu-1.2.1/sense_emu/examples/intermediate/bar_graph.py`

 * *Files identical despite different names*

### Comparing `sense-emu-1.1/sense_emu/examples/intermediate/rainbow.py` & `sense-emu-1.2.1/sense_emu/examples/intermediate/rainbow.py`

 * *Files identical despite different names*

### Comparing `sense-emu-1.1/sense_emu/examples/intermediate/joystick_loop.py` & `sense-emu-1.2.1/sense_emu/examples/intermediate/joystick_loop.py`

 * *Files identical despite different names*

### Comparing `sense-emu-1.1/sense_emu/examples/intermediate/plumb_line.py` & `sense-emu-1.2.1/sense_emu/examples/intermediate/plumb_line.py`

 * *Files identical despite different names*

### Comparing `sense-emu-1.1/sense_emu/examples/intermediate/line_graph.py` & `sense-emu-1.2.1/sense_emu/examples/intermediate/line_graph.py`

 * *Files identical despite different names*

### Comparing `sense-emu-1.1/sense_emu/examples/advanced/joystick_events.py` & `sense-emu-1.2.1/sense_emu/examples/advanced/joystick_events.py`

 * *Files identical despite different names*

### Comparing `sense-emu-1.1/sense_emu/examples/advanced/sensor_menu.py` & `sense-emu-1.2.1/sense_emu/examples/advanced/sensor_menu.py`

 * *Files identical despite different names*

### Comparing `sense-emu-1.1/LICENSE.txt` & `sense-emu-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

