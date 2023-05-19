# Comparing `tmp/mid_to_gcode-0.0.0a1.tar.gz` & `tmp/mid_to_gcode-0.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mid_to_gcode-0.0.0a1.tar", last modified: Wed May 17 18:36:51 2023, max compression
+gzip compressed data, was "mid_to_gcode-0.0.0a2.tar", last modified: Fri May 19 16:12:55 2023, max compression
```

## Comparing `mid_to_gcode-0.0.0a1.tar` & `mid_to_gcode-0.0.0a2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-05-17 18:36:51.004418 mid_to_gcode-0.0.0a1/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      677 2023-05-17 18:18:12.000000 mid_to_gcode-0.0.0a1/LICENSE
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      838 2023-05-17 18:36:51.004418 mid_to_gcode-0.0.0a1/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)        0 2023-05-17 15:30:19.000000 mid_to_gcode-0.0.0a1/README.rst
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-05-17 18:36:51.003419 mid_to_gcode-0.0.0a1/mid_to_gcode/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)       35 2023-05-17 15:37:10.000000 mid_to_gcode-0.0.0a1/mid_to_gcode/__init__.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1726 2023-05-17 18:17:01.000000 mid_to_gcode-0.0.0a1/mid_to_gcode/functions.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      466 2023-05-17 18:05:51.000000 mid_to_gcode-0.0.0a1/mid_to_gcode/mid_to_gcod.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      942 2023-05-17 18:35:37.000000 mid_to_gcode-0.0.0a1/mid_to_gcode/support_functions.py
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-05-17 18:36:51.004418 mid_to_gcode-0.0.0a1/mid_to_gcode.egg-info/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      838 2023-05-17 18:36:50.000000 mid_to_gcode-0.0.0a1/mid_to_gcode.egg-info/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      299 2023-05-17 18:36:50.000000 mid_to_gcode-0.0.0a1/mid_to_gcode.egg-info/SOURCES.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)        1 2023-05-17 18:36:50.000000 mid_to_gcode-0.0.0a1/mid_to_gcode.egg-info/dependency_links.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)       13 2023-05-17 18:36:50.000000 mid_to_gcode-0.0.0a1/mid_to_gcode.egg-info/top_level.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      669 2023-05-17 18:36:23.000000 mid_to_gcode-0.0.0a1/pyproject.toml
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)       38 2023-05-17 18:36:51.004418 mid_to_gcode-0.0.0a1/setup.cfg
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1332 2023-05-17 18:22:46.000000 mid_to_gcode-0.0.0a1/setup.py
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-05-19 16:12:55.253206 mid_to_gcode-0.0.0a2/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      677 2023-05-17 18:18:12.000000 mid_to_gcode-0.0.0a2/LICENSE
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1614 2023-05-19 16:12:55.253206 mid_to_gcode-0.0.0a2/PKG-INFO
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      774 2023-05-17 18:52:47.000000 mid_to_gcode-0.0.0a2/README.rst
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-05-19 16:12:55.253206 mid_to_gcode-0.0.0a2/mid_to_gcode/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)       35 2023-05-17 15:37:10.000000 mid_to_gcode-0.0.0a2/mid_to_gcode/__init__.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1529 2023-05-19 16:09:49.000000 mid_to_gcode-0.0.0a2/mid_to_gcode/functions.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      468 2023-05-18 16:23:27.000000 mid_to_gcode-0.0.0a2/mid_to_gcode/mid_to_gcod.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1615 2023-05-19 16:09:33.000000 mid_to_gcode-0.0.0a2/mid_to_gcode/support_functions.py
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-05-19 16:12:55.253206 mid_to_gcode-0.0.0a2/mid_to_gcode.egg-info/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1614 2023-05-19 16:12:55.000000 mid_to_gcode-0.0.0a2/mid_to_gcode.egg-info/PKG-INFO
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      299 2023-05-19 16:12:55.000000 mid_to_gcode-0.0.0a2/mid_to_gcode.egg-info/SOURCES.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)        1 2023-05-19 16:12:55.000000 mid_to_gcode-0.0.0a2/mid_to_gcode.egg-info/dependency_links.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)       13 2023-05-19 16:12:55.000000 mid_to_gcode-0.0.0a2/mid_to_gcode.egg-info/top_level.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)      669 2023-05-19 16:12:47.000000 mid_to_gcode-0.0.0a2/pyproject.toml
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)       38 2023-05-19 16:12:55.253206 mid_to_gcode-0.0.0a2/setup.cfg
+-rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1332 2023-05-17 18:22:46.000000 mid_to_gcode-0.0.0a2/setup.py
```

### Comparing `mid_to_gcode-0.0.0a1/LICENSE` & `mid_to_gcode-0.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `mid_to_gcode-0.0.0a1/mid_to_gcode/functions.py` & `mid_to_gcode-0.0.0a2/mid_to_gcode/functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,49 @@
 from typing import Any
 
 from mido import MidiFile, MidiTrack
 
-from .support_functions import pair_range, number_to_ghz
+from .support_functions import accords_range, number_to_ghz, get_time_per_note, get_sr_per_note
 
 
 def prepearing(mid_file: MidiFile) -> tuple[MidiTrack, dict[str, Any]]:
     new_track = MidiTrack()
     config = {
         'control_change': []
     }
 
     if len(mid_file.tracks) > 1:
         print('WARNING: more than one track')
         [mid_file.tracks.remove(track) for track in mid_file.tracks[1:]]
 
-    use_accords_flag = False
-    last_note = None
     for msg in mid_file.tracks[0]:
-        if msg.type == 'note_on':
-            if not last_note and msg.velocity != 0:
-                last_note = msg.note
-                new_track.append(msg)
-
-            elif msg.velocity == 0 and last_note == msg.note:
-                new_track.append(msg)
-                last_note = None
-            
-            elif last_note and msg.velocity != 0:
-                use_accords_flag = True
+        if msg.type == 'note_on' or msg.type == 'note_off':
+            new_track.append(msg)
 
         elif msg.type == 'control_change':
             config['control_change'].append({
                 'channel': msg.channel,
                 'control': msg.control,
                 'value': msg.value,
                 'time': msg.time,
             })
         
         elif msg.type == 'set_tempo':
             config['set_tempo'] = msg.tempo
     
-    if use_accords_flag:
-        print('WARNING: the library can\'t process chords yet! From them the upper note is taken')
-    
     return new_track, config
 
 def convert_to_gcode(track: MidiTrack, config: dict[str, Any]) -> str:
     res = ''
 
-    for note_start, note_finish in pair_range(track):
-        note_time = note_finish.time + note_start.time
-        ghz = number_to_ghz(note_start.note)
-        
-        res += f'M300 P{note_time} S{ghz}\n'
+    for accord in accords_range(track):
+        note_time = get_time_per_note(accord)
+        for note in range(len(accord) - 1, -1, -1):
+            ghz = number_to_ghz(accord[note].note)
+            
+            # if note == 0:
+            #     res += f'M300 P{get_sr_per_note(accord) - (len(accord) - 1) * note_time} S{ghz}\n'
+            # else:
+            #     res += f'M300 P{note_time} S{ghz}\n'
+            res += f'M300 P{note_time} S{ghz}\n'
 
     return res
```

### Comparing `mid_to_gcode-0.0.0a1/pyproject.toml` & `mid_to_gcode-0.0.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mid-to-gcode"
-version = "0.0.0a1"
+version = "0.0.0a2"
 description = "The project for translate .mid format to 3d printers gcode "
 authors = ["GigantPro <pochtagigantpro@gmail.com>"]
 readme = "README.rst"
 packages = [{include = "mid_to_gcode"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `mid_to_gcode-0.0.0a1/setup.py` & `mid_to_gcode-0.0.0a2/setup.py`

 * *Files identical despite different names*

