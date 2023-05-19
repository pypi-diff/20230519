# Comparing `tmp/Chill-Streams-0.3.2.tar.gz` & `tmp/Chill-Streams-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chill-Streams-0.3.2.tar", last modified: Fri Jan  6 17:17:55 2023, max compression
+gzip compressed data, was "Chill-Streams-0.4.0.tar", last modified: Fri May 19 17:00:30 2023, max compression
```

## Comparing `Chill-Streams-0.3.2.tar` & `Chill-Streams-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-01-06 17:17:55.389504 Chill-Streams-0.3.2/
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-01-06 17:17:55.385989 Chill-Streams-0.3.2/Chill_Streams.egg-info/
--rw-r--r--   0 zach       (502) staff       (20)     4892 2023-01-06 17:17:55.000000 Chill-Streams-0.3.2/Chill_Streams.egg-info/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     1027 2023-01-06 17:17:55.000000 Chill-Streams-0.3.2/Chill_Streams.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2023-01-06 17:17:55.000000 Chill-Streams-0.3.2/Chill_Streams.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (502) staff       (20)       88 2023-01-06 17:17:55.000000 Chill-Streams-0.3.2/Chill_Streams.egg-info/entry_points.txt
--rw-r--r--   0 zach       (502) staff       (20)      111 2023-01-06 17:17:55.000000 Chill-Streams-0.3.2/Chill_Streams.egg-info/requires.txt
--rw-r--r--   0 zach       (502) staff       (20)       14 2023-01-06 17:17:55.000000 Chill-Streams-0.3.2/Chill_Streams.egg-info/top_level.txt
--rw-r--r--   0 zach       (502) staff       (20)     1065 2021-07-09 18:54:48.000000 Chill-Streams-0.3.2/LICENSE
--rw-r--r--   0 zach       (502) staff       (20)     4892 2023-01-06 17:17:55.389562 Chill-Streams-0.3.2/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     4563 2022-12-03 03:18:33.000000 Chill-Streams-0.3.2/README.md
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-01-06 17:17:55.388241 Chill-Streams-0.3.2/chill_streams/
--rw-r--r--   0 zach       (502) staff       (20)      407 2023-01-06 17:11:07.000000 Chill-Streams-0.3.2/chill_streams/__about__.py
--rw-r--r--   0 zach       (502) staff       (20)       75 2021-07-16 14:56:57.000000 Chill-Streams-0.3.2/chill_streams/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     4377 2022-05-03 18:35:47.000000 Chill-Streams-0.3.2/chill_streams/app.py
--rw-r--r--   0 zach       (502) staff       (20)      728 2022-05-03 18:33:55.000000 Chill-Streams-0.3.2/chill_streams/ascii_art.py
--rw-r--r--   0 zach       (502) staff       (20)      365 2022-05-03 18:33:55.000000 Chill-Streams-0.3.2/chill_streams/cli.py
--rw-r--r--   0 zach       (502) staff       (20)     1105 2022-05-03 18:34:50.000000 Chill-Streams-0.3.2/chill_streams/cmd.py
--rw-r--r--   0 zach       (502) staff       (20)     1331 2022-01-04 21:20:39.000000 Chill-Streams-0.3.2/chill_streams/config.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-01-06 17:17:55.389373 Chill-Streams-0.3.2/chill_streams/data/
--rw-r--r--   0 zach       (502) staff       (20)        0 2021-07-09 18:54:48.000000 Chill-Streams-0.3.2/chill_streams/data/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)       59 2022-05-03 18:33:55.000000 Chill-Streams-0.3.2/chill_streams/data/https.txt
--rw-r--r--   0 zach       (502) staff       (20)     8270 2022-11-17 23:43:08.000000 Chill-Streams-0.3.2/chill_streams/data/stations.csv
--rw-r--r--   0 zach       (502) staff       (20)        0 2022-11-17 23:43:08.000000 Chill-Streams-0.3.2/chill_streams/data/videostreams.csv
--rwxr-xr-x   0 zach       (502) staff       (20)     2064 2023-01-06 17:08:51.000000 Chill-Streams-0.3.2/chill_streams/data/vlc-radio-template.sh
--rw-r--r--   0 zach       (502) staff       (20)      839 2022-05-03 18:26:46.000000 Chill-Streams-0.3.2/chill_streams/logging.py
--rw-r--r--   0 zach       (502) staff       (20)      161 2023-01-06 17:08:27.000000 Chill-Streams-0.3.2/chill_streams/pkg_resources.py
--rw-r--r--   0 zach       (502) staff       (20)      912 2021-07-12 23:44:06.000000 Chill-Streams-0.3.2/chill_streams/script_path.py
--rw-r--r--   0 zach       (502) staff       (20)     2545 2022-05-03 18:33:55.000000 Chill-Streams-0.3.2/chill_streams/shell_script.py
--rw-r--r--   0 zach       (502) staff       (20)     5896 2022-05-03 18:33:55.000000 Chill-Streams-0.3.2/chill_streams/station_list.py
--rw-r--r--   0 zach       (502) staff       (20)     1893 2022-05-03 18:33:55.000000 Chill-Streams-0.3.2/chill_streams/url.py
--rw-r--r--   0 zach       (502) staff       (20)      288 2022-05-03 18:33:55.000000 Chill-Streams-0.3.2/chill_streams/version.py
--rw-r--r--   0 zach       (502) staff       (20)     1487 2022-05-03 18:33:55.000000 Chill-Streams-0.3.2/chill_streams/video_streams.py
--rw-r--r--   0 zach       (502) staff       (20)     3283 2022-05-03 18:35:20.000000 Chill-Streams-0.3.2/chill_streams/vlc.py
--rw-r--r--   0 zach       (502) staff       (20)      154 2023-01-06 17:17:55.389757 Chill-Streams-0.3.2/setup.cfg
--rw-r--r--   0 zach       (502) staff       (20)     1126 2022-11-17 23:43:08.000000 Chill-Streams-0.3.2/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-05-19 17:00:30.405335 Chill-Streams-0.4.0/
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-05-19 17:00:30.402804 Chill-Streams-0.4.0/Chill_Streams.egg-info/
+-rw-r--r--   0 zach       (502) staff       (20)     4892 2023-05-19 17:00:30.000000 Chill-Streams-0.4.0/Chill_Streams.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)      839 2023-05-19 17:00:30.000000 Chill-Streams-0.4.0/Chill_Streams.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2023-05-19 17:00:30.000000 Chill-Streams-0.4.0/Chill_Streams.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (502) staff       (20)       88 2023-05-19 17:00:30.000000 Chill-Streams-0.4.0/Chill_Streams.egg-info/entry_points.txt
+-rw-r--r--   0 zach       (502) staff       (20)      111 2023-05-19 17:00:30.000000 Chill-Streams-0.4.0/Chill_Streams.egg-info/requires.txt
+-rw-r--r--   0 zach       (502) staff       (20)       14 2023-05-19 17:00:30.000000 Chill-Streams-0.4.0/Chill_Streams.egg-info/top_level.txt
+-rw-r--r--   0 zach       (502) staff       (20)     1065 2021-07-09 18:54:48.000000 Chill-Streams-0.4.0/LICENSE
+-rw-r--r--   0 zach       (502) staff       (20)     4892 2023-05-19 17:00:30.405382 Chill-Streams-0.4.0/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     4563 2022-12-03 03:18:33.000000 Chill-Streams-0.4.0/README.md
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-05-19 17:00:30.404706 Chill-Streams-0.4.0/chill_streams/
+-rw-r--r--   0 zach       (502) staff       (20)      407 2023-05-19 16:58:06.000000 Chill-Streams-0.4.0/chill_streams/__about__.py
+-rw-r--r--   0 zach       (502) staff       (20)       75 2021-07-16 14:56:57.000000 Chill-Streams-0.4.0/chill_streams/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     4902 2023-05-19 16:24:59.000000 Chill-Streams-0.4.0/chill_streams/app.py
+-rw-r--r--   0 zach       (502) staff       (20)      728 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/ascii_art.py
+-rw-r--r--   0 zach       (502) staff       (20)      365 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/cli.py
+-rw-r--r--   0 zach       (502) staff       (20)     1105 2022-05-03 18:34:50.000000 Chill-Streams-0.4.0/chill_streams/cmd.py
+-rw-r--r--   0 zach       (502) staff       (20)     1331 2022-01-04 21:20:39.000000 Chill-Streams-0.4.0/chill_streams/config.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-05-19 17:00:30.405233 Chill-Streams-0.4.0/chill_streams/data/
+-rw-r--r--   0 zach       (502) staff       (20)        0 2021-07-09 18:54:48.000000 Chill-Streams-0.4.0/chill_streams/data/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)       59 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/data/https.txt
+-rw-r--r--   0 zach       (502) staff       (20)     8270 2022-11-17 23:43:08.000000 Chill-Streams-0.4.0/chill_streams/data/stations.csv
+-rw-r--r--   0 zach       (502) staff       (20)        0 2022-11-17 23:43:08.000000 Chill-Streams-0.4.0/chill_streams/data/videostreams.csv
+-rwxr-xr-x   0 zach       (502) staff       (20)     2064 2023-01-06 17:08:51.000000 Chill-Streams-0.4.0/chill_streams/data/vlc-radio-template.sh
+-rw-r--r--   0 zach       (502) staff       (20)      839 2022-05-03 18:26:46.000000 Chill-Streams-0.4.0/chill_streams/logging.py
+-rw-r--r--   0 zach       (502) staff       (20)      161 2023-01-06 17:08:27.000000 Chill-Streams-0.4.0/chill_streams/pkg_resources.py
+-rw-r--r--   0 zach       (502) staff       (20)      912 2021-07-12 23:44:06.000000 Chill-Streams-0.4.0/chill_streams/script_path.py
+-rw-r--r--   0 zach       (502) staff       (20)     2545 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/shell_script.py
+-rw-r--r--   0 zach       (502) staff       (20)     5896 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/station_list.py
+-rw-r--r--   0 zach       (502) staff       (20)     1893 2023-05-19 16:03:26.000000 Chill-Streams-0.4.0/chill_streams/url.py
+-rw-r--r--   0 zach       (502) staff       (20)      288 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/version.py
+-rw-r--r--   0 zach       (502) staff       (20)     1487 2022-05-03 18:33:55.000000 Chill-Streams-0.4.0/chill_streams/video_streams.py
+-rw-r--r--   0 zach       (502) staff       (20)     3283 2022-05-03 18:35:20.000000 Chill-Streams-0.4.0/chill_streams/vlc.py
+-rw-r--r--   0 zach       (502) staff       (20)      154 2023-05-19 17:00:30.405550 Chill-Streams-0.4.0/setup.cfg
+-rw-r--r--   0 zach       (502) staff       (20)     1126 2022-11-17 23:43:08.000000 Chill-Streams-0.4.0/setup.py
```

### Comparing `Chill-Streams-0.3.2/Chill_Streams.egg-info/PKG-INFO` & `Chill-Streams-0.4.0/Chill_Streams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chill-Streams
-Version: 0.3.2
+Version: 0.4.0
 Summary: Chill electronica streaming
 Home-page: https://github.com/zcutlip/chill_streams
 Author: Zachary Cutlip
 Author-email: uid000@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `Chill-Streams-0.3.2/Chill_Streams.egg-info/SOURCES.txt` & `Chill-Streams-0.4.0/Chill_Streams.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -20,17 +20,12 @@
 chill_streams/script_path.py
 chill_streams/shell_script.py
 chill_streams/station_list.py
 chill_streams/url.py
 chill_streams/version.py
 chill_streams/video_streams.py
 chill_streams/vlc.py
-chill_streams.egg-info/PKG-INFO
-chill_streams.egg-info/SOURCES.txt
-chill_streams.egg-info/dependency_links.txt
-chill_streams.egg-info/entry_points.txt
-chill_streams.egg-info/top_level.txt
 chill_streams/data/__init__.py
 chill_streams/data/https.txt
 chill_streams/data/stations.csv
 chill_streams/data/videostreams.csv
 chill_streams/data/vlc-radio-template.sh
```

### Comparing `Chill-Streams-0.3.2/LICENSE` & `Chill-Streams-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/PKG-INFO` & `Chill-Streams-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chill-Streams
-Version: 0.3.2
+Version: 0.4.0
 Summary: Chill electronica streaming
 Home-page: https://github.com/zcutlip/chill_streams
 Author: Zachary Cutlip
 Author-email: uid000@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `Chill-Streams-0.3.2/README.md` & `Chill-Streams-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/chill_streams/app.py` & `Chill-Streams-0.4.0/chill_streams/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #!/usr/bin/env python
 '''Play internet radio selection in VLC media player.
 Shift + M --> meta-info; q --> quit'''
 
 import argparse
 import sys
-
-from . import logging
-
 from argparse import ArgumentParser
+from typing import Optional
 
-
+from . import logging
 from .ascii_art import get_ascii_art
 from .shell_script import VLCShellScript, VLCShellScriptException
 from .station_list import StationEntry, StationList
 from .version import CSAbout
-from .video_streams import VideoStreamList, VideoStreamDependencyException
+from .video_streams import VideoStreamDependencyException, VideoStreamList
 from .vlc import VLC
 
 
 def vlc_parse_args():
     parser = ArgumentParser(description=str(CSAbout()))
     parser.add_argument(
         "station",
@@ -57,36 +55,39 @@
         help=argparse.SUPPRESS,
         action='version',
         version=CSAbout().version
     )
     parser.add_argument(
         "--debug", help="Enable debug logging", action='store_true')
 
+    parser.add_argument(
+        "--print-url", "-U", help="Print station URL to console and exit", action="store_true")
+
     parsed = parser.parse_args()
     return parsed
 
 
 def station_selection(options):
     print(get_ascii_art())  # get color-schemed ASCII art heading
     '''Play selected internet radio station.'''
     station_text = ""
     station_num = -1
+    ret = -1
     if options.station:
         try:
             station_num = int(options.station)
         except ValueError:
             station_text = options.station
-
     go_again = True
     while go_again:
         go_again = False
         station_list = StationList(
             substring=station_text, first_match=options.first_match)
-        video_list = {}
-        entry: StationEntry = None
+        video_list: Optional[VideoStreamList] = None
+        entry: Optional[StationEntry] = None
         if station_list.match:
             entry = station_list.match
         elif station_list.has_station_num(station_num):
             entry = station_list[station_num]
         else:
             idx = station_list.last_idx + 1
             try:
@@ -98,38 +99,46 @@
                     entry = video_list[station_num]
                 else:
                     entry = video_list.match
             except VideoStreamDependencyException:
                 pass
 
         if not entry:
-            all_stations = dict(station_list)
-            all_stations.update(video_list)
-
             station_list.print_menu()
+            all_stations = dict(station_list)
             if video_list:
+                all_stations.update(video_list)
                 video_list.print_menu()
             inp = input('Enter item number [\'q\' to quit]: ')
             if inp in ['Q', 'q']:
                 return 0
             station_num = int(inp)
             entry = all_stations[station_num]
 
         station_text = ""
         station_num = -1
 
         curses = not options.gui
 
-        vlc = VLC(entry, ncurses=curses)
-        _, ret = vlc.run()
-        if ret != 0:
-            print(f"Failed to run {vlc.location}", file=sys.stderr)
-            break
-        if options.loop:
-            go_again = True
+        if entry:
+            if options.print_url:
+                ret = 0
+                print("")
+                print(f"{entry.ansi_colorized()}:\n    {entry.url}")
+                print("")
+            else:
+                vlc = VLC(entry, ncurses=curses)
+                _, ret = vlc.run()
+                if ret != 0:
+                    print(f"Failed to run {vlc.location}", file=sys.stderr)
+                    break
+                if options.loop:
+                    go_again = True
+        else:
+            print("Station not found")
 
     return ret
 
 
 def vlc_main():
     options = vlc_parse_args()
     if options.debug:
```

### Comparing `Chill-Streams-0.3.2/chill_streams/ascii_art.py` & `Chill-Streams-0.4.0/chill_streams/ascii_art.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/chill_streams/cmd.py` & `Chill-Streams-0.4.0/chill_streams/cmd.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/chill_streams/config.py` & `Chill-Streams-0.4.0/chill_streams/config.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/chill_streams/data/stations.csv` & `Chill-Streams-0.4.0/chill_streams/data/stations.csv`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/chill_streams/data/vlc-radio-template.sh` & `Chill-Streams-0.4.0/chill_streams/data/vlc-radio-template.sh`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/chill_streams/logging.py` & `Chill-Streams-0.4.0/chill_streams/logging.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/chill_streams/script_path.py` & `Chill-Streams-0.4.0/chill_streams/script_path.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/chill_streams/shell_script.py` & `Chill-Streams-0.4.0/chill_streams/shell_script.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/chill_streams/station_list.py` & `Chill-Streams-0.4.0/chill_streams/station_list.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/chill_streams/url.py` & `Chill-Streams-0.4.0/chill_streams/url.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/chill_streams/video_streams.py` & `Chill-Streams-0.4.0/chill_streams/video_streams.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/chill_streams/vlc.py` & `Chill-Streams-0.4.0/chill_streams/vlc.py`

 * *Files identical despite different names*

### Comparing `Chill-Streams-0.3.2/setup.py` & `Chill-Streams-0.4.0/setup.py`

 * *Files identical despite different names*

