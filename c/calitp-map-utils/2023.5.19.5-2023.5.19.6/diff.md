# Comparing `tmp/calitp_map_utils-2023.5.19.5.tar.gz` & `tmp/calitp_map_utils-2023.5.19.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_map_utils-2023.5.19.5.tar", max compression
+gzip compressed data, was "calitp_map_utils-2023.5.19.6.tar", max compression
```

## Comparing `calitp_map_utils-2023.5.19.5.tar` & `calitp_map_utils-2023.5.19.6.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      944 2023-05-18 19:13:08.501349 calitp_map_utils-2023.5.19.5/README.md
--rw-r--r--   0        0        0     3128 2023-05-19 17:13:42.921804 calitp_map_utils-2023.5.19.5/calitp_map_utils/__init__.py
--rw-r--r--   0        0        0     1355 2023-05-19 16:46:58.152408 calitp_map_utils-2023.5.19.5/calitp_map_utils/__main__.py
--rw-r--r--   0        0        0      632 2023-05-19 17:18:51.273585 calitp_map_utils-2023.5.19.5/pyproject.toml
--rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 calitp_map_utils-2023.5.19.5/PKG-INFO
+-rw-r--r--   0        0        0      944 2023-05-18 19:13:08.501349 calitp_map_utils-2023.5.19.6/README.md
+-rw-r--r--   0        0        0     3414 2023-05-19 17:43:02.079326 calitp_map_utils-2023.5.19.6/calitp_map_utils/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-19 17:31:40.764053 calitp_map_utils-2023.5.19.6/calitp_map_utils/__main__.py
+-rw-r--r--   0        0        0     1321 2023-05-19 17:39:43.981472 calitp_map_utils-2023.5.19.6/calitp_map_utils/cli.py
+-rw-r--r--   0        0        0      632 2023-05-19 17:45:19.115916 calitp_map_utils-2023.5.19.6/pyproject.toml
+-rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 calitp_map_utils-2023.5.19.6/PKG-INFO
```

### Comparing `calitp_map_utils-2023.5.19.5/README.md` & `calitp_map_utils-2023.5.19.6/README.md`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.5.19.5/calitp_map_utils/__init__.py` & `calitp_map_utils-2023.5.19.6/calitp_map_utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,17 +40,19 @@
 ANALYSIS_FEATURE_TYPES = {
     Analysis.speedmaps: Feature[Polygon, Speedmap],
     Analysis.hqta_areas: Feature[Union[Polygon, MultiPolygon], HQTA],
     Analysis.hqta_stops: Feature[Point, HQTA],
 }
 
 
-def validate_geojson(path: str, analysis: Optional[Analysis] = None, verbose=False):
+def validate_geojson(
+    path: str, analysis: Optional[Analysis] = None, verbose=False
+) -> FeatureCollection:
     if verbose:
-        typer.secho(f"Validating {path}...", fg=typer.colors.MAGENTA)
+        typer.secho(f"Validating {typer.style(path, fg=typer.colors.CYAN)} contents...")
 
     is_compressed = path.endswith(".gz")
 
     if path.startswith("https://"):
         resp = requests.get(path)
         resp.raise_for_status()
         d = json.loads(
@@ -65,39 +67,50 @@
             d = json.load(f)
 
     collection = FeatureCollection(**d)
 
     if analysis:
         analysis_class = ANALYSIS_FEATURE_TYPES[analysis]
         if verbose:
-            typer.secho(f"Validating that features are {analysis_class}...")
+            typer.secho(
+                f"Validating that features are {typer.style(str(analysis_class), fg=typer.colors.YELLOW)}..."
+            )
         for feature in tqdm(collection.features):
             try:
                 analysis_class(**feature.dict())
             except ValidationError:
                 typer.secho(feature.json(), fg=typer.colors.RED)
                 raise
 
+    return collection
+
 
 # Any positions in this are flipped from typical geojson
 # leaflet wants lat/lon
 class State(BaseModel):
     name: str
     url: HttpUrl
     lat_lon: Optional[Position]
     zoom: Optional[int]
     bbox: Optional[Tuple[Position, Position]]
     analysis: Optional[Analysis]
 
-    def validate_url(self, data: bool = False, verbose: bool = False):
+    def validate_url(
+        self,
+        data: bool = False,
+        verbose: bool = False,
+        analysis: Optional[Analysis] = None,
+    ):
         if verbose:
-            typer.secho(f"Checking that {self.url} exists...", fg=typer.colors.MAGENTA)
+            typer.secho(
+                f"Checking that {typer.style(self.url, fg=typer.colors.CYAN)} exists..."
+            )
         resp = urllib3.request("HEAD", self.url)  # type: ignore[operator]
 
         if resp.status != 200:
             msg = f"Failed to find file at {self.url}"
             if verbose:
                 typer.secho(msg, fg=typer.colors.RED)
             raise FileNotFoundError(msg)
 
         if data:
-            validate_geojson(self.url, self.analysis)
+            validate_geojson(self.url, analysis or self.analysis, verbose=verbose)
```

### Comparing `calitp_map_utils-2023.5.19.5/calitp_map_utils/__main__.py` & `calitp_map_utils-2023.5.19.6/calitp_map_utils/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,52 +4,50 @@
 import sys
 from typing import Optional
 
 import typer
 
 from . import Analysis, State
 from . import validate_geojson as validate_geojson_func
-from . import validate_state as validate_state_func
 
 app = typer.Typer()
 
 
 @app.command()
 def validate_geojson(path: str, analysis: Optional[Analysis] = None):
-    validate_geojson_func(path, analysis, verbose=True)
+    collection = validate_geojson_func(path, analysis, verbose=True)
 
     typer.secho(
         f"Success! Validated {len(collection.features)} features.",
         fg=typer.colors.GREEN,
     )
 
 
 @app.command()
 def validate_state(
     infile: Optional[str] = None,
     base64url: bool = False,
     compressed: bool = False,
+    data: bool = False,
+    verbose: bool = False,
     analysis: Optional[Analysis] = None,
 ):
     if infile:
-        typer.secho(f"Reading {infile}.", fg=typer.colors.MAGENTA)
+        typer.secho(f"Reading {infile}.")
         with open(infile) as f:
             contents = f.read()
     else:
-        typer.secho("Reading from stdin...", fg=typer.colors.MAGENTA)
+        typer.secho("Reading from stdin...")
         contents = sys.stdin.read()
 
     if base64url:
-        typer.secho("Decoding base64 contents...", fg=typer.colors.MAGENTA)
+        typer.secho("Decoding base64 contents...")
         byts = base64.urlsafe_b64decode(contents.encode())
 
         if compressed:
             byts = gzip.decompress(byts)
 
         contents = byts.decode()
 
     state = State(**json.loads(contents))
-    state.validate(verbose=True)
+    state.validate_url(verbose=verbose, data=data, analysis=analysis)
     typer.secho("Validation successful!", fg=typer.colors.GREEN)
-
-
-app()
```

### Comparing `calitp_map_utils-2023.5.19.5/pyproject.toml` & `calitp_map_utils-2023.5.19.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calitp_map_utils"
-version = "2023.5.19.5"
+version = "2023.5.19.6"
 description = ""
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.9"
 pyyaml = "^6.0"
```

### Comparing `calitp_map_utils-2023.5.19.5/PKG-INFO` & `calitp_map_utils-2023.5.19.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calitp-map-utils
-Version: 2023.5.19.5
+Version: 2023.5.19.6
 Summary: 
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: calitp-data (==2023.2.13.1)
```

