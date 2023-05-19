# Comparing `tmp/calitp_map_utils-2023.5.19.3.tar.gz` & `tmp/calitp_map_utils-2023.5.19.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_map_utils-2023.5.19.3.tar", max compression
+gzip compressed data, was "calitp_map_utils-2023.5.19.4.tar", max compression
```

## Comparing `calitp_map_utils-2023.5.19.3.tar` & `calitp_map_utils-2023.5.19.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      944 2023-05-18 19:13:08.501349 calitp_map_utils-2023.5.19.3/README.md
--rw-r--r--   0        0        0     3744 2023-05-19 14:49:58.954976 calitp_map_utils-2023.5.19.3/calitp_map_utils/__init__.py
--rw-r--r--   0        0        0      647 2023-05-19 14:49:59.217026 calitp_map_utils-2023.5.19.3/calitp_map_utils/__main__.py
--rw-r--r--   0        0        0      591 2023-05-19 15:21:16.445788 calitp_map_utils-2023.5.19.3/pyproject.toml
--rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 calitp_map_utils-2023.5.19.3/PKG-INFO
+-rw-r--r--   0        0        0      944 2023-05-18 19:13:08.501349 calitp_map_utils-2023.5.19.4/README.md
+-rw-r--r--   0        0        0     3124 2023-05-19 17:09:53.889476 calitp_map_utils-2023.5.19.4/calitp_map_utils/__init__.py
+-rw-r--r--   0        0        0     1355 2023-05-19 16:46:58.152408 calitp_map_utils-2023.5.19.4/calitp_map_utils/__main__.py
+-rw-r--r--   0        0        0      609 2023-05-19 17:10:46.903789 calitp_map_utils-2023.5.19.4/pyproject.toml
+-rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 calitp_map_utils-2023.5.19.4/PKG-INFO
```

### Comparing `calitp_map_utils-2023.5.19.3/README.md` & `calitp_map_utils-2023.5.19.4/README.md`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.5.19.3/calitp_map_utils/__init__.py` & `calitp_map_utils-2023.5.19.4/calitp_map_utils/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-import base64
 import gzip
 import json
-import sys
 from enum import Enum
 from typing import Optional, Tuple, Union
 
 import requests
 import typer
 import urllib3
 from calitp_data.storage import get_fs  # type: ignore
 from geojson_pydantic import Feature, FeatureCollection, MultiPolygon, Point, Polygon
 from geojson_pydantic.types import Position
 from pydantic import BaseModel, HttpUrl, ValidationError, root_validator
 from tqdm import tqdm
 
 
-# Any positions in this are flipped;
-class State(BaseModel):
-    name: str
-    url: HttpUrl
-    lat_lon: Optional[Position]
-    zoom: Optional[int]
-    bbox: Optional[Tuple[Position, Position]]
+class Analysis(str, Enum):
+    speedmaps = "speedmap"
+    hqta_areas = "hqta_areas"
+    hqta_stops = "hqta_stops"
 
 
 class Speedmap(BaseModel):
     stop_id: Optional[str]
     stop_name: Optional[str]
     route_id: Optional[str]
 
@@ -37,30 +32,25 @@
 
 class HQTA(BaseModel):
     hqta_type: str
     agency_name_primary: str
     agency_name_secondary: Optional[str]
 
 
-class Analysis(str, Enum):
-    speedmaps = "speedmap"
-    hqta_areas = "hqta_areas"
-    hqta_stops = "hqta_stops"
-
-
 # Dict Props just mean properties are an arbitrary dictionary
 ANALYSIS_FEATURE_TYPES = {
     Analysis.speedmaps: Feature[Polygon, Speedmap],
     Analysis.hqta_areas: Feature[Union[Polygon, MultiPolygon], HQTA],
     Analysis.hqta_stops: Feature[Point, HQTA],
 }
 
 
-def validate_geojson(path: str, analysis: Optional[Analysis] = None):
-    typer.secho(f"Validating {path}...", fg=typer.colors.MAGENTA)
+def validate_geojson(path: str, analysis: Optional[Analysis] = None, verbose=False):
+    if verbose:
+        typer.secho(f"Validating {path}...", fg=typer.colors.MAGENTA)
 
     is_compressed = path.endswith(".gz")
 
     if path.startswith("https://"):
         resp = requests.get(path)
         resp.raise_for_status()
         d = json.loads(
@@ -74,56 +64,40 @@
                 f = gzip.GzipFile(fileobj=f)
             d = json.load(f)
 
     collection = FeatureCollection(**d)
 
     if analysis:
         analysis_class = ANALYSIS_FEATURE_TYPES[analysis]
-        typer.secho(f"Validating that features are {analysis_class}...")
+        if verbose:
+            typer.secho(f"Validating that features are {analysis_class}...")
         for feature in tqdm(collection.features):
             try:
                 analysis_class(**feature.dict())
             except ValidationError:
                 typer.secho(feature.json(), fg=typer.colors.RED)
                 raise
 
-    typer.secho(
-        f"Success! Validated {len(collection.features)} features.",
-        fg=typer.colors.GREEN,
-    )
-
-
-def validate_state(
-    infile: Optional[str] = None,
-    base64url: bool = False,
-    compressed: bool = False,
-    analysis: Optional[Analysis] = None,
-):
-    if infile:
-        typer.secho(f"Reading {infile}.", fg=typer.colors.MAGENTA)
-        with open(infile) as f:
-            contents = f.read()
-    else:
-        typer.secho("Reading from stdin...", fg=typer.colors.MAGENTA)
-        contents = sys.stdin.read()
-
-    if base64url:
-        typer.secho("Decoding base64 contents...", fg=typer.colors.MAGENTA)
-        byts = base64.urlsafe_b64decode(contents.encode())
-
-        if compressed:
-            byts = gzip.decompress(byts)
-
-        contents = byts.decode()
-
-    state = State(**json.loads(contents))
-    typer.secho(f"Checking that {state.url} exists...", fg=typer.colors.MAGENTA)
-    resp = urllib3.request("HEAD", state.url)  # type: ignore[operator]
 
-    if resp.status != 200:
-        typer.secho(f"Failed to find file at {state.url}.", fg=typer.colors.RED)
-        raise typer.Exit(1)
+# Any positions in this are flipped from typical geojson
+# leaflet wants lat/lon
+class State(BaseModel):
+    name: str
+    url: HttpUrl
+    lat_lon: Optional[Position]
+    zoom: Optional[int]
+    bbox: Optional[Tuple[Position, Position]]
+    analysis: Optional[Analysis]
 
-    if analysis:
-        validate_geojson(state.url, analysis)
+    def validate(self, data: bool = False, verbose: bool = False):
+        if verbose:
+            typer.secho(f"Checking that {self.url} exists...", fg=typer.colors.MAGENTA)
+        resp = urllib3.request("HEAD", self.url)  # type: ignore[operator]
+
+        if resp.status != 200:
+            msg = f"Failed to find file at {self.url}"
+            if verbose:
+                typer.secho(msg, fg=typer.colors.RED)
+            raise FileNotFoundError(msg)
 
-    typer.secho("Validation successful!", fg=typer.colors.GREEN)
+        if data:
+            validate_geojson(self.url, self.analysis)
```

### Comparing `calitp_map_utils-2023.5.19.3/pyproject.toml` & `calitp_map_utils-2023.5.19.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calitp_map_utils"
-version = "2023.5.19.3"
+version = "2023.5.19.4"
 description = ""
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.9"
 pyyaml = "^6.0"
@@ -17,11 +17,12 @@
 
 
 [tool.poetry.group.dev.dependencies]
 pydantic-to-typescript = "^1.0.10"
 mypy = "^1.3.0"
 types-tqdm = "^4.65.0.1"
 types-requests = "^2.30.0.0"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `calitp_map_utils-2023.5.19.3/PKG-INFO` & `calitp_map_utils-2023.5.19.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calitp-map-utils
-Version: 2023.5.19.3
+Version: 2023.5.19.4
 Summary: 
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: calitp-data (==2023.2.13.1)
```

