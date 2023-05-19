# Comparing `tmp/basic-pitch-0.2.4.tar.gz` & `tmp/basic-pitch-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic-pitch-0.2.4.tar", last modified: Mon Apr 10 16:04:35 2023, max compression
+gzip compressed data, was "basic-pitch-0.2.5.tar", last modified: Fri May 19 16:52:46 2023, max compression
```

## Comparing `basic-pitch-0.2.4.tar` & `basic-pitch-0.2.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.644003 basic-pitch-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/OWNERS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-10 16:04:35.644003 basic-pitch-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.640003 basic-pitch-0.2.4/basic_pitch/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/commandline_printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17170 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.640003 basic-pitch-0.2.4/basic_pitch/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/layers/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    26142 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/layers/nnaudio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/layers/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/note_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.636003 basic-pitch-0.2.4/basic_pitch/saved_models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.636003 basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.640003 basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/
--rw-r--r--   0 runner    (1001) docker     (123)  1084140 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.640003 basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/variables/
--rw-r--r--   0 runner    (1001) docker     (123)   219309 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.640003 basic-pitch-0.2.4/basic_pitch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/catalog-info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-10 16:04:35.644003 basic-pitch-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.640003 basic-pitch-0.2.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.644003 basic-pitch-0.2.4/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   802472 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/tests/resources/vocadito_10.wav
--rw-r--r--   0 runner    (1001) docker     (123)  1075892 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/tests/resources/vocadito_14.wav
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/tests/test_note_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.505214 basic-pitch-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/OWNERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-19 16:52:46.505214 basic-pitch-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.501214 basic-pitch-0.2.5/basic_pitch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/commandline_printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.501214 basic-pitch-0.2.5/basic_pitch/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/layers/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26142 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/layers/nnaudio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/layers/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/note_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.497214 basic-pitch-0.2.5/basic_pitch/saved_models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.497214 basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.501214 basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/
+-rw-r--r--   0 runner    (1001) docker     (123)  1084140 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.505214 basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)   219309 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.501214 basic-pitch-0.2.5/basic_pitch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 16:52:46.000000 basic-pitch-0.2.5/basic_pitch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/catalog-info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-19 16:52:46.505214 basic-pitch-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.505214 basic-pitch-0.2.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:52:46.505214 basic-pitch-0.2.5/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   802472 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/tests/resources/vocadito_10.wav
+-rw-r--r--   0 runner    (1001) docker     (123)  1075892 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/tests/resources/vocadito_14.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/tests/test_note_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-19 16:52:32.000000 basic-pitch-0.2.5/tox.ini
```

### Comparing `basic-pitch-0.2.4/CODE_OF_CONDUCT.md` & `basic-pitch-0.2.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/CONTRIBUTING.md` & `basic-pitch-0.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/LICENSE` & `basic-pitch-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/NOTICE` & `basic-pitch-0.2.5/NOTICE`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/OWNERS.md` & `basic-pitch-0.2.5/OWNERS.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/PKG-INFO` & `basic-pitch-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basic-pitch
-Version: 0.2.4
+Version: 0.2.5
 Summary: Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection.
 Home-page: https://github.com/spotify/basic-pitch
 Author: Spotify
 Author-email: basic-pitch@spotify.com
 Maintainer: Spotify
 Maintainer-email: basic-pitch@spotify.com
 License: Apache 2.0
```

### Comparing `basic-pitch-0.2.4/README.md` & `basic-pitch-0.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
     pip install basic-pitch
 
 To update Basic Pitch to the latest version, add `--upgrade` to the above command.
 
 #### Compatible Environments:
 - MacOS, Windows and Ubuntu operating systems
-- Python versions 3.7, 3.8, 3.9
+- Python versions 3.7, 3.8, 3.9, 3.10
+- **For Mac M1 hardware, we currently only support python version 3.10. Otherwise, we suggest using a virtual machine.**
 
 
 ## Usage
 
 ### Model Prediction
 
 #### Command Line Tool
@@ -171,14 +172,18 @@
 
 This model can process any size or length of audio, but processing of larger/longer audio files could be limited by your machine's available disk space. To process these files, we recommend streaming the audio of the file, processing windows of audio at a time.
 
 **Sample Rate**
 
 Input audio maybe be of any sample rate, however, all audio will be resampled to 22050 Hz before processing.
 
+### VST
+
+Thanks to DamRsn for developing this working VST version of basic-pitch! - https://github.com/DamRsn/NeuralNote
+
 
 ## Contributing
 
 Contributions to `basic-pitch` are welcomed! See [CONTRIBUTING.md](CONTRIBUTING.md) for details.
 
 ## Copyright and License
 `basic-pitch` is Copyright 2022 Spotify AB.
```

### Comparing `basic-pitch-0.2.4/SECURITY.md` & `basic-pitch-0.2.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/basic_pitch/__init__.py` & `basic-pitch-0.2.5/basic_pitch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pathlib
 
 __author__ = "Spotify"
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 __email__ = "basic-pitch@spotify.com"
 __demowebsite__ = "https://basicpitch.io"
 __description__ = "Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection."
 __url__ = "https://github.com/spotify/basic-pitch"
 
 ICASSP_2022_MODEL_PATH = pathlib.Path(__file__).parent / "saved_models/icassp_2022/nmp"
```

### Comparing `basic-pitch-0.2.4/basic_pitch/commandline_printing.py` & `basic-pitch-0.2.5/basic_pitch/commandline_printing.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/basic_pitch/constants.py` & `basic-pitch-0.2.5/basic_pitch/constants.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/basic_pitch/inference.py` & `basic-pitch-0.2.5/basic_pitch/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # limitations under the License.
 
 import csv
 import enum
 import json
 import os
 import pathlib
-import traceback
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 from tensorflow import Tensor, signal, keras, saved_model
 import numpy as np
 import librosa
 import pretty_midi
 
@@ -401,37 +400,42 @@
             )
 
             if save_model_outputs:
                 model_output_path = build_output_path(audio_path, output_directory, OutputExtensions.MODEL_OUTPUT_NPZ)
                 try:
                     np.savez(model_output_path, basic_pitch_model_output=model_output)
                     file_saved_confirmation(OutputExtensions.MODEL_OUTPUT_NPZ.name, model_output_path)
-                except Exception:
+                except Exception as e:
                     failed_to_save(OutputExtensions.MODEL_OUTPUT_NPZ.name, model_output_path)
+                    raise e
 
             if save_midi:
-                midi_path = build_output_path(audio_path, output_directory, OutputExtensions.MIDI)
+                try:
+                    midi_path = build_output_path(audio_path, output_directory, OutputExtensions.MIDI)
+                except IOError as e:
+                    raise e
                 try:
                     midi_data.write(str(midi_path))
                     file_saved_confirmation(OutputExtensions.MIDI.name, midi_path)
-                except Exception:
+                except Exception as e:
                     failed_to_save(OutputExtensions.MIDI.name, midi_path)
+                    raise e
 
             if sonify_midi:
                 midi_sonify_path = build_output_path(audio_path, output_directory, OutputExtensions.MIDI_SONIFICATION)
                 try:
                     infer.sonify_midi(midi_data, midi_sonify_path, sr=sonification_samplerate)
                     file_saved_confirmation(OutputExtensions.MIDI_SONIFICATION.name, midi_sonify_path)
-                except Exception:
+                except Exception as e:
                     failed_to_save(OutputExtensions.MIDI_SONIFICATION.name, midi_sonify_path)
+                    raise e
 
             if save_notes:
                 note_events_path = build_output_path(audio_path, output_directory, OutputExtensions.NOTE_EVENTS)
                 try:
                     save_note_events(note_events, note_events_path)
                     file_saved_confirmation(OutputExtensions.NOTE_EVENTS.name, note_events_path)
-                except Exception:
+                except Exception as e:
                     failed_to_save(OutputExtensions.NOTE_EVENTS.name, note_events_path)
-        except Exception:
-            print("🚨 Something went wrong 😔 - see the traceback below for details.")
-            print("")
-            print(traceback.format_exc())
+                    raise e
+        except Exception as e:
+            raise e
```

### Comparing `basic-pitch-0.2.4/basic_pitch/layers/math.py` & `basic-pitch-0.2.5/basic_pitch/layers/math.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/basic_pitch/layers/nnaudio.py` & `basic-pitch-0.2.5/basic_pitch/layers/nnaudio.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/basic_pitch/layers/signal.py` & `basic-pitch-0.2.5/basic_pitch/layers/signal.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/basic_pitch/models.py` & `basic-pitch-0.2.5/basic_pitch/models.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/basic_pitch/nn.py` & `basic-pitch-0.2.5/basic_pitch/nn.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/basic_pitch/note_creation.py` & `basic-pitch-0.2.5/basic_pitch/note_creation.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/basic_pitch/predict.py` & `basic-pitch-0.2.5/basic_pitch/predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import argparse
 import os
 import pathlib
+import traceback
 
 from basic_pitch import ICASSP_2022_MODEL_PATH
 
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 
 
@@ -123,32 +124,39 @@
     output_dir = pathlib.Path(args.output_dir)
     verify_output_dir(output_dir)
 
     audio_path_list = [pathlib.Path(audio_path) for audio_path in args.audio_paths]
     for audio_path in audio_path_list:
         verify_input_path(audio_path)
 
-    predict_and_save(
-        audio_path_list,
-        output_dir,
-        args.save_midi,
-        args.sonify_midi,
-        args.save_model_outputs,
-        args.save_note_events,
-        pathlib.Path(args.model_path),
-        args.onset_threshold,
-        args.frame_threshold,
-        args.minimum_note_length,
-        args.minimum_frequency,
-        args.maximum_frequency,
-        args.multiple_pitch_bends,
-        not args.no_melodia,
-        pathlib.Path(args.debug_file) if args.debug_file else None,
-        args.sonification_samplerate,
-        args.midi_tempo,
-    )
-
-    print("\n✨ Done ✨\n")
+    try:
+        predict_and_save(
+            audio_path_list,
+            output_dir,
+            args.save_midi,
+            args.sonify_midi,
+            args.save_model_outputs,
+            args.save_note_events,
+            pathlib.Path(args.model_path),
+            args.onset_threshold,
+            args.frame_threshold,
+            args.minimum_note_length,
+            args.minimum_frequency,
+            args.maximum_frequency,
+            args.multiple_pitch_bends,
+            not args.no_melodia,
+            pathlib.Path(args.debug_file) if args.debug_file else None,
+            args.sonification_samplerate,
+            args.midi_tempo,
+        )
+        print("\n✨ Done ✨\n")
+    except IOError as ioe:
+        print(ioe)
+    except Exception as e:
+        print("🚨 Something went wrong 😔 - see the traceback below for details.")
+        print("")
+        print(e)
+        print(traceback.format_exc())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb` & `basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001` & `basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index` & `basic-pitch-0.2.5/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/basic_pitch.egg-info/PKG-INFO` & `basic-pitch-0.2.5/basic_pitch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basic-pitch
-Version: 0.2.4
+Version: 0.2.5
 Summary: Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection.
 Home-page: https://github.com/spotify/basic-pitch
 Author: Spotify
 Author-email: basic-pitch@spotify.com
 Maintainer: Spotify
 Maintainer-email: basic-pitch@spotify.com
 License: Apache 2.0
```

### Comparing `basic-pitch-0.2.4/basic_pitch.egg-info/SOURCES.txt` & `basic-pitch-0.2.5/basic_pitch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/setup.cfg` & `basic-pitch-0.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.4
+current_version = 0.2.5
 commit = True
 tag = True
 
 [metadata]
 name = basic-pitch
 version = attr: basic_pitch.__version__
 description = Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection.
```

### Comparing `basic-pitch-0.2.4/setup.py` & `basic-pitch-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/tests/resources/vocadito_10.wav` & `basic-pitch-0.2.5/tests/resources/vocadito_10.wav`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/tests/resources/vocadito_14.wav` & `basic-pitch-0.2.5/tests/resources/vocadito_14.wav`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/tests/test_inference.py` & `basic-pitch-0.2.5/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/tests/test_nn.py` & `basic-pitch-0.2.5/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/tests/test_note_creation.py` & `basic-pitch-0.2.5/tests/test_note_creation.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.4/tox.ini` & `basic-pitch-0.2.5/tox.ini`

 * *Files identical despite different names*

