# Comparing `tmp/OmeSliCC-0.5.1.2.tar.gz` & `tmp/OmeSliCC-0.5.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OmeSliCC-0.5.1.2.tar", last modified: Thu May 18 21:48:06 2023, max compression
+gzip compressed data, was "OmeSliCC-0.5.1b0.tar", last modified: Thu May 18 20:43:10 2023, max compression
```

## Comparing `OmeSliCC-0.5.1.2.tar` & `OmeSliCC-0.5.1b0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 21:48:06.916609 OmeSliCC-0.5.1.2/
--rw-rw-rw-   0        0        0    36454 2022-09-16 15:34:35.000000 OmeSliCC-0.5.1.2/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-05-18 21:48:06.901727 OmeSliCC-0.5.1.2/OmeSliCC/
--rw-rw-rw-   0        0        0     3133 2023-05-18 21:03:21.000000 OmeSliCC-0.5.1.2/OmeSliCC/BioSource.py
--rw-rw-rw-   0        0        0    12073 2023-05-18 21:04:15.000000 OmeSliCC-0.5.1.2/OmeSliCC/OmeSource.py
--rw-rw-rw-   0        0        0     5942 2023-05-18 21:03:54.000000 OmeSliCC-0.5.1.2/OmeSliCC/Omero.py
--rw-rw-rw-   0        0        0     2046 2023-05-18 19:37:19.000000 OmeSliCC-0.5.1.2/OmeSliCC/OmeroLabelReader.py
--rw-rw-rw-   0        0        0     4682 2023-05-18 21:04:07.000000 OmeSliCC-0.5.1.2/OmeSliCC/OmeroSource.py
--rw-rw-rw-   0        0        0     3323 2023-05-18 21:04:25.000000 OmeSliCC-0.5.1.2/OmeSliCC/PlainImageSource.py
--rw-rw-rw-   0        0        0    11948 2023-05-18 21:04:33.000000 OmeSliCC-0.5.1.2/OmeSliCC/TiffSource.py
--rw-rw-rw-   0        0        0     1896 2023-03-25 15:06:02.000000 OmeSliCC-0.5.1.2/OmeSliCC/XmlDict.py
--rw-rw-rw-   0        0        0     4710 2023-05-18 21:04:49.000000 OmeSliCC-0.5.1.2/OmeSliCC/ZarrSource.py
--rw-rw-rw-   0        0        0    11624 2023-05-18 21:03:34.000000 OmeSliCC-0.5.1.2/OmeSliCC/conversion.py
--rw-rw-rw-   0        0        0    10772 2023-05-18 21:03:40.000000 OmeSliCC-0.5.1.2/OmeSliCC/image_util.py
--rw-rw-rw-   0        0        0    17535 2023-05-18 21:03:47.000000 OmeSliCC-0.5.1.2/OmeSliCC/ome.py
--rw-rw-rw-   0        0        0     1298 2022-10-27 12:37:45.000000 OmeSliCC-0.5.1.2/OmeSliCC/omero_credentials.py
--rw-rw-rw-   0        0        0      225 2022-09-29 12:36:36.000000 OmeSliCC-0.5.1.2/OmeSliCC/parameters.py
--rw-rw-rw-   0        0        0     4970 2023-03-06 12:50:47.000000 OmeSliCC-0.5.1.2/OmeSliCC/util.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:48:06.909701 OmeSliCC-0.5.1.2/OmeSliCC.egg-info/
--rw-rw-rw-   0        0        0    44210 2023-05-18 21:48:06.000000 OmeSliCC-0.5.1.2/OmeSliCC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      594 2023-05-18 21:48:06.000000 OmeSliCC-0.5.1.2/OmeSliCC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 21:48:06.000000 OmeSliCC-0.5.1.2/OmeSliCC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      209 2023-05-18 21:48:06.000000 OmeSliCC-0.5.1.2/OmeSliCC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 21:48:06.000000 OmeSliCC-0.5.1.2/OmeSliCC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    44210 2023-05-18 21:48:06.915598 OmeSliCC-0.5.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2210 2023-03-04 11:28:54.000000 OmeSliCC-0.5.1.2/README.md
--rw-rw-rw-   0        0        0      493 2023-05-18 21:47:48.000000 OmeSliCC-0.5.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      232 2023-05-18 20:12:27.000000 OmeSliCC-0.5.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 21:48:06.916609 OmeSliCC-0.5.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-18 21:48:06.913629 OmeSliCC-0.5.1.2/tests/
--rw-rw-rw-   0        0        0      325 2023-05-18 21:05:09.000000 OmeSliCC-0.5.1.2/tests/label_reader_test.py
--rw-rw-rw-   0        0        0     4474 2023-05-18 21:05:14.000000 OmeSliCC-0.5.1.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:43:10.707701 OmeSliCC-0.5.1b0/
+-rw-rw-rw-   0        0        0    36454 2022-09-16 15:34:35.000000 OmeSliCC-0.5.1b0/LICENSE.md
+-rw-rw-rw-   0        0        0    44210 2023-05-18 20:43:10.706702 OmeSliCC-0.5.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0     2210 2023-03-04 11:28:54.000000 OmeSliCC-0.5.1b0/README.md
+-rw-rw-rw-   0        0        0      433 2023-05-18 20:42:46.000000 OmeSliCC-0.5.1b0/pyproject.toml
+-rw-rw-rw-   0        0        0      232 2023-05-18 20:12:27.000000 OmeSliCC-0.5.1b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 20:43:10.707701 OmeSliCC-0.5.1b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 20:43:10.665743 OmeSliCC-0.5.1b0/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 20:43:10.694699 OmeSliCC-0.5.1b0/src/OmeSliCC/
+-rw-rw-rw-   0        0        0     3141 2023-05-18 19:44:23.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/BioSource.py
+-rw-rw-rw-   0        0        0    12089 2023-05-18 19:44:39.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/OmeSource.py
+-rw-rw-rw-   0        0        0     5950 2023-05-18 19:43:38.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/Omero.py
+-rw-rw-rw-   0        0        0     2046 2023-05-18 19:37:19.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/OmeroLabelReader.py
+-rw-rw-rw-   0        0        0     4702 2023-05-18 19:45:26.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/OmeroSource.py
+-rw-rw-rw-   0        0        0     3335 2023-05-18 19:44:46.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/PlainImageSource.py
+-rw-rw-rw-   0        0        0    11964 2023-05-18 19:45:50.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/TiffSource.py
+-rw-rw-rw-   0        0        0     1896 2023-03-25 15:06:02.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/XmlDict.py
+-rw-rw-rw-   0        0        0     4718 2023-05-18 19:46:09.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/ZarrSource.py
+-rw-rw-rw-   0        0        0    11660 2023-05-18 19:44:05.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/conversion.py
+-rw-rw-rw-   0        0        0    10776 2023-05-18 19:45:10.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/image_util.py
+-rw-rw-rw-   0        0        0    17547 2023-05-18 19:44:55.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/ome.py
+-rw-rw-rw-   0        0        0     1298 2022-10-27 12:37:45.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/omero_credentials.py
+-rw-rw-rw-   0        0        0      225 2022-09-29 12:36:36.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/parameters.py
+-rw-rw-rw-   0        0        0     4970 2023-03-06 12:50:47.000000 OmeSliCC-0.5.1b0/src/OmeSliCC/util.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:43:10.704698 OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/
+-rw-rw-rw-   0        0        0    44210 2023-05-18 20:43:10.000000 OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2023-05-18 20:43:10.000000 OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 20:43:10.000000 OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      209 2023-05-18 20:43:10.000000 OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 20:43:10.000000 OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 20:43:10.705703 OmeSliCC-0.5.1b0/tests/
+-rw-rw-rw-   0        0        0     4482 2023-05-18 19:41:34.000000 OmeSliCC-0.5.1b0/tests/test.py
```

### Comparing `OmeSliCC-0.5.1.2/LICENSE.md` & `OmeSliCC-0.5.1b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/BioSource.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/BioSource.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import bioformats
 import javabridge
 from bioformats.formatreader import ImageReader
 
-from OmeSliCC import XmlDict
-from OmeSliCC.OmeSource import OmeSource
+from src.OmeSliCC import XmlDict
+from src.OmeSliCC.OmeSource import OmeSource
 
 
 class BioSource(OmeSource):
     """bioformats compatible image source"""
 
     filename: str
     """original filename"""
```

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/OmeSource.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/OmeSource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import numpy as np
 
-from OmeSliCC.XmlDict import XmlDict
-from OmeSliCC.ome import create_ome_metadata
-from OmeSliCC.image_util import *
-from OmeSliCC.util import *
+from src.OmeSliCC.XmlDict import XmlDict
+from src.OmeSliCC.ome import create_ome_metadata
+from src.OmeSliCC.image_util import *
+from src.OmeSliCC.util import *
 
 
 class OmeSource:
     """OME-compatible image source (base class)"""
 
     metadata: dict
     """metadata dictionary"""
```

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/Omero.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/Omero.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 import logging
 import omero
 from omero.gateway import BlitzGateway
 import omero.model
 from types import TracebackType
 
-from OmeSliCC.omero_credentials import decrypt_credentials
-from OmeSliCC.util import *
+from src.OmeSliCC.omero_credentials import decrypt_credentials
+from src.OmeSliCC.util import *
 
 
 class Omero:
     """Omero image and metadata extraction"""
     
     def __init__(self, params: dict):
         self.params = params
```

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/OmeroLabelReader.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/OmeroLabelReader.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/OmeroSource.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/OmeroSource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import io
 import numpy as np
 import PIL.Image
 import omero.gateway
 
-from OmeSliCC import Omero
-from OmeSliCC.OmeSource import OmeSource
-from OmeSliCC.ome import create_ome_metadata_from_omero
-from OmeSliCC.XmlDict import XmlDict
-from OmeSliCC.util import *
+from src.OmeSliCC import Omero
+from src.OmeSliCC.OmeSource import OmeSource
+from src.OmeSliCC.ome import create_ome_metadata_from_omero
+from src.OmeSliCC.XmlDict import XmlDict
+from src.OmeSliCC.util import *
 
 
 class OmeroSource(OmeSource):
     """Omero image source"""
 
     omero: Omero
     """Omero instance"""
```

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/PlainImageSource.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/PlainImageSource.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import numpy as np
 from PIL import Image
 from concurrent.futures import ThreadPoolExecutor
 
-from OmeSliCC.OmeSource import OmeSource
-from OmeSliCC.XmlDict import XmlDict
-from OmeSliCC.image_util import *
+from src.OmeSliCC.OmeSource import OmeSource
+from src.OmeSliCC.XmlDict import XmlDict
+from src.OmeSliCC.image_util import *
 
 Image.MAX_IMAGE_PIXELS = None   # avoid DecompressionBombError (which prevents loading large images)
 
 
 class PlainImageSource(OmeSource):
     """Plain common format image source"""
```

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/TiffSource.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/TiffSource.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 import os
 from enum import Enum
 import numpy as np
 from tifffile import TiffFile, TiffPage
 from concurrent.futures import ThreadPoolExecutor
 
-from OmeSliCC import XmlDict
-from OmeSliCC.OmeSource import OmeSource
-from OmeSliCC.image_util import *
-from OmeSliCC.util import *
+from src.OmeSliCC import XmlDict
+from src.OmeSliCC.OmeSource import OmeSource
+from src.OmeSliCC.image_util import *
+from src.OmeSliCC.util import *
 
 
 class TiffSource(OmeSource):
     """Tiff-compatible image source"""
 
     filename: str
     """original filename"""
```

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/XmlDict.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/XmlDict.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/ZarrSource.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/ZarrSource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import zarr
 from zarr.errors import GroupNotFoundError
 
-from OmeSliCC.OmeSource import OmeSource
-from OmeSliCC.XmlDict import XmlDict
+from src.OmeSliCC.OmeSource import OmeSource
+from src.OmeSliCC.XmlDict import XmlDict
 
 
 class ZarrSource(OmeSource):
     """Zarr-compatible image source"""
 
     filename: str
     """original filename / URL"""
```

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/conversion.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import os
 import numpy as np
 import zarr
 from PIL import Image
 from imagecodecs.numcodecs import Lzw, Jpeg2k, JpegXr, JpegXl
 from tifffile import TIFF, TiffWriter
 
-from OmeSliCC import Omero
-from OmeSliCC.BioSource import BioSource
-from OmeSliCC.OmeSource import OmeSource, get_resolution_from_pixel_size
-from OmeSliCC.OmeroSource import OmeroSource
-from OmeSliCC.PlainImageSource import PlainImageSource
-from OmeSliCC.TiffSource import TiffSource
-from OmeSliCC.ZarrSource import ZarrSource
-from OmeSliCC.image_util import *
-from OmeSliCC.util import *
+from src.OmeSliCC import Omero
+from src.OmeSliCC.BioSource import BioSource
+from src.OmeSliCC.OmeSource import OmeSource, get_resolution_from_pixel_size
+from src.OmeSliCC.OmeroSource import OmeroSource
+from src.OmeSliCC.PlainImageSource import PlainImageSource
+from src.OmeSliCC.TiffSource import TiffSource
+from src.OmeSliCC.ZarrSource import ZarrSource
+from src.OmeSliCC.image_util import *
+from src.OmeSliCC.util import *
 
 
 def create_source(source_ref: str, params: dict, omero: Omero = None) -> OmeSource:
     source_pixel_size = split_value_unit_list(params['input'].get('pixel_size'))
     target_pixel_size = split_value_unit_list(params['output'].get('pixel_size'))
     ext = os.path.splitext(source_ref)[1].lower()
     if omero is not None:
```

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/image_util.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/image_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import cv2 as cv
 import matplotlib.pyplot as plt
 import tifffile
 from PIL.ExifTags import TAGS
 import imagecodecs
 from tifffile import TiffFile
 
-from OmeSliCC.util import *
+from src.OmeSliCC.util import *
 
 
 # required for auto decoding Zarr
 register_codec(Lzw)
 register_codec(Jpeg2k)
 register_codec(JpegXr)
 register_codec(JpegXl)
```

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/ome.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/ome.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import Ice
 import os
 import omero.gateway
 import omero.model
 import toml
 from uuid import uuid4
 
-from OmeSliCC.image_util import *
-from OmeSliCC.util import *
-from OmeSliCC.XmlDict import dict2xml, XmlDict
+from src.OmeSliCC.image_util import *
+from src.OmeSliCC.util import *
+from src.OmeSliCC.XmlDict import dict2xml, XmlDict
 
 
 name = toml.load("pyproject.toml")["project"]["name"]
 version = toml.load("pyproject.toml")["project"]["version"]
 
 # https://www.openmicroscopy.org/Schemas/Documentation/Generated/OME-2016-06/ome.html
 OME_URI = "http://www.openmicroscopy.org/Schemas/OME/2016-06"
```

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/omero_credentials.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/omero_credentials.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC/util.py` & `OmeSliCC-0.5.1b0/src/OmeSliCC/util.py`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC.egg-info/PKG-INFO` & `OmeSliCC-0.5.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OmeSliCC
-Version: 0.5.1.2
+Version: 0.5.1b0
 Summary: Ome(ro) Slide Image Conversion and Compression pipeline
 Author-email: Joost de Folter <folterj@gmail.com>
 License: # OmeSliCC Licence Agreement
         
         ## OmeSliCC: Ome(ro) SLide Image Conversion and Compression: Software for image conversion including handing both the images and meta-data from Omero.
         
         ©2022, The Francis Crick Institute
```

### Comparing `OmeSliCC-0.5.1.2/OmeSliCC.egg-info/SOURCES.txt` & `OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 LICENSE.md
 README.md
 pyproject.toml
 requirements.txt
-OmeSliCC/BioSource.py
-OmeSliCC/OmeSource.py
-OmeSliCC/Omero.py
-OmeSliCC/OmeroLabelReader.py
-OmeSliCC/OmeroSource.py
-OmeSliCC/PlainImageSource.py
-OmeSliCC/TiffSource.py
-OmeSliCC/XmlDict.py
-OmeSliCC/ZarrSource.py
-OmeSliCC/conversion.py
-OmeSliCC/image_util.py
-OmeSliCC/ome.py
-OmeSliCC/omero_credentials.py
-OmeSliCC/parameters.py
-OmeSliCC/util.py
-OmeSliCC.egg-info/PKG-INFO
-OmeSliCC.egg-info/SOURCES.txt
-OmeSliCC.egg-info/dependency_links.txt
-OmeSliCC.egg-info/requires.txt
-OmeSliCC.egg-info/top_level.txt
-tests/label_reader_test.py
+src/OmeSliCC/BioSource.py
+src/OmeSliCC/OmeSource.py
+src/OmeSliCC/Omero.py
+src/OmeSliCC/OmeroLabelReader.py
+src/OmeSliCC/OmeroSource.py
+src/OmeSliCC/PlainImageSource.py
+src/OmeSliCC/TiffSource.py
+src/OmeSliCC/XmlDict.py
+src/OmeSliCC/ZarrSource.py
+src/OmeSliCC/conversion.py
+src/OmeSliCC/image_util.py
+src/OmeSliCC/ome.py
+src/OmeSliCC/omero_credentials.py
+src/OmeSliCC/parameters.py
+src/OmeSliCC/util.py
+src/OmeSliCC.egg-info/PKG-INFO
+src/OmeSliCC.egg-info/SOURCES.txt
+src/OmeSliCC.egg-info/dependency_links.txt
+src/OmeSliCC.egg-info/requires.txt
+src/OmeSliCC.egg-info/top_level.txt
 tests/test.py
```

### Comparing `OmeSliCC-0.5.1.2/PKG-INFO` & `OmeSliCC-0.5.1b0/src/OmeSliCC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OmeSliCC
-Version: 0.5.1.2
+Version: 0.5.1b0
 Summary: Ome(ro) Slide Image Conversion and Compression pipeline
 Author-email: Joost de Folter <folterj@gmail.com>
 License: # OmeSliCC Licence Agreement
         
         ## OmeSliCC: Ome(ro) SLide Image Conversion and Compression: Software for image conversion including handing both the images and meta-data from Omero.
         
         ©2022, The Francis Crick Institute
```

### Comparing `OmeSliCC-0.5.1.2/README.md` & `OmeSliCC-0.5.1b0/README.md`

 * *Files identical despite different names*

### Comparing `OmeSliCC-0.5.1.2/tests/test.py` & `OmeSliCC-0.5.1b0/tests/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import numpy as np
 import random
 import zarr
 from imageio import imread
 from tqdm import tqdm
 from timeit import default_timer as timer
 
-from OmeSliCC.TiffSource import TiffSource
-from OmeSliCC.image_util import *
+from src.OmeSliCC.TiffSource import TiffSource
+from src.OmeSliCC.image_util import *
 
 
 def test_load(filename: str, pixel_size: list, position: tuple = None, size: tuple = None) -> np.ndarray:
     source = TiffSource(filename, pixel_size)
     if position is None:
         position = (0, 0)
     if size is None:
```

