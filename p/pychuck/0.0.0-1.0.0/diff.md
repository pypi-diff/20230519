# Comparing `tmp/pychuck-0.0.0.tar.gz` & `tmp/pychuck-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychuck-0.0.0.tar", last modified: Wed May 17 22:53:57 2023, max compression
+gzip compressed data, was "pychuck-1.0.0.tar", last modified: Fri May 19 01:28:41 2023, max compression
```

## Comparing `pychuck-0.0.0.tar` & `pychuck-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-17 22:53:57.446331 pychuck-0.0.0/
--rw-r--r--   0 ykli       (501) staff       (20)     1073 2023-05-12 02:50:29.000000 pychuck-0.0.0/LICENSE
--rw-r--r--   0 ykli       (501) staff       (20)     2177 2023-05-17 22:53:57.446225 pychuck-0.0.0/PKG-INFO
--rw-r--r--   0 ykli       (501) staff       (20)      480 2023-05-17 20:56:23.000000 pychuck-0.0.0/README.md
--rw-r--r--   0 ykli       (501) staff       (20)     1082 2023-05-17 22:50:06.000000 pychuck-0.0.0/pyproject.toml
--rw-r--r--   0 ykli       (501) staff       (20)       38 2023-05-17 22:53:57.446360 pychuck-0.0.0/setup.cfg
-drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-17 22:53:57.444754 pychuck-0.0.0/src/
-drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-17 22:53:57.445486 pychuck-0.0.0/src/pychuck/
--rw-r--r--   0 ykli       (501) staff       (20)      284 2023-05-17 13:42:38.000000 pychuck-0.0.0/src/pychuck/__init__.py
--rw-r--r--   0 ykli       (501) staff       (20)     3746 2023-05-17 21:15:43.000000 pychuck-0.0.0/src/pychuck/core.py
--rw-r--r--   0 ykli       (501) staff       (20)     3006 2023-05-17 21:31:38.000000 pychuck-0.0.0/src/pychuck/unit.py
--rw-r--r--   0 ykli       (501) staff       (20)     3409 2023-05-17 21:16:04.000000 pychuck-0.0.0/src/pychuck/util.py
-drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-17 22:53:57.446094 pychuck-0.0.0/src/pychuck.egg-info/
--rw-r--r--   0 ykli       (501) staff       (20)     2177 2023-05-17 22:53:57.000000 pychuck-0.0.0/src/pychuck.egg-info/PKG-INFO
--rw-r--r--   0 ykli       (501) staff       (20)      328 2023-05-17 22:53:57.000000 pychuck-0.0.0/src/pychuck.egg-info/SOURCES.txt
--rw-r--r--   0 ykli       (501) staff       (20)        1 2023-05-17 22:53:57.000000 pychuck-0.0.0/src/pychuck.egg-info/dependency_links.txt
--rw-r--r--   0 ykli       (501) staff       (20)       41 2023-05-17 22:53:57.000000 pychuck-0.0.0/src/pychuck.egg-info/entry_points.txt
--rw-r--r--   0 ykli       (501) staff       (20)       23 2023-05-17 22:53:57.000000 pychuck-0.0.0/src/pychuck.egg-info/requires.txt
--rw-r--r--   0 ykli       (501) staff       (20)        8 2023-05-17 22:53:57.000000 pychuck-0.0.0/src/pychuck.egg-info/top_level.txt
+drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-19 01:28:41.121923 pychuck-1.0.0/
+-rw-r--r--   0 ykli       (501) staff       (20)     1073 2023-05-18 08:14:19.000000 pychuck-1.0.0/LICENSE
+-rw-r--r--   0 ykli       (501) staff       (20)     2267 2023-05-19 01:28:41.121818 pychuck-1.0.0/PKG-INFO
+-rw-r--r--   0 ykli       (501) staff       (20)      501 2023-05-18 21:41:10.000000 pychuck-1.0.0/README.md
+-rw-r--r--   0 ykli       (501) staff       (20)     1175 2023-05-19 01:28:28.000000 pychuck-1.0.0/pyproject.toml
+-rw-r--r--   0 ykli       (501) staff       (20)       38 2023-05-19 01:28:41.121952 pychuck-1.0.0/setup.cfg
+drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-19 01:28:41.119338 pychuck-1.0.0/src/
+drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-19 01:28:41.120853 pychuck-1.0.0/src/pychuck/
+-rw-r--r--   0 ykli       (501) staff       (20)      278 2023-05-18 10:21:13.000000 pychuck-1.0.0/src/pychuck/__init__.py
+-rw-r--r--   0 ykli       (501) staff       (20)     3908 2023-05-18 21:30:14.000000 pychuck-1.0.0/src/pychuck/core.py
+-rw-r--r--   0 ykli       (501) staff       (20)     4176 2023-05-18 10:25:46.000000 pychuck-1.0.0/src/pychuck/unit.py
+-rw-r--r--   0 ykli       (501) staff       (20)     3439 2023-05-18 10:15:01.000000 pychuck-1.0.0/src/pychuck/util.py
+drwxr-xr-x   0 ykli       (501) staff       (20)        0 2023-05-19 01:28:41.121685 pychuck-1.0.0/src/pychuck.egg-info/
+-rw-r--r--   0 ykli       (501) staff       (20)     2267 2023-05-19 01:28:41.000000 pychuck-1.0.0/src/pychuck.egg-info/PKG-INFO
+-rw-r--r--   0 ykli       (501) staff       (20)      328 2023-05-19 01:28:41.000000 pychuck-1.0.0/src/pychuck.egg-info/SOURCES.txt
+-rw-r--r--   0 ykli       (501) staff       (20)        1 2023-05-19 01:28:41.000000 pychuck-1.0.0/src/pychuck.egg-info/dependency_links.txt
+-rw-r--r--   0 ykli       (501) staff       (20)       99 2023-05-19 01:28:41.000000 pychuck-1.0.0/src/pychuck.egg-info/entry_points.txt
+-rw-r--r--   0 ykli       (501) staff       (20)       47 2023-05-19 01:28:41.000000 pychuck-1.0.0/src/pychuck.egg-info/requires.txt
+-rw-r--r--   0 ykli       (501) staff       (20)        8 2023-05-19 01:28:41.000000 pychuck-1.0.0/src/pychuck.egg-info/top_level.txt
```

### Comparing `pychuck-0.0.0/LICENSE` & `pychuck-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pychuck-0.0.0/PKG-INFO` & `pychuck-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pychuck
-Version: 0.0.0
-Summary: Python implementation of the music programming language Chuck.
+Version: 1.0.0
+Summary: Python implementation of music programming language Chuck
 Author-email: Yikai Li <yikaili@stanford.edu>
 Maintainer-email: Yikai Li <yikaili@stanford.edu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -20,51 +20,56 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: repository, https://github.com/42x00/pychuck.git
-Keywords: chuck
+Keywords: chuck,music,programming,sound,synthesis
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: gui
+Provides-Extra: cli
 License-File: LICENSE
 
 # PyChucK
 
 ### Installation
 
 ```bash
 pip install pychuck
 ```
 
-### Usage
+### Quickstart
 
 ```python
 # demo.py
 from pychuck import *
 
 
-# Custom UGen
+# custom unit
 class Noise(UGen):
+    # generator
     def _tick(self, samples: int) -> np.ndarray:
         return np.random.uniform(-1, 1, samples)
 
 
-# Graph
-n = Noise()
+# unit
+n = Noise(gain=0.5)
+
+# graph
 n >> dac
 
-# Main loop
+# main loop
 while True:
-    # Adjust Parameters
+    # parameter
     n.gain = np.random.uniform(0, 1)
-    # Time Control
+    # time
     200 * ms >> now
 ```
 
 ```bash
 # pychuck --help
 pychuck demo.py
 ```
```

### Comparing `pychuck-0.0.0/pyproject.toml` & `pychuck-1.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pychuck"
-#version = "1.0"
-description = "Python implementation of the music programming language Chuck."
+version = "1.0.0"
+description = "Python implementation of music programming language Chuck"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
-keywords = ["chuck"]
+keywords = ["chuck", "music", "programming", "sound", "synthesis"]
 authors = [
     { name = "Yikai Li", email = "yikaili@stanford.edu" },
 ]
 maintainers = [
     { name = "Yikai Li", email = "yikaili@stanford.edu" },
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python"
 ]
 
 dependencies = [
     "numpy",
     "networkx",
-    "pyaudio",
+    "sounddevice",
 ]
 
-dynamic = ["version"]
+# dynamic = ["version", "description"]
 
 [project.optional-dependencies]
-#gui = ["PyQt5"]
-#cli = [
-#]
+gui = ["PyQt6"]
+cli = []
 
 [project.urls]
 #homepage = "https://example.com"
-#documentation = "https://readthedocs.org"
+#documentation = "https://pychuck.readthedocs.io/en/latest/"
 repository = "https://github.com/42x00/pychuck.git"
 #changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
 
 [project.scripts]
-pychuck = "pychuck:main"
+pychuck = "pychuck.core:main_cli"
 
-#[project.gui-scripts]
-#spam-gui = "spam:main_gui"
+[project.gui-scripts]
+pyaudicle = "pychuck.core:main_gui"
 
 #[project.entry-points."spam.magical"]
 #tomatoes = "spam:main_tomatoes"
```

### Comparing `pychuck-0.0.0/src/pychuck/core.py` & `pychuck-1.0.0/src/pychuck/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,119 @@
 import argparse
 import queue
 from types import GeneratorType
 from typing import List
 
+import sounddevice as sd
 import networkx as nx
 import numpy as np
 import pychuck
 from .unit import _Unit
 from .util import _wrap_code, _init_globals
 
 
 class _Shred:
     def __init__(self, generator: GeneratorType):
         self._samples_left: int = 0
         self._units: List[_Unit] = []
+        self._shreds: List[_Shred] = []
         self._generator: GeneratorType = generator
         if self._next():
             pychuck.VM._shreds.append(self)
 
     def _next(self):
         pychuck.me = self
         try:
             self._samples_left = int(next(self._generator))
             if self._samples_left < 0:
                 raise ValueError('Duration must be positive')
             return True
         except StopIteration:
             self._remove()
-            return False
+        return False
 
     def _remove(self):
+        for shred in self._shreds:
+            shred._remove()
+        self._shreds.clear()
         for unit in self._units:
             unit._remove()
+        self._units.clear()
         pychuck.VM._shreds.remove(self)
 
 
 class _Chuck:
-    def __init__(self, sample_rate: int = 44100, buffer_size: int = 256):
+    def __init__(self, sample_rate: int = 44100, buffer_size: int = 256, in_channels: int = 1, out_channels: int = 2):
         pychuck.VM = self
         self._sample_rate: int = sample_rate
         self._buffer_size: int = buffer_size
-        self._units: List[_Unit] = []
+        self._in_channels: int = in_channels
+        self._out_channels: int = out_channels
         self._shreds: List[_Shred] = []
         self._event_queue = queue.Queue()
         self._graph = nx.DiGraph()
+        self._sorted_graph: List[_Unit] = []
         _init_globals(sample_rate)
 
-    def callback(self, in_data: np.ndarray) -> np.ndarray:
-        pychuck.adc._set_buffer(in_data)
+    def callback(self, indata: np.ndarray) -> np.ndarray:
+        pychuck.adc._set_buffer(indata)
 
         while not self._event_queue.empty():
             self._handle_event(self._event_queue.get())
 
-        samples_left = length = len(in_data)
+        samples_left = length = len(indata)
         while samples_left > 0:
             samples_to_compute = min([samples_left] + [shred._samples_left for shred in self._shreds])
-            self._compute(samples_to_compute)
-            self._update_shreds(samples_to_compute)
+
+            for unit in self._sorted_graph:
+                unit._compute(samples_to_compute)
+
+            pychuck.now._value += samples_to_compute
+            for shred in self._shreds:
+                shred._samples_left -= samples_to_compute
+                if shred._samples_left <= 0:
+                    shred._next()
+
             samples_left -= samples_to_compute
 
         return pychuck.dac._get_buffer(length)
 
     def add_shred(self, code: str):
         exec(_wrap_code(code), globals())
         self._event_queue.put(globals()['__shred__']())
 
     def start(self):
-        import pyaudio
-        import time
-        def callback(in_data, frame_count, time_info, status_flags):
-            in_data = np.frombuffer(in_data, dtype=np.float32)
-            out_data = self.callback(in_data).tobytes()
-            return (out_data, pyaudio.paContinue)
-
-        pyaudio.PyAudio().open(rate=self._sample_rate,
-                               channels=1,
-                               format=pyaudio.paFloat32,
-                               input=True,
-                               output=True,
-                               frames_per_buffer=self._buffer_size,
-                               stream_callback=callback)
-        time.sleep(1e5)
+        def callback(indata, outdata, frames, time, status):
+            if status:
+                print(status)
+            outdata[:] = self.callback(indata)
+
+        sd.Stream(samplerate=self._sample_rate, blocksize=self._buffer_size,
+                  channels=(self._in_channels, self._out_channels), dtype=np.float32,
+                  callback=callback).start()
+        try:
+            sd.sleep(1000000)
+        except KeyboardInterrupt:
+            pass
 
     def _handle_event(self, event):
+        # TODO: Handle more events
         _Shred(event)
 
-    def _compute(self, samples: int):
-        for unit in self._units:
-            unit._compute(samples)
-
-    def _update_shreds(self, samples: int):
-        pychuck.now._value += samples
-        for shred in self._shreds:
-            shred._samples_left -= samples
-            if shred._samples_left <= 0:
-                shred._next()
-
-    def _update_graph(self):
-        try:
-            self._units = list(nx.topological_sort(self._graph))
-        except nx.NetworkXUnfeasible:
-            raise RuntimeError('Cyclic dependency detected')
+    def _sort_graph(self):
+        # TODO: Check for cycles
+        self._sorted_graph = list(nx.topological_sort(self._graph))
 
 
-def main():
+def main_cli():
     parser = argparse.ArgumentParser()
     parser.add_argument('--srate', type=int, default=44100)
     parser.add_argument('--bufsize', type=int, default=256)
+    parser.add_argument('--in', type=int, default=1, dest='in_channels')
+    parser.add_argument('--out', type=int, default=2)
     parser.add_argument('files', nargs='+', type=str)
     args = parser.parse_args()
-    chuck = _Chuck(sample_rate=args.srate, buffer_size=args.bufsize)
+    chuck = _Chuck(sample_rate=args.srate, buffer_size=args.bufsize,
+                   in_channels=args.in_channels, out_channels=args.out)
     for file in args.files:
         chuck.add_shred(open(file).read())
     chuck.start()
```

### Comparing `pychuck-0.0.0/src/pychuck/unit.py` & `pychuck-1.0.0/src/pychuck/unit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,41 @@
+from typing import List
+
 import numpy as np
 import pychuck
 
 
 class _Unit:
-    def __init__(self, _add2me: bool = True, *args, **kwargs):
-        if _add2me:
+    def __init__(self, add_to_shred: bool = True, add_to_graph: bool = True):
+        if add_to_shred:
             pychuck.me._units.append(self)
-        pychuck.VM._graph.add_node(self)
+        if add_to_graph:
+            pychuck.VM._graph.add_node(self)
+        self.chan: List[_Unit] = [self]
 
     def __rshift__(self, other: '_Unit') -> '_Unit':
-        pychuck.VM._graph.add_edge(self, other)
-        pychuck.VM._update_graph()
+        if len(self.chan) == len(other.chan):
+            for self_chan, other_chan in zip(self.chan, other.chan):
+                pychuck.VM._graph.add_edge(self_chan, other_chan)
+        else:
+            for self_chan in self.chan:
+                for other_chan in other.chan:
+                    pychuck.VM._graph.add_edge(self_chan, other_chan)
+        pychuck.VM._sort_graph()
         return other
 
     def __lshift__(self, other: '_Unit'):
-        pychuck.VM._graph.remove_edge(self, other)
-        pychuck.VM._update_graph()
+        for self_chan in self.chan:
+            for other_chan in other.chan:
+                pychuck.VM._graph.remove_edge(self_chan, other_chan)
+        pychuck.VM._sort_graph()
 
     def _remove(self):
         pychuck.VM._graph.remove_node(self)
-        pychuck.VM._update_graph()
+        pychuck.VM._sort_graph()
 
     def _compute(self, samples: int):
         raise NotImplementedError
 
 
 class UGen(_Unit):
     def __init__(self, gain: float = 1.0, *args, **kwargs):
@@ -34,68 +46,79 @@
         self._in_buffer: np.ndarray = np.zeros_like(self._buffer)
 
     def _compute(self, samples: int):
         self._aggregate_input(samples)
         self.buffered = self._tick(samples) * self.gain
 
     def _aggregate_input(self, samples: int):
-        self._in_buffer.fill(0.0)
-        for pred in pychuck.VM._graph.predecessors(self):
-            self._in_buffer[:samples] += pred.buffered
+        self._in_buffer.fill(0)
+        for predecessor in pychuck.VM._graph.predecessors(self):
+            self._in_buffer[:samples] += predecessor.buffered
 
     def _tick(self, samples: int) -> np.ndarray:
         raise NotImplementedError
 
 
-class _ADC(UGen):
+class _ADCChannel(UGen):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        super().__init__(add_to_shred=False, *args, **kwargs)
         self._i = 0
 
     def _compute(self, samples: int):
-        self.buffered = self._in_buffer[self._i:self._i + samples] * self.gain
+        self.buffered = self._buffer[self._i:self._i + samples] * self.gain
         self._i += samples
 
+
+class _ADC(UGen):
+    def __init__(self, *args, **kwargs):
+        super().__init__(add_to_shred=False, add_to_graph=False, *args, **kwargs)
+        self.chan = [_ADCChannel(*args, **kwargs) for _ in range(pychuck.VM._in_channels)]
+
     def _set_buffer(self, indata: np.ndarray):
         length = len(indata)
-        self._in_buffer[:length] = indata
-        self._i = 0
+        for i, chan in enumerate(self.chan):
+            chan._buffer[:length] = indata[:, i]
+            chan._i = 0
 
 
-class _DAC(UGen):
+class _DACChannel(UGen):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        super().__init__(add_to_shred=False, *args, **kwargs)
         self._i = 0
 
     def _compute(self, samples: int):
         self._aggregate_input(samples)
         self.buffered = self._in_buffer[:samples] * self.gain
         self._buffer[self._i:self._i + samples] = self.buffered
         self._i += samples
 
+
+class _DAC(UGen):
+    def __init__(self, *args, **kwargs):
+        super().__init__(add_to_shred=False, add_to_graph=False, *args, **kwargs)
+        self.chan = [_DACChannel(*args, **kwargs) for _ in range(pychuck.VM._out_channels)]
+
     def _get_buffer(self, length: int) -> np.ndarray:
-        self._i = 0
-        return self._buffer[:length]
+        for chan in self.chan:
+            chan._i = 0
+        return np.stack([chan._buffer[:length] for chan in self.chan], axis=1)
 
 
 class _Blackhole(UGen):
+    def __init__(self, *args, **kwargs):
+        super().__init__(add_to_shred=False, *args, **kwargs)
+
     def _compute(self, samples: int):
         pass
 
 
-class Gain(UGen):
-    def _tick(self, samples: int) -> np.ndarray:
-        return self._in_buffer[:samples]
-
-
 class SinOsc(UGen):
     def __init__(self, freq: float = 440.0, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.freq: float = freq
         self._phase: float = -np.pi / 2
         self._sample_rate: int = pychuck.VM._sample_rate
 
-    def _tick(self, samples: int) -> np.ndarray:
-        phase = self._phase + samples * 2 * np.pi * self.freq / self._sample_rate
-        ret = np.sin(np.linspace(self._phase, phase, samples, endpoint=False))
-        self._phase = phase
-        return ret
+    def _compute(self, samples: int):
+        new_phase = self._phase + samples * 2 * np.pi * self.freq / self._sample_rate
+        self.buffered = np.sin(np.linspace(self._phase, new_phase, samples, endpoint=False)) * self.gain
+        self._phase = new_phase
```

### Comparing `pychuck-0.0.0/src/pychuck/util.py` & `pychuck-1.0.0/src/pychuck/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 import ast
 
 import pychuck
 from .unit import _ADC, _DAC, _Blackhole
 
 
+def spork(generator):
+    current_shred = pychuck.me
+    current_shred._shreds.append(pychuck.core._Shred(generator))
+    pychuck.me = current_shred
+
+
 class _Time:
     def __init__(self, value: float):
-        self._value: float = value
+        self._value = value
 
     def __rshift__(self, other):
         raise NotImplementedError
 
     def __add__(self, other: '_Dur') -> '_Time':
         if isinstance(other, _Dur):
             return _Time(self._value + other._value)
         else:
             raise TypeError
 
-    def __sub__(self, other: '_Time' or '_Dur') -> '_Time' or '_Dur':
+    def __sub__(self, other: '_Time' or '_Dur') -> '_Dur' or '_Time':
         if isinstance(other, _Time):
             return _Dur(self._value - other._value)
         elif isinstance(other, _Dur):
             return _Time(self._value - other._value)
         else:
             raise TypeError
 
     def __str__(self) -> str:
         return str(self._value)
 
 
 class _Dur:
     def __init__(self, value: float):
-        self._value: float = value
-
-    def __rshift__(self, other):
-        raise NotImplementedError
+        self._value = value
 
     def __add__(self, other: '_Dur' or '_Time') -> '_Dur' or '_Time':
         if isinstance(other, _Dur):
             return _Dur(self._value + other._value)
         elif isinstance(other, _Time):
-            return _Time(other._value + self._value)
+            return _Time(self._value + other._value)
         else:
             raise TypeError
 
     def __sub__(self, other: '_Dur') -> '_Dur':
         if isinstance(other, _Dur):
             return _Dur(self._value - other._value)
         else:
@@ -52,15 +55,15 @@
 
     def __mul__(self, other: float) -> '_Dur':
         return _Dur(self._value * other)
 
     def __rmul__(self, other: float) -> '_Dur':
         return _Dur(self._value * other)
 
-    def __truediv__(self, other: '_Dur' or float) -> '_Dur' or float:
+    def __truediv__(self, other: '_Dur' or float) -> float or '_Dur':
         if isinstance(other, _Dur):
             return self._value / other._value
         else:
             return _Dur(self._value / other)
 
     def __int__(self) -> int:
         return int(self._value)
@@ -96,17 +99,17 @@
     code_tree = ast.parse(code)
     ast.fix_missing_locations(_CodeTransformer().visit(code_tree))
     wrapper_tree.body[1].body = code_tree.body
     return ast.unparse(wrapper_tree)
 
 
 def _init_globals(sample_rate: int):
-    pychuck.adc = _ADC(_add2me=False)
-    pychuck.dac = _DAC(_add2me=False)
-    pychuck.blackhole = _Blackhole(_add2me=False)
+    pychuck.adc = _ADC()
+    pychuck.dac = _DAC()
+    pychuck.blackhole = _Blackhole()
     pychuck.now = _Time(0)
     pychuck.samp = _Dur(1)
     pychuck.second = _Dur(sample_rate)
     pychuck.ms = pychuck.second / 1000
     pychuck.minute = pychuck.second * 60
     pychuck.hour = pychuck.minute * 60
     pychuck.day = pychuck.hour * 24
```

### Comparing `pychuck-0.0.0/src/pychuck.egg-info/PKG-INFO` & `pychuck-1.0.0/src/pychuck.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pychuck
-Version: 0.0.0
-Summary: Python implementation of the music programming language Chuck.
+Version: 1.0.0
+Summary: Python implementation of music programming language Chuck
 Author-email: Yikai Li <yikaili@stanford.edu>
 Maintainer-email: Yikai Li <yikaili@stanford.edu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -20,51 +20,56 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: repository, https://github.com/42x00/pychuck.git
-Keywords: chuck
+Keywords: chuck,music,programming,sound,synthesis
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: gui
+Provides-Extra: cli
 License-File: LICENSE
 
 # PyChucK
 
 ### Installation
 
 ```bash
 pip install pychuck
 ```
 
-### Usage
+### Quickstart
 
 ```python
 # demo.py
 from pychuck import *
 
 
-# Custom UGen
+# custom unit
 class Noise(UGen):
+    # generator
     def _tick(self, samples: int) -> np.ndarray:
         return np.random.uniform(-1, 1, samples)
 
 
-# Graph
-n = Noise()
+# unit
+n = Noise(gain=0.5)
+
+# graph
 n >> dac
 
-# Main loop
+# main loop
 while True:
-    # Adjust Parameters
+    # parameter
     n.gain = np.random.uniform(0, 1)
-    # Time Control
+    # time
     200 * ms >> now
 ```
 
 ```bash
 # pychuck --help
 pychuck demo.py
 ```
```

