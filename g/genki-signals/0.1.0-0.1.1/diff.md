# Comparing `tmp/genki_signals-0.1.0.tar.gz` & `tmp/genki_signals-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genki_signals-0.1.0.tar", last modified: Fri May 19 15:13:46 2023, max compression
+gzip compressed data, was "genki_signals-0.1.1.tar", last modified: Fri May 19 17:57:56 2023, max compression
```

## Comparing `genki_signals-0.1.0.tar` & `genki_signals-0.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 15:13:46.757381 genki_signals-0.1.0/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1108 2023-05-19 15:13:46.757178 genki_signals-0.1.0/PKG-INFO
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      592 2023-05-19 11:53:35.000000 genki_signals-0.1.0/README.md
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 15:13:46.751006 genki_signals-0.1.0/genki_signals/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      537 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/__init__.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     8700 2023-05-10 16:26:33.000000 genki_signals-0.1.0/genki_signals/buffers.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2233 2023-05-16 15:12:05.000000 genki_signals-0.1.0/genki_signals/dead_reckoning.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     8182 2023-05-10 13:32:35.000000 genki_signals-0.1.0/genki_signals/filters.py
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 15:13:46.752640 genki_signals-0.1.0/genki_signals/frontends/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)       94 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/frontends/__init__.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      429 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/frontends/base.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)    11308 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/frontends/visualization.py
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 15:13:46.754583 genki_signals-0.1.0/genki_signals/functions/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      917 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/functions/__init__.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     5492 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/functions/arithmetic.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1666 2023-05-19 15:08:48.000000 genki_signals-0.1.0/genki_signals/functions/base.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     3197 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/functions/filters.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)    13660 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/functions/geometry.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2433 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/functions/inference.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      880 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/functions/serialization.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2774 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/functions/shape.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1946 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/functions/waveforms.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     4756 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/functions/windowed.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1008 2023-05-16 15:12:05.000000 genki_signals-0.1.0/genki_signals/fusion.py
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 15:13:46.754774 genki_signals-0.1.0/genki_signals/models/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2445 2023-05-04 16:25:52.000000 genki_signals-0.1.0/genki_signals/models/letter_detection_model.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2489 2023-05-16 14:58:32.000000 genki_signals-0.1.0/genki_signals/recorders.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     5542 2023-05-19 15:08:48.000000 genki_signals-0.1.0/genki_signals/session.py
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 15:13:46.756877 genki_signals-0.1.0/genki_signals/sources/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      551 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/sources/__init__.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      376 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/sources/base.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     4871 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/sources/ble.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2301 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/sources/dataframe.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      337 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/sources/generators.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     4828 2023-05-19 15:08:48.000000 genki_signals-0.1.0/genki_signals/sources/local.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2596 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/sources/sampler.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     3935 2023-05-19 14:59:19.000000 genki_signals-0.1.0/genki_signals/sources/wave.py
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     3393 2023-05-19 15:08:48.000000 genki_signals-0.1.0/genki_signals/system.py
-drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 15:13:46.751898 genki_signals-0.1.0/genki_signals.egg-info/
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1108 2023-05-19 15:13:46.000000 genki_signals-0.1.0/genki_signals.egg-info/PKG-INFO
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1200 2023-05-19 15:13:46.000000 genki_signals-0.1.0/genki_signals.egg-info/SOURCES.txt
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)        1 2023-05-19 15:13:46.000000 genki_signals-0.1.0/genki_signals.egg-info/dependency_links.txt
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      100 2023-05-19 15:13:46.000000 genki_signals-0.1.0/genki_signals.egg-info/requires.txt
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)       14 2023-05-19 15:13:46.000000 genki_signals-0.1.0/genki_signals.egg-info/top_level.txt
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)       31 2023-05-17 15:55:12.000000 genki_signals-0.1.0/pyproject.toml
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)       38 2023-05-19 15:13:46.757433 genki_signals-0.1.0/setup.cfg
--rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1436 2023-05-19 11:53:35.000000 genki_signals-0.1.0/setup.py
+drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.071357 genki_signals-0.1.1/
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1108 2023-05-19 17:57:56.071144 genki_signals-0.1.1/PKG-INFO
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      592 2023-05-19 11:53:35.000000 genki_signals-0.1.1/README.md
+drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.062967 genki_signals-0.1.1/genki_signals/
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      537 2023-05-19 17:56:29.000000 genki_signals-0.1.1/genki_signals/__init__.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     8700 2023-05-10 16:26:33.000000 genki_signals-0.1.1/genki_signals/buffers.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2233 2023-05-16 15:12:05.000000 genki_signals-0.1.1/genki_signals/dead_reckoning.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     8182 2023-05-10 13:32:35.000000 genki_signals-0.1.1/genki_signals/filters.py
+drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.065029 genki_signals-0.1.1/genki_signals/frontends/
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)       94 2023-05-19 15:44:12.000000 genki_signals-0.1.1/genki_signals/frontends/__init__.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      429 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/frontends/base.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)    11322 2023-05-19 17:56:29.000000 genki_signals-0.1.1/genki_signals/frontends/visualization.py
+drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.068276 genki_signals-0.1.1/genki_signals/functions/
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      964 2023-05-19 17:56:29.000000 genki_signals-0.1.1/genki_signals/functions/__init__.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     5492 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/arithmetic.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1666 2023-05-19 15:08:48.000000 genki_signals-0.1.1/genki_signals/functions/base.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     3197 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/filters.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)    13660 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/geometry.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2433 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/inference.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      880 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/serialization.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     3702 2023-05-19 17:56:29.000000 genki_signals-0.1.1/genki_signals/functions/shape.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1946 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/waveforms.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     4756 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/functions/windowed.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1008 2023-05-16 15:12:05.000000 genki_signals-0.1.1/genki_signals/fusion.py
+drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.068524 genki_signals-0.1.1/genki_signals/models/
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2445 2023-05-04 16:25:52.000000 genki_signals-0.1.1/genki_signals/models/letter_detection_model.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2489 2023-05-16 14:58:32.000000 genki_signals-0.1.1/genki_signals/recorders.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     5542 2023-05-19 15:08:48.000000 genki_signals-0.1.1/genki_signals/session.py
+drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.070824 genki_signals-0.1.1/genki_signals/sources/
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      660 2023-05-19 17:56:29.000000 genki_signals-0.1.1/genki_signals/sources/__init__.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      376 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/sources/base.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     4871 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/sources/ble.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2301 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/sources/dataframe.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      337 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/sources/generators.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     4828 2023-05-19 15:21:22.000000 genki_signals-0.1.1/genki_signals/sources/local.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     2596 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/sources/sampler.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     3935 2023-05-19 14:59:19.000000 genki_signals-0.1.1/genki_signals/sources/wave.py
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     3393 2023-05-19 15:08:48.000000 genki_signals-0.1.1/genki_signals/system.py
+drwxr-xr-x   0 bjarnihaukurbjarnason   (501) staff       (20)        0 2023-05-19 17:57:56.064196 genki_signals-0.1.1/genki_signals.egg-info/
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1108 2023-05-19 17:57:56.000000 genki_signals-0.1.1/genki_signals.egg-info/PKG-INFO
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1200 2023-05-19 17:57:56.000000 genki_signals-0.1.1/genki_signals.egg-info/SOURCES.txt
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)        1 2023-05-19 17:57:56.000000 genki_signals-0.1.1/genki_signals.egg-info/dependency_links.txt
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)      115 2023-05-19 17:57:56.000000 genki_signals-0.1.1/genki_signals.egg-info/requires.txt
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)       14 2023-05-19 17:57:56.000000 genki_signals-0.1.1/genki_signals.egg-info/top_level.txt
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)       31 2023-05-17 15:55:12.000000 genki_signals-0.1.1/pyproject.toml
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)       38 2023-05-19 17:57:56.071423 genki_signals-0.1.1/setup.cfg
+-rw-r--r--   0 bjarnihaukurbjarnason   (501) staff       (20)     1625 2023-05-19 17:57:45.000000 genki_signals-0.1.1/setup.py
```

### Comparing `genki_signals-0.1.0/PKG-INFO` & `genki_signals-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genki_signals
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for realtime signal processing and machine learning
 Home-page: https://github.com/genkiinstruments/genki-signals
 Author: Genki Instruments
 Author-email: genki@genkiinstruments.com
 Keywords: Signal Processing,Machine Learning,Realtime
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `genki_signals-0.1.0/README.md` & `genki_signals-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/__init__.py` & `genki_signals-0.1.1/genki_signals/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .fusion import *
 from .recorders import *
 from .session import *
 from .system import *
 
 from .buffers import Buffer, DataBuffer
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 __doc__ = """
 genki_signals
 =============
 
 Description
 -----------
```

### Comparing `genki_signals-0.1.0/genki_signals/buffers.py` & `genki_signals-0.1.1/genki_signals/buffers.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/dead_reckoning.py` & `genki_signals-0.1.1/genki_signals/dead_reckoning.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/filters.py` & `genki_signals-0.1.1/genki_signals/filters.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/frontends/visualization.py` & `genki_signals-0.1.1/genki_signals/frontends/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from abc import ABC, abstractmethod
 from typing import Literal
 
 import cv2
 import bqplot as bq
 import ipywidgets
 from ipywidgets import Image
+from IPython.display import display
 
 from genki_signals.buffers import DataBuffer
 from genki_signals.system import System
 from genki_signals.frontends.base import FrontendBase
 
 
 class WidgetFrontend(FrontendBase):
@@ -38,27 +39,27 @@
             cols = []
             for j in range(n):
                 try:
                     cols.append(self.widgets[i * n + j].widget)
                 except IndexError:
                     pass
             rows.append(ipywidgets.HBox(cols))
-        return ipywidgets.VBox(rows)._ipython_display_()
+        return display(ipywidgets.VBox(rows))
 
 
 class PlottableWidget(ABC):
     def __init__(self):
         self.widget = None
 
     @abstractmethod
     def update(self, data: DataBuffer):
         pass
 
     def _ipython_display_(self):
-        return self.widget._ipython_display_()
+        return display(self.widget)
 
 
 class Video(PlottableWidget):
     def __init__(self, video_key: str):
         super().__init__()
 
         self.video_key = video_key
```

### Comparing `genki_signals-0.1.0/genki_signals/functions/__init__.py` & `genki_signals-0.1.1/genki_signals/functions/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 deserialized, and their parameters can be treated like hyperparameters
 in a machine learning model. When a data session is recorded with a signal
 system, only the json serialisation of the signal functions is stored.
 Signal functions are also assumed to be causal, i.e. they only depend
 on past values of the input and can thus be computed in real time.
 """
 
-
 from .arithmetic import *  # noqa: F401, F403
 from .filters import *  # noqa: F401, F403
 from .geometry import *  # noqa: F401, F403
 from .inference import *  # noqa: F401, F403
 from .windowed import *  # noqa: F401, F403
 from .shape import *  # noqa: F401, F403
 from .waveforms import *  # noqa: F401, F403
-from .base import compute_signal_functions
+from .base import compute_signal_functions, SignalFunction, SignalName  # noqa: F401, F403
```

### Comparing `genki_signals-0.1.0/genki_signals/functions/arithmetic.py` & `genki_signals-0.1.1/genki_signals/functions/arithmetic.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/functions/base.py` & `genki_signals-0.1.1/genki_signals/functions/base.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/functions/filters.py` & `genki_signals-0.1.1/genki_signals/functions/filters.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/functions/geometry.py` & `genki_signals-0.1.1/genki_signals/functions/geometry.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/functions/inference.py` & `genki_signals-0.1.1/genki_signals/functions/inference.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/functions/serialization.py` & `genki_signals-0.1.1/genki_signals/functions/serialization.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/functions/shape.py` & `genki_signals-0.1.1/genki_signals/functions/shape.py`

 * *Files 17% similar despite different names*

```diff
@@ -79,13 +79,36 @@
         self.shape = shape
 
     def __call__(self, v):
         time = v.shape[-1]
         return v.reshape(self.shape + (time,))
 
 
+class Combine(SignalFunction):
+    def __init__(self, signal_fns, name: str):
+        self.signal_fns = signal_fns
+        internal_outputs = [fn.name for fn in signal_fns]
+        all_inputs = set().union(*[fn.input_signals for fn in signal_fns])
+        inputs = all_inputs - set(internal_outputs)
+        super().__init__(*inputs, name=name, params={"signal_fns": signal_fns})
+
+    def __call__(self, *args):
+        internal_outputs = {}
+        for fn in self.signal_fns:
+            fn_inputs = []
+            for fn_input in fn.input_signals:
+                if fn_input in internal_outputs:
+                    fn_inputs.append(internal_outputs[fn_input])
+                else:
+                    fn_inputs.append(args[self.input_signals.index(fn_input)])
+            fn_output = fn(*fn_inputs)
+            internal_outputs[fn.name] = fn_output
+        return internal_outputs[self.signal_fns[-1].name]
+
+
 __all__ = [
     "ExtractDimension",
     "Concatenate",
     "Stack",
     "Reshape",
+    "Combine"
 ]
```

### Comparing `genki_signals-0.1.0/genki_signals/functions/waveforms.py` & `genki_signals-0.1.1/genki_signals/functions/waveforms.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/functions/windowed.py` & `genki_signals-0.1.1/genki_signals/functions/windowed.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/fusion.py` & `genki_signals-0.1.1/genki_signals/fusion.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/models/letter_detection_model.py` & `genki_signals-0.1.1/genki_signals/models/letter_detection_model.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/recorders.py` & `genki_signals-0.1.1/genki_signals/recorders.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/session.py` & `genki_signals-0.1.1/genki_signals/session.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/sources/__init__.py` & `genki_signals-0.1.1/genki_signals/sources/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,12 +2,14 @@
 Signal sources are classes that sample signals from various sources, usually external devices.
 
 Some signal sources act as "samplers" meaning they have their own clock and sample at a given rate.
 Other sources are pure "sources" which means they can only generate data when asked to do so, and
 need to be sampled by a sampler.
 """
 
+from .base import SignalSource, SamplerBase  # noqa: F401, F403
 from .sampler import Sampler  # noqa: F401, F403
 from .generators import *  # noqa: F401, F403
-from .wave import *  # noqa: F401, F403
 from .local import *  # noqa: F401, F403
+from .dataframe import *  # noqa: F401, F403
 from .ble import *  # noqa: F401, F403
+from .wave import *  # noqa: F401, F403
```

### Comparing `genki_signals-0.1.0/genki_signals/sources/ble.py` & `genki_signals-0.1.1/genki_signals/sources/ble.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/sources/dataframe.py` & `genki_signals-0.1.1/genki_signals/sources/dataframe.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/sources/local.py` & `genki_signals-0.1.1/genki_signals/sources/local.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/sources/sampler.py` & `genki_signals-0.1.1/genki_signals/sources/sampler.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/sources/wave.py` & `genki_signals-0.1.1/genki_signals/sources/wave.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals/system.py` & `genki_signals-0.1.1/genki_signals/system.py`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/genki_signals.egg-info/PKG-INFO` & `genki_signals-0.1.1/genki_signals.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genki-signals
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for realtime signal processing and machine learning
 Home-page: https://github.com/genkiinstruments/genki-signals
 Author: Genki Instruments
 Author-email: genki@genkiinstruments.com
 Keywords: Signal Processing,Machine Learning,Realtime
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `genki_signals-0.1.0/genki_signals.egg-info/SOURCES.txt` & `genki_signals-0.1.1/genki_signals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genki_signals-0.1.0/setup.py` & `genki_signals-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,20 @@
     version = getversion.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 short_description = "A library for realtime signal processing and machine learning"
 long_description = open("README.md").read()
 
+print()
+print("Version: ", version)
+print("Short description: ", short_description)
+print("Long description: ", long_description[:100], "...")
+print()
+
 setuptools.setup(
     name="genki_signals",
     version=version,
     description=short_description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     license_files=["LICENSE"],
@@ -25,16 +31,18 @@
     install_requires=[
         "numpy",
         "pandas",
         "scipy",
         "onnx",
         "onnxruntime",
         "opencv-python",
+        "pynput",
         "bqplot",
         "ipywidgets",
+        "IPython",
         "ahrs",
         "imufusion",
         "bleak",
         "genki_wave",
     ],
     author="Genki Instruments",
     author_email="genki@genkiinstruments.com",
```

