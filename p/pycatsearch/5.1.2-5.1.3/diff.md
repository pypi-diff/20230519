# Comparing `tmp/pycatsearch-5.1.2.tar.gz` & `tmp/pycatsearch-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatsearch-5.1.2.tar", last modified: Wed May 17 10:44:01 2023, max compression
+gzip compressed data, was "pycatsearch-5.1.3.tar", last modified: Fri May 19 17:57:11 2023, max compression
```

## Comparing `pycatsearch-5.1.2.tar` & `pycatsearch-5.1.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.960428 pycatsearch-5.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.948428 pycatsearch-5.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.952427 pycatsearch-5.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-05-17 10:44:01.960428 pycatsearch-5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:44:01.960428 pycatsearch-5.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.948428 pycatsearch-5.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.952427 pycatsearch-5.1.2/src/pycatsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/async_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/catalog_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.960428 pycatsearch-5.1.2/src/pycatsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/download_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/float_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/frequency_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/menu_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/selectable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/substance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/substances_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/titled_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    37542 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/gui/waiting_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/src/pycatsearch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:44:01.956427 pycatsearch-5.1.2/src/pycatsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 10:44:01.000000 pycatsearch-5.1.2/src/pycatsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-17 10:43:49.000000 pycatsearch-5.1.2/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.452977 pycatsearch-5.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.444977 pycatsearch-5.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.444977 pycatsearch-5.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-05-19 17:57:11.448977 pycatsearch-5.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 17:57:11.452977 pycatsearch-5.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.444977 pycatsearch-5.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.448977 pycatsearch-5.1.3/src/pycatsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/async_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/catalog_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.448977 pycatsearch-5.1.3/src/pycatsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/download_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/float_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/frequency_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/menu_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/selectable_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/substance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/substances_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/titled_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38950 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/waiting_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21042 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.448977 pycatsearch-5.1.3/src/pycatsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/updater.py
```

### Comparing `pycatsearch-5.1.2/.github/workflows/publish-to-pypi.yml` & `pycatsearch-5.1.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/LICENSE.md` & `pycatsearch-5.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/PKG-INFO` & `pycatsearch-5.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.2
+Version: 5.1.3
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
```

### Comparing `pycatsearch-5.1.2/README.md` & `pycatsearch-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/main.py` & `pycatsearch-5.1.3/main.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/pyproject.toml` & `pycatsearch-5.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/setup.py` & `pycatsearch-5.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/__init__.py` & `pycatsearch-5.1.3/src/pycatsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/async_downloader.py` & `pycatsearch-5.1.3/src/pycatsearch/async_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import asyncio
-import json
 import logging
 import random
 from contextlib import suppress
 from math import inf
 from queue import Empty, Queue
 from threading import Thread
 from typing import Any, Final, Mapping, cast
 from urllib.error import HTTPError
 from urllib.parse import urlencode
 
 import aiohttp
 import aiohttp.client_exceptions
 
+try:
+    import orjson as json
+except ImportError:
+    import json
+
 from .catalog_entry import CatalogEntry
 from .utils import *
 
 __all__ = ['Downloader', 'get_catalog', 'save_catalog', 'download']
 
 logger: logging.Logger = logging.getLogger('async_downloader')
 
@@ -223,11 +227,7 @@
     ap.add_argument('-f''max', '--max-frequency', type=float, help='the upper frequency [MHz] to take', default=+inf)
     args: argparse.Namespace = ap.parse_intermixed_args()
 
     logging.basicConfig(level=logging.DEBUG)
     logger.info(f'started at {datetime.now()}')
     save_catalog(args.catalog, (args.min_frequency, args.max_frequency))
     logger.info(f'finished at {datetime.now()}')
-
-
-if __name__ == '__main__':
-    download()
```

### Comparing `pycatsearch-5.1.2/src/pycatsearch/catalog.py` & `pycatsearch-5.1.3/src/pycatsearch/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import bz2
 import gzip
-import json
 import lzma
 import math
 import os.path
 import time
 from contextlib import contextmanager
 from datetime import datetime, timezone
 from os import PathLike
 from pathlib import Path
-from typing import Any, BinaryIO, Callable, Dict, List, NamedTuple, Optional, TextIO, Union, cast
+from typing import Any, AnyStr, BinaryIO, Callable, Dict, List, NamedTuple, Optional, TextIO, Union, cast
+
+try:
+    import orjson as json
+except ImportError:
+    import json
 
 from .utils import *
 
 __all__ = ['Catalog', 'CatalogSourceInfo', 'LineType', 'LinesType', 'CatalogEntryType']
 
 LineType = Dict[str, float]
 LinesType = List[LineType]
@@ -140,15 +144,15 @@
 
     def __init__(self, *catalog_file_names: str) -> None:
         self._data: CatalogData = CatalogData()
         self._sources: list[CatalogSourceInfo] = []
 
         for filename in catalog_file_names:
             if os.path.exists(filename) and os.path.isfile(filename):
-                f_in: BinaryIO | gzip.GzipFile
+                f_in: BinaryIO
                 with Catalog.Opener(filename).open('rb') as f_in:
                     content: bytes = f_in.read()
                     try:
                         json_data: dict[str, list[float | None] | list[CatalogEntryType]] = json.loads(content)
                     except (json.decoder.JSONDecodeError, UnicodeDecodeError):
                         pass
                     else:
@@ -367,10 +371,17 @@
         }
         opener: Catalog.Opener
         try:
             opener = Catalog.Opener(filename)
         except ValueError:
             opener = Catalog.Opener(filename + Catalog.DEFAULT_SUFFIX)
 
+        def ensure_bytes(data: AnyStr) -> bytes:
+            if isinstance(data, str):
+                return data.encode('utf-8')
+            if isinstance(data, bytes):
+                return data
+            raise TypeError('Unknown conversion to bytes')
+
         f: BinaryIO
         with opener.open('wb') as f:
-            f.write(json.dumps(data_to_save, indent=4).encode())
+            f.write(ensure_bytes(json.dumps(data_to_save, indent=4)))
```

### Comparing `pycatsearch-5.1.2/src/pycatsearch/catalog_entry.py` & `pycatsearch-5.1.3/src/pycatsearch/catalog_entry.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/downloader.py` & `pycatsearch-5.1.3/src/pycatsearch/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
-import json
 import logging
 import random
 import time
 from http.client import HTTPConnection, HTTPResponse, HTTPSConnection
 from math import inf
 from queue import Empty, Queue
 from threading import Thread
 from typing import Any, Final, Mapping, cast
 from urllib.error import HTTPError
 from urllib.parse import ParseResult, urlencode, urlparse
 
+try:
+    import orjson as json
+except ImportError:
+    import json
+
 from .catalog_entry import CatalogEntry
 from .utils import *
 
 __all__ = ['Downloader', 'get_catalog', 'save_catalog', 'download']
 
 logger: logging.Logger = logging.getLogger('downloader')
 
@@ -233,11 +237,7 @@
     ap.add_argument('-f''max', '--max-frequency', type=float, help='the upper frequency [MHz] to take', default=+inf)
     args: argparse.Namespace = ap.parse_intermixed_args()
 
     logging.basicConfig(level=logging.DEBUG)
     logger.info(f'started at {datetime.now()}')
     save_catalog(args.catalog, (args.min_frequency, args.max_frequency))
     logger.info(f'finished at {datetime.now()}')
-
-
-if __name__ == '__main__':
-    download()
```

### Comparing `pycatsearch-5.1.2/src/pycatsearch/gui/catalog_info.py` & `pycatsearch-5.1.3/src/pycatsearch/gui/catalog_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/gui/download_dialog.py` & `pycatsearch-5.1.3/src/pycatsearch/gui/download_dialog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/gui/float_spinbox.py` & `pycatsearch-5.1.3/src/pycatsearch/gui/float_spinbox.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/gui/frequency_box.py` & `pycatsearch-5.1.3/src/pycatsearch/gui/frequency_box.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/gui/menu_bar.py` & `pycatsearch-5.1.3/src/pycatsearch/gui/menu_bar.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/gui/preferences.py` & `pycatsearch-5.1.3/src/pycatsearch/gui/preferences.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/gui/settings.py` & `pycatsearch-5.1.3/src/pycatsearch/gui/settings.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/gui/substance_info.py` & `pycatsearch-5.1.3/src/pycatsearch/gui/substance_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/gui/substances_box.py` & `pycatsearch-5.1.3/src/pycatsearch/gui/substances_box.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/gui/titled_list_widget.py` & `pycatsearch-5.1.3/src/pycatsearch/gui/titled_list_widget.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/gui/ui.py` & `pycatsearch-5.1.3/src/pycatsearch/gui/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import math
-from typing import Any, Final, NamedTuple
+from typing import Any, Callable, Final
 
 from qtpy.QtCore import QAbstractTableModel, QMimeData, QModelIndex, QPoint, QPointF, QRect, QSize, Qt
 from qtpy.QtGui import (QAbstractTextDocumentLayout, QClipboard, QCloseEvent, QCursor, QIcon, QPainter, QPixmap,
                         QScreen, QTextDocument)
 from qtpy.QtWidgets import (QAbstractItemView, QAbstractSpinBox, QApplication, QDoubleSpinBox, QFormLayout, QGridLayout,
                             QHeaderView, QMainWindow, QMessageBox, QPushButton, QStatusBar, QStyle,
                             QStyleOptionViewItem, QStyledItemDelegate, QTableView, QTableWidgetSelectionRange, QWidget)
@@ -18,15 +18,15 @@
 from .frequency_box import FrequencyBox
 from .menu_bar import MenuBar
 from .preferences import Preferences
 from .settings import Settings
 from .substance_info import SubstanceInfo
 from .substances_box import SubstancesBox
 from .. import __version__
-from ..catalog import Catalog, CatalogEntryType, LineType
+from ..catalog import Catalog, CatalogEntryType
 from ..utils import *
 
 __all__ = ['UI']
 
 
 def copy_to_clipboard(text: str, text_type: Qt.TextFormat | str = Qt.TextFormat.PlainText) -> None:
     clipboard: QClipboard = QApplication.clipboard()
@@ -84,23 +84,42 @@
         doc.setTextWidth(options.rect.width())
         return QSize(round(doc.idealWidth()), round(doc.size().height()))
 
 
 class LinesListModel(QAbstractTableModel):
     ROW_BATCH_COUNT: Final[int] = 5
 
-    class DataType(NamedTuple):
-        id: int
-        best_name: str
-        frequency_str: str
-        frequency: float
-        intensity_str: str
-        intensity: float
-        lower_state_energy_str: str
-        lower_state_energy: float
+    class DataType:
+        __slots__ = ['id', 'name',
+                     'frequency_str', 'frequency',
+                     'intensity_str', 'intensity',
+                     'lower_state_energy_str', 'lower_state_energy']
+
+        def __init__(self,
+                     species_id: int, name: str,
+                     frequency_str: str, frequency: float,
+                     intensity_str: str, intensity: float,
+                     lower_state_energy_str: str, lower_state_energy: float) -> None:
+            self.id: int = species_id
+            self.name: str = name
+            self.frequency_str: str = frequency_str
+            self.frequency: float = frequency
+            self.intensity_str: str = intensity_str
+            self.intensity: float = intensity
+            self.lower_state_energy_str: str = lower_state_energy_str
+            self.lower_state_energy: float = lower_state_energy
+
+        def __eq__(self, other: LinesListModel.DataType) -> int:
+            return (self.id == other.id
+                    and self.frequency == other.frequency
+                    and self.intensity == other.intensity
+                    and self.lower_state_energy == other.lower_state_energy)
+
+        def __hash__(self) -> int:
+            return hash(self.id) ^ hash(self.frequency) ^ hash(self.lower_state_energy)
 
     def __init__(self, settings: Settings, parent: QWidget | None = None) -> None:
         super().__init__(parent)
         self._settings: Settings = settings
         self._entries: list[CatalogEntryType] = []
         self._data: list[LinesListModel.DataType] = []
         self._rows_loaded: int = LinesListModel.ROW_BATCH_COUNT
@@ -121,31 +140,32 @@
 
     def rowCount(self, parent: QModelIndex = ...) -> int:
         return min(len(self._data), self._rows_loaded)
 
     def columnCount(self, parent: QModelIndex = ...) -> int:
         return len(self._header)
 
-    def data(self, index: QModelIndex, role: int = Qt.ItemDataRole.DisplayRole) -> int | str | float | None:
+    def data(self, index: QModelIndex, role: int = Qt.ItemDataRole.DisplayRole) -> str | None:
         if index.isValid():
             if role == Qt.ItemDataRole.DisplayRole:
-                data_column: Final[int] = {0: 1, 1: 2, 2: 4, 3: 6}[index.column()]
-                return self._data[index.row()][data_column]
+                item: LinesListModel.DataType = self._data[index.row()]
+                column_index: int = index.column()
+                if column_index == 0:
+                    return item.name
+                if column_index == 1:
+                    return item.frequency_str
+                if column_index == 2:
+                    return item.intensity_str
+                if column_index == 3:
+                    return item.lower_state_energy_str
         return None
 
     def row(self, row_index: int) -> LinesListModel.DataType:
         return self._data[row_index]
 
-    def item(self, row_index: int, column_index: int) -> int | str | float:
-        data_column: Final[int] = {0: 1, 1: 2, 2: 4, 3: 6}[column_index]
-        return self._data[row_index][data_column]
-
-    def raw_item(self, row_index: int, column_index: int) -> int | str | float:
-        return self._data[row_index][column_index]
-
     def headerData(self, col: int, orientation: Qt.Orientation, role: int = ...) -> str | None:
         if orientation == Qt.Orientation.Horizontal and role == Qt.ItemDataRole.DisplayRole:
             return self._header[col]
         return None
 
     def setHeaderData(self, section: int, orientation: Qt.Orientation, value: str, role: int = ...) -> bool:
         if (orientation == Qt.Orientation.Horizontal
@@ -155,83 +175,90 @@
             return True
         return False
 
     def clear(self) -> None:
         self.set_entries([])
 
     def set_entries(self, new_data: list[CatalogEntryType]) -> None:
-        def frequency_str(line: LineType) -> tuple[str, float]:
-            frequency: float = self._settings.from_mhz(line[FREQUENCY])
-            frequency_suffix: int = self._settings.frequency_unit
-            precision: int = [4, 7, 8, 8][frequency_suffix]
+        from_mhz: Callable[[float], float] = self._settings.from_mhz
+        from_log10_sq_nm_mhz: Callable[[float], float] = self._settings.from_log10_sq_nm_mhz
+        from_rec_cm: Callable[[float], float] = self._settings.from_rec_cm
+        frequency_suffix: int = self._settings.frequency_unit
+        precision: int = [4, 7, 8, 8][frequency_suffix]
+
+        def frequency_str(frequency: float) -> tuple[str, float]:
+            frequency = from_mhz(frequency)
             return f'{frequency:.{precision}f}', frequency
 
-        def intensity_str(line: LineType) -> tuple[str, float]:
-            intensity: float = self._settings.from_log10_sq_nm_mhz(line[INTENSITY])
+        def intensity_str(intensity: float) -> tuple[str, float]:
+            intensity = from_log10_sq_nm_mhz(intensity)
             if intensity == 0.0:
                 return '0', intensity
             elif abs(intensity) < 0.1:
                 return f'{intensity:.4e}', intensity
             else:
                 return f'{intensity:.4f}', intensity
 
-        def lower_state_energy_str(line: LineType) -> tuple[str, float]:
-            lower_state_energy: float = self._settings.from_rec_cm(line[LOWER_STATE_ENERGY])
+        def lower_state_energy_str(lower_state_energy: float) -> tuple[str, float]:
+            lower_state_energy = from_rec_cm(lower_state_energy)
             if lower_state_energy == 0.0:
                 return '0', lower_state_energy
             elif abs(lower_state_energy) < 0.1:
                 return f'{lower_state_energy:.4e}', lower_state_energy
             else:
                 return f'{lower_state_energy:.4f}', lower_state_energy
 
-        def same_entry(entry_1: CatalogEntryType, entry_2: CatalogEntryType) -> bool:
-            if len(entry_1) != len(entry_2):
-                return False
-            for key, value in entry_1.items():
-                if key not in entry_2:
-                    return False
-                if key != LINES and value != entry_2[key]:
-                    return False
-                if key == LINES and len(value) != len(entry_2[key]):
-                    return False
-            return True
-
         self.beginResetModel()
-        unique_entries = new_data.copy()
+        unique_entries: list[CatalogEntryType] = []
+        non_unique_indices: set[int] = set()
+        unique: bool
         all_unique: bool = True  # unless the opposite is proven
         for i in range(len(new_data)):
-            unique: bool = True
+            if i in non_unique_indices:
+                continue
+            unique = True
             for j in range(i + 1, len(new_data)):
-                if same_entry(new_data[i], new_data[j]):
+                if j in non_unique_indices:
+                    continue
+                if new_data[i] == new_data[j]:
+                    non_unique_indices.add(j)
                     unique = False
-                    if all_unique:
-                        unique_entries = []
-                        all_unique = False
+                    all_unique = False
+                    break
             if unique and not all_unique:
                 unique_entries.append(new_data[i])
-        self._entries = unique_entries
+        if all_unique:
+            self._entries = new_data.copy()
+        else:
+            self._entries = unique_entries
         entry: CatalogEntryType
-        self._data = [
+        rich_text_in_formulas: bool = self._settings.rich_text_in_formulas
+        self._data = list(set(
             LinesListModel.DataType(
                 entry[ID],
-                best_name(entry, self._settings.rich_text_in_formulas),
-                *frequency_str(line),
-                *intensity_str(line),
-                *lower_state_energy_str(line),
+                best_name(entry, rich_text_in_formulas),
+                *frequency_str(line[FREQUENCY]),
+                *intensity_str(line[INTENSITY]),
+                *lower_state_energy_str(line[LOWER_STATE_ENERGY]),
             )
             for entry in self._entries
             for line in entry[LINES]
-        ]
+        ))
         self._rows_loaded = LinesListModel.ROW_BATCH_COUNT
         self.endResetModel()
 
     def sort(self, column: int, order: Qt.SortOrder = Qt.SortOrder.AscendingOrder) -> None:
         self.beginResetModel()
-        data_column: Final[int] = {0: 1, 1: 3, 2: 5, 3: 7}[column]
-        self._data.sort(key=lambda l: l[data_column], reverse=bool(order != Qt.SortOrder.AscendingOrder))
+        key = {
+            0: (lambda l: (l.name, l.frequency, l.intensity, l.lower_state_energy)),
+            1: (lambda l: (l.frequency, l.intensity, l.name, l.lower_state_energy)),
+            2: (lambda l: (l.intensity, l.frequency, l.name, l.lower_state_energy)),
+            3: (lambda l: (l.lower_state_energy, l.intensity, l.frequency, l.name))
+        }[column]
+        self._data.sort(key=key, reverse=bool(order != Qt.SortOrder.AscendingOrder))
         self.endResetModel()
 
     def canFetchMore(self, index: QModelIndex = QModelIndex()) -> bool:
         return len(self._data) > self._rows_loaded
 
     def fetchMore(self, index: QModelIndex = QModelIndex()) -> None:
         # https://sateeshkumarb.wordpress.com/2012/04/01/paginated-display-of-table-data-in-pyqt/
@@ -498,18 +525,18 @@
             3: self.settings.energy_unit_str,
         }
         for r in self.results_table.selectionModel().selectedRows():
             row: LinesListModel.DataType = self.results_model.row(r.row())
             text.append(
                 '<tr><td>' +
                 f'</td>{self.settings.csv_separator}<td>'.join(
-                    [row.best_name] +
-                    [(str(row[_c * 2]) + ((' ' + units[_c]) if self.settings.with_units and _c in units else ''))
-                     for _c, _a in zip(range(1, self.results_model.columnCount()),
-                                       self.menu_bar.menu_columns.actions())
+                    [row.name] +
+                    [(str(_c) + ((' ' + units[_i]) if self.settings.with_units and _i in units else ''))
+                     for _i, (_c, _a) in enumerate(zip((row.frequency, row.intensity, row.lower_state_energy),
+                                                       self.menu_bar.menu_columns.actions()))
                      if _a.isChecked()]
                 ) +
                 '</td></tr>' + self.settings.line_end
             )
         return '<table>' + self.settings.line_end + ''.join(text) + '</table>'
 
     def on_action_download_catalog_triggered(self) -> None:
```

### Comparing `pycatsearch-5.1.2/src/pycatsearch/gui/waiting_screen.py` & `pycatsearch-5.1.3/src/pycatsearch/gui/waiting_screen.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/src/pycatsearch/utils.py` & `pycatsearch-5.1.3/src/pycatsearch/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,44 +461,60 @@
     """ Basic check that all tags are sound """
     _1, _2, _3 = text.count('<'), text.count('>'), 2 * text.count('</')
     return _1 == _2 and _1 == _3
 
 
 def best_name(entry: dict[str, int | str | list[dict[str, float]]],
               allow_html: bool = True) -> str:
-    if allow_html and ISOTOPOLOG in entry and entry[ISOTOPOLOG]:
-        if allow_html:
-            if (is_good_html(str(entry[MOLECULE_SYMBOL]))
-                    and ((STRUCTURAL_FORMULA in entry and entry[STRUCTURAL_FORMULA] == entry[ISOTOPOLOG])
-                         or (STOICHIOMETRIC_FORMULA in entry and entry[STOICHIOMETRIC_FORMULA] == entry[ISOTOPOLOG]))):
-                if STATE_HTML in entry and entry[STATE_HTML]:
-                    # span tags are needed when the molecule symbol is malformed
-                    return f'<span>{entry[MOLECULE_SYMBOL]}</span>, ' \
-                           f'{chem_html(tex_to_html_entity(str(entry[STATE_HTML])))}'
-                return str(entry[MOLECULE_SYMBOL])
+    last: str = best_name.__dict__.get('last', dict()).get(entry[SPECIES_TAG], dict()).get(allow_html, '')
+    if last:
+        return last
+
+    def _best_name() -> str:
+        if allow_html and ISOTOPOLOG in entry and entry[ISOTOPOLOG]:
+            if allow_html:
+                if (is_good_html(str(entry[MOLECULE_SYMBOL]))
+                        and ((STRUCTURAL_FORMULA in entry and entry[STRUCTURAL_FORMULA] == entry[ISOTOPOLOG])
+                             or (STOICHIOMETRIC_FORMULA in entry
+                                 and entry[STOICHIOMETRIC_FORMULA] == entry[ISOTOPOLOG]))):
+                    if STATE_HTML in entry and entry[STATE_HTML]:
+                        # span tags are needed when the molecule symbol is malformed
+                        return f'<span>{entry[MOLECULE_SYMBOL]}</span>, ' \
+                               f'{chem_html(tex_to_html_entity(str(entry[STATE_HTML])))}'
+                    return str(entry[MOLECULE_SYMBOL])
+                else:
+                    if STATE_HTML in entry and entry[STATE_HTML]:
+                        return f'{chem_html(str(entry[ISOTOPOLOG]))}, ' \
+                               f'{chem_html(tex_to_html_entity(str(entry[STATE_HTML])))}'
+                    return chem_html(str(entry[ISOTOPOLOG]))
             else:
                 if STATE_HTML in entry and entry[STATE_HTML]:
-                    return f'{chem_html(str(entry[ISOTOPOLOG]))}, ' \
-                           f'{chem_html(tex_to_html_entity(str(entry[STATE_HTML])))}'
-                return chem_html(str(entry[ISOTOPOLOG]))
-        else:
-            if STATE_HTML in entry and entry[STATE_HTML]:
-                return f'{entry[ISOTOPOLOG]}, {remove_html(tex_to_html_entity(entry[STATE_HTML]))}'
-            if STATE in entry and entry[STATE]:
-                return f'{entry[ISOTOPOLOG]}, {remove_html(tex_to_html_entity(entry[STATE].strip("$")))}'
-            return entry[ISOTOPOLOG]
-
-    for key in (NAME, STRUCTURAL_FORMULA, STOICHIOMETRIC_FORMULA):
-        if key in entry and entry[key]:
-            return chem_html(str(entry[key])) if allow_html else str(entry[key])
-    if TRIVIAL_NAME in entry and entry[TRIVIAL_NAME]:
-        return str(entry[TRIVIAL_NAME])
-    if SPECIES_TAG in entry and entry[SPECIES_TAG]:
-        return str(entry[SPECIES_TAG])
-    return 'no name'
+                    return f'{entry[ISOTOPOLOG]}, {remove_html(tex_to_html_entity(entry[STATE_HTML]))}'
+                if STATE in entry and entry[STATE]:
+                    return f'{entry[ISOTOPOLOG]}, {remove_html(tex_to_html_entity(entry[STATE].strip("$")))}'
+                return entry[ISOTOPOLOG]
+
+        for key in (NAME, STRUCTURAL_FORMULA, STOICHIOMETRIC_FORMULA):
+            if key in entry and entry[key]:
+                return chem_html(str(entry[key])) if allow_html else str(entry[key])
+        if TRIVIAL_NAME in entry and entry[TRIVIAL_NAME]:
+            return str(entry[TRIVIAL_NAME])
+        if SPECIES_TAG in entry and entry[SPECIES_TAG]:
+            return str(entry[SPECIES_TAG])
+        return 'no name'
+
+    res: str = _best_name()
+    if SPECIES_TAG not in entry:
+        return res
+    if 'last' not in best_name.__dict__:
+        best_name.__dict__['last'] = dict()
+    if entry[SPECIES_TAG] not in best_name.__dict__['last']:
+        best_name.__dict__['last'][entry[SPECIES_TAG]] = dict()
+    best_name.__dict__['last'][entry[SPECIES_TAG]][allow_html] = res
+    return res
 
 
 def remove_html(line: str) -> str:
     """ removes HTML tags and decodes HTML entities """
     if not is_good_html(line):
         return html.unescape(line)
```

### Comparing `pycatsearch-5.1.2/src/pycatsearch.egg-info/PKG-INFO` & `pycatsearch-5.1.3/src/pycatsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.2
+Version: 5.1.3
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
```

### Comparing `pycatsearch-5.1.2/src/pycatsearch.egg-info/SOURCES.txt` & `pycatsearch-5.1.3/src/pycatsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.2/updater.py` & `pycatsearch-5.1.3/updater.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import logging
+import subprocess
 import sys
 import urllib.request
 from contextlib import suppress
 from datetime import datetime
 from http.client import HTTPResponse
 from pathlib import Path
-from subprocess import PIPE, Popen, check_call
 
 __all__ = ['update_from_github', 'update_with_git', 'update_with_pip']
 
 logger: logging.Logger = logging.getLogger('updater')
 
 
 def from_iso_format(s: str) -> datetime:
@@ -93,17 +93,15 @@
     return True
 
 
 def update_with_git() -> bool:
     with suppress(Exception):
         code_directory: Path = Path(__file__).parent
         if (code_directory / '.git').exists():
-            p: Popen
-            with Popen(args=['git', 'pull']) as p:
-                return p.returncode == 0
+            return subprocess.run(args=['git', 'pull'], capture_output=True).returncode == 0
     return False
 
 
 def update_from_github(user: str, repo_name: str, branch: str = 'master') -> bool:
     with suppress(Exception):
         code_directory: Path = Path(__file__).parent
         version_path: Path = code_directory / 'src' / repo_name / '_version.py'
@@ -144,52 +142,53 @@
         offset = 0
         for col, title in zip(cols, titles):
             data[-1][title] = text_lines[line_no][offset:(offset + col)].strip()
             offset += col + 1
     return data
 
 
-def update_package(package_name: str) -> tuple[str, str]:
-    p: Popen
-    with Popen(args=[sys.executable, '-m', 'pip', 'install', '--user', '-U', package_name],
-               stdout=PIPE, stderr=PIPE, text=True) as p:
-        err: str = p.stderr.read()
-        return p.stdout.read(), err
+def update_package(package_name: str) -> tuple[str, str, int | None]:
+    p: subprocess.CompletedProcess = subprocess.run(
+        args=[sys.executable, '-m', 'pip', 'install', '-U', package_name],
+        capture_output=True, text=True)
+    return p.stdout, p.stderr, p.returncode
 
 
 def update_packages() -> list[str]:
     priority_packages: list[str] = ['pip', 'setuptools', 'wheel']
+    out: str
     err: str
-    p: Popen
-    with Popen(args=[sys.executable, '-m', 'pip', 'list', '--outdated'], stdout=PIPE, stderr=PIPE, text=True) as p:
-        err = p.stderr.read()
-        if err:
-            return []
-        outdated_packages: list[str] = [item['Package'] for item in parse_table(p.stdout.read())]
+    ret: int | None
+    p: subprocess.CompletedProcess = subprocess.run(
+        args=[sys.executable, '-m', 'pip', 'list', '--outdated'],
+        capture_output=True, text=True)
+    if p.returncode:
+        return []
+    outdated_packages: list[str] = [item['Package'] for item in parse_table(p.stdout)]
     updated_packages: list[str] = []
     try:
         for pp in priority_packages:
             if pp in outdated_packages:
-                out, err = update_package(pp)
-                if err:
-                    return []
+                out, err, ret = update_package(pp)
+                if ret:
+                    return updated_packages
                 outdated_packages.remove(pp)
                 updated_packages.append(pp)
         for op in outdated_packages:
             update_package(op)
             updated_packages.append(op)
     finally:
         return updated_packages
 
 
 def update_with_pip(package_name: str) -> bool:
     with suppress(Exception):
         if package_name not in update_packages():
-            out, err = update_package(package_name)
-            return not err
+            out, err, ret = update_package(package_name)
+            return not ret
     return False
 
 
 if __name__ == '__main__':
     import argparse
 
     ap: argparse.ArgumentParser = argparse.ArgumentParser(
```

