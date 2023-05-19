# Comparing `tmp/xyzservices-2023.2.0.tar.gz` & `tmp/xyzservices-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyzservices-2023.2.0.tar", last modified: Sun Feb 19 14:01:44 2023, max compression
+gzip compressed data, was "xyzservices-2023.5.0.tar", last modified: Fri May 19 20:50:17 2023, max compression
```

## Comparing `xyzservices-2023.2.0.tar` & `xyzservices-2023.5.0.tar`

### file list

```diff
@@ -1,25 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 14:01:44.202255 xyzservices-2023.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-02-19 14:01:39.000000 xyzservices-2023.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-19 14:01:39.000000 xyzservices-2023.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-02-19 14:01:44.202255 xyzservices-2023.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-02-19 14:01:39.000000 xyzservices-2023.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-19 14:01:44.202255 xyzservices-2023.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-19 14:01:39.000000 xyzservices-2023.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    70142 2023-02-19 14:01:39.000000 xyzservices-2023.2.0/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 14:01:44.202255 xyzservices-2023.2.0/xyzservices/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-19 14:01:39.000000 xyzservices-2023.2.0/xyzservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-19 14:01:44.202255 xyzservices-2023.2.0/xyzservices/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 14:01:44.202255 xyzservices-2023.2.0/xyzservices/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 14:01:39.000000 xyzservices-2023.2.0/xyzservices/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   412477 2023-02-19 14:01:39.000000 xyzservices-2023.2.0/xyzservices/data/providers.json
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-02-19 14:01:39.000000 xyzservices-2023.2.0/xyzservices/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-19 14:01:39.000000 xyzservices-2023.2.0/xyzservices/providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 14:01:44.202255 xyzservices-2023.2.0/xyzservices/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 14:01:39.000000 xyzservices-2023.2.0/xyzservices/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-02-19 14:01:39.000000 xyzservices-2023.2.0/xyzservices/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-02-19 14:01:39.000000 xyzservices-2023.2.0/xyzservices/tests/test_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 14:01:44.202255 xyzservices-2023.2.0/xyzservices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-02-19 14:01:44.000000 xyzservices-2023.2.0/xyzservices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-19 14:01:44.000000 xyzservices-2023.2.0/xyzservices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 14:01:44.000000 xyzservices-2023.2.0/xyzservices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-19 14:01:44.000000 xyzservices-2023.2.0/xyzservices.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.321644 xyzservices-2023.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.github/PULL_REQUEST_TEMPLATE/community_contribution.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.github/workflows/release_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.github/workflows/update_providers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-19 20:50:17.321644 xyzservices-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/ci/latest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/ci/update_providers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/_static/generate_gallery.js
+-rw-r--r--   0 runner    (1001) docker     (123)   380575 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/_static/xyzmaps.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/gallery.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35770 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/registration.md
+-rw-r--r--   0 runner    (1001) docker     (123)   663316 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/tiles.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/provider_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/provider_sources/_compress_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/provider_sources/_parse_leaflet_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/provider_sources/leaflet-providers-parsed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/provider_sources/xyzservices-providers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 20:50:17.321644 xyzservices-2023.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/xyzservices/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.321644 xyzservices-2023.5.0/xyzservices/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   430664 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/data/providers.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21475 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.321644 xyzservices-2023.5.0/xyzservices/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/tests/test_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/xyzservices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-19 20:50:17.000000 xyzservices-2023.5.0/xyzservices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-19 20:50:17.000000 xyzservices-2023.5.0/xyzservices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:50:17.000000 xyzservices-2023.5.0/xyzservices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 20:50:17.000000 xyzservices-2023.5.0/xyzservices.egg-info/top_level.txt
```

### Comparing `xyzservices-2023.2.0/LICENSE` & `xyzservices-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.2.0/PKG-INFO` & `xyzservices-2023.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: xyzservices
-Version: 2023.2.0
+Version: 2023.5.0
 Summary: Source of XYZ tiles providers
 Home-page: https://github.com/geopandas/xyzservices
 Author: Dani Arribas-Bel, Martin Fleischmann
 Author-email: daniel.arribas.bel@gmail.com, martin@martinfleischmann.net
 License: 3-Clause BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # xyzservices - Source of XYZ tiles providers
 
 `xyzservices` is a lightweight library providing a repository of available XYZ services
 offering raster basemap tiles. The repository is provided via Python API and as a
```

### Comparing `xyzservices-2023.2.0/README.md` & `xyzservices-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.2.0/xyzservices/data/providers.json` & `xyzservices-2023.5.0/xyzservices/data/providers.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9743036265432099%*

 * *Differences: {"'GeoportailFrance'": "{'Orthoimagery_Orthophotos_Ortho_asp_pac2022': {'apikey': 'orthohisto'}, "*

 * *                       "'Bdcarto_etat_major_Niveau3': {'bounds': [[43.151, -5.15012], [51.0938, "*

 * *                       "7.19384]]}, 'Prairies_Sensibles_Bcae': OrderedDict([('url', "*

 * *                       "'https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}'), […]*

```diff
@@ -668,20 +668,20 @@
         },
         "Bdcarto_etat_major_Niveau3": {
             "TileMatrixSet": "PM",
             "apikey": "sol",
             "attribution": "Geoportail France",
             "bounds": [
                 [
-                    41.3252,
-                    -5.15047
+                    43.151,
+                    -5.15012
                 ],
                 [
-                    51.0991,
-                    9.57054
+                    51.0938,
+                    7.19384
                 ]
             ],
             "format": "image/png",
             "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
             "max_zoom": 16,
             "min_zoom": 6,
             "name": "GeoportailFrance.Bdcarto_etat_major_Niveau3",
@@ -754,14 +754,37 @@
             "max_zoom": 17,
             "min_zoom": 6,
             "name": "GeoportailFrance.Communes_Prioritydisctrict",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "COMMUNES.PRIORITYDISCTRICT"
         },
+        "Debroussaillement": {
+            "TileMatrixSet": "PM",
+            "apikey": "environnement",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    41.3252,
+                    -5.15047
+                ],
+                [
+                    51.0991,
+                    9.57054
+                ]
+            ],
+            "format": "image/png",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 18,
+            "min_zoom": 6,
+            "name": "GeoportailFrance.Debroussaillement",
+            "style": "nolegend",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "DEBROUSSAILLEMENT"
+        },
         "Dreal_Zonage_pinel": {
             "TileMatrixSet": "PM",
             "apikey": "economie",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     47.2719,
@@ -1283,37 +1306,14 @@
             "max_zoom": 19,
             "min_zoom": 6,
             "name": "GeoportailFrance.Hr_Orthoimagery_Orthophotos",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "HR.ORTHOIMAGERY.ORTHOPHOTOS"
         },
-        "Hydrography_Bcae_2022": {
-            "TileMatrixSet": "PM",
-            "apikey": "agriculture",
-            "attribution": "Geoportail France",
-            "bounds": [
-                [
-                    41.3252,
-                    -5.15047
-                ],
-                [
-                    51.0991,
-                    9.57054
-                ]
-            ],
-            "format": "image/png",
-            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
-            "max_zoom": 17,
-            "min_zoom": 6,
-            "name": "GeoportailFrance.Hydrography_Bcae_2022",
-            "style": "normal",
-            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
-            "variant": "HYDROGRAPHY.BCAE.2022"
-        },
         "Hydrography_Bcae_Latest": {
             "TileMatrixSet": "PM",
             "apikey": "agriculture",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     41.3252,
@@ -3400,14 +3400,60 @@
             "min_zoom": 6,
             "name": "GeoportailFrance.Ocsge_Constructions_2002",
             "status": "broken",
             "style": "nolegend",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "OCSGE.CONSTRUCTIONS.2002"
         },
+        "Ocsge_Constructions_2010": {
+            "TileMatrixSet": "PM",
+            "apikey": "ocsge",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    41.3252,
+                    -5.15047
+                ],
+                [
+                    51.0991,
+                    9.57054
+                ]
+            ],
+            "format": "image/png",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 16,
+            "min_zoom": 6,
+            "name": "GeoportailFrance.Ocsge_Constructions_2010",
+            "style": "nolegend",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "OCSGE.CONSTRUCTIONS.2010"
+        },
+        "Ocsge_Constructions_2011": {
+            "TileMatrixSet": "PM",
+            "apikey": "ocsge",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    41.3252,
+                    -5.15047
+                ],
+                [
+                    51.0991,
+                    9.57054
+                ]
+            ],
+            "format": "image/png",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 16,
+            "min_zoom": 6,
+            "name": "GeoportailFrance.Ocsge_Constructions_2011",
+            "style": "nolegend",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "OCSGE.CONSTRUCTIONS.2011"
+        },
         "Ocsge_Constructions_2014": {
             "TileMatrixSet": "PM",
             "apikey": "ocsge",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     41.366,
@@ -3447,14 +3493,37 @@
             "max_zoom": 16,
             "min_zoom": 6,
             "name": "GeoportailFrance.Ocsge_Constructions_2016",
             "style": "nolegend",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "OCSGE.CONSTRUCTIONS.2016"
         },
+        "Ocsge_Constructions_2017": {
+            "TileMatrixSet": "PM",
+            "apikey": "ocsge",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    14.2395,
+                    -61.6644
+                ],
+                [
+                    51.0991,
+                    9.57054
+                ]
+            ],
+            "format": "image/png",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 16,
+            "min_zoom": 6,
+            "name": "GeoportailFrance.Ocsge_Constructions_2017",
+            "style": "nolegend",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "OCSGE.CONSTRUCTIONS.2017"
+        },
         "Ocsge_Constructions_2019": {
             "TileMatrixSet": "PM",
             "apikey": "ocsge",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     43.3043,
@@ -3517,14 +3586,60 @@
             "min_zoom": 6,
             "name": "GeoportailFrance.Ocsge_Couverture_2002",
             "status": "broken",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "OCSGE.COUVERTURE.2002"
         },
+        "Ocsge_Couverture_2010": {
+            "TileMatrixSet": "PM",
+            "apikey": "ocsge",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    41.3252,
+                    -5.15047
+                ],
+                [
+                    51.0991,
+                    9.57054
+                ]
+            ],
+            "format": "image/png",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 16,
+            "min_zoom": 6,
+            "name": "GeoportailFrance.Ocsge_Couverture_2010",
+            "style": "nolegend",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "OCSGE.COUVERTURE.2010"
+        },
+        "Ocsge_Couverture_2011": {
+            "TileMatrixSet": "PM",
+            "apikey": "ocsge",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    41.3252,
+                    -5.15047
+                ],
+                [
+                    51.0991,
+                    9.57054
+                ]
+            ],
+            "format": "image/png",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 16,
+            "min_zoom": 6,
+            "name": "GeoportailFrance.Ocsge_Couverture_2011",
+            "style": "nolegend",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "OCSGE.COUVERTURE.2011"
+        },
         "Ocsge_Couverture_2014": {
             "TileMatrixSet": "PM",
             "apikey": "ocsge",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     41.366,
@@ -3564,14 +3679,37 @@
             "max_zoom": 16,
             "min_zoom": 6,
             "name": "GeoportailFrance.Ocsge_Couverture_2016",
             "style": "nolegend",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "OCSGE.COUVERTURE.2016"
         },
+        "Ocsge_Couverture_2017": {
+            "TileMatrixSet": "PM",
+            "apikey": "ocsge",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    14.2395,
+                    -61.6644
+                ],
+                [
+                    51.0991,
+                    9.57054
+                ]
+            ],
+            "format": "image/png",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 16,
+            "min_zoom": 6,
+            "name": "GeoportailFrance.Ocsge_Couverture_2017",
+            "style": "nolegend",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "OCSGE.COUVERTURE.2017"
+        },
         "Ocsge_Couverture_2019": {
             "TileMatrixSet": "PM",
             "apikey": "ocsge",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     43.3043,
@@ -3634,14 +3772,60 @@
             "min_zoom": 6,
             "name": "GeoportailFrance.Ocsge_Usage_2002",
             "status": "broken",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "OCSGE.USAGE.2002"
         },
+        "Ocsge_Usage_2010": {
+            "TileMatrixSet": "PM",
+            "apikey": "ocsge",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    41.3252,
+                    -5.15047
+                ],
+                [
+                    51.0991,
+                    9.57054
+                ]
+            ],
+            "format": "image/png",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 16,
+            "min_zoom": 6,
+            "name": "GeoportailFrance.Ocsge_Usage_2010",
+            "style": "nolegend",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "OCSGE.USAGE.2010"
+        },
+        "Ocsge_Usage_2011": {
+            "TileMatrixSet": "PM",
+            "apikey": "ocsge",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    41.3252,
+                    -5.15047
+                ],
+                [
+                    51.0991,
+                    9.57054
+                ]
+            ],
+            "format": "image/png",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 16,
+            "min_zoom": 6,
+            "name": "GeoportailFrance.Ocsge_Usage_2011",
+            "style": "nolegend",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "OCSGE.USAGE.2011"
+        },
         "Ocsge_Usage_2014": {
             "TileMatrixSet": "PM",
             "apikey": "ocsge",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     41.366,
@@ -3681,14 +3865,37 @@
             "max_zoom": 16,
             "min_zoom": 6,
             "name": "GeoportailFrance.Ocsge_Usage_2016",
             "style": "nolegend",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "OCSGE.USAGE.2016"
         },
+        "Ocsge_Usage_2017": {
+            "TileMatrixSet": "PM",
+            "apikey": "ocsge",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    14.2395,
+                    -61.6644
+                ],
+                [
+                    51.0991,
+                    9.57054
+                ]
+            ],
+            "format": "image/png",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 16,
+            "min_zoom": 6,
+            "name": "GeoportailFrance.Ocsge_Usage_2017",
+            "style": "nolegend",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "OCSGE.USAGE.2017"
+        },
         "Ocsge_Usage_2019": {
             "TileMatrixSet": "PM",
             "apikey": "ocsge",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     43.3043,
@@ -5249,15 +5456,15 @@
             "name": "GeoportailFrance.Orthoimagery_Orthophotos_Ortho_asp_pac2021",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "ORTHOIMAGERY.ORTHOPHOTOS.ORTHO-ASP_PAC2021"
         },
         "Orthoimagery_Orthophotos_Ortho_asp_pac2022": {
             "TileMatrixSet": "PM",
-            "apikey": "ortho",
+            "apikey": "orthohisto",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     -75.0,
                     -179.5
                 ],
                 [
@@ -5270,14 +5477,37 @@
             "max_zoom": 18,
             "min_zoom": 0,
             "name": "GeoportailFrance.Orthoimagery_Orthophotos_Ortho_asp_pac2022",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "ORTHOIMAGERY.ORTHOPHOTOS.ORTHO-ASP_PAC2022"
         },
+        "Orthoimagery_Orthophotos_Ortho_asp_pac2023": {
+            "TileMatrixSet": "PM",
+            "apikey": "ortho",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    -75.0,
+                    -179.5
+                ],
+                [
+                    75.0,
+                    179.5
+                ]
+            ],
+            "format": "image/jpeg",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 18,
+            "min_zoom": 0,
+            "name": "GeoportailFrance.Orthoimagery_Orthophotos_Ortho_asp_pac2023",
+            "style": "normal",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "ORTHOIMAGERY.ORTHOPHOTOS.ORTHO-ASP_PAC2023"
+        },
         "Orthoimagery_Orthophotos_Ortho_express_2021": {
             "TileMatrixSet": "PM",
             "apikey": "orthohisto",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     -75.0,
@@ -5386,14 +5616,37 @@
             "min_zoom": 6,
             "name": "GeoportailFrance.Pcrs_Lamb93",
             "status": "broken",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "PCRS.LAMB93"
         },
+        "Prairies_Sensibles_Bcae": {
+            "TileMatrixSet": "PM",
+            "apikey": "agriculture",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    41.3252,
+                    -5.15047
+                ],
+                [
+                    51.0991,
+                    9.57054
+                ]
+            ],
+            "format": "image/png",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 16,
+            "min_zoom": 6,
+            "name": "GeoportailFrance.Prairies_Sensibles_Bcae",
+            "style": "nolegend",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "PRAIRIES.SENSIBLES.BCAE"
+        },
         "Protectedareas_Apb": {
             "TileMatrixSet": "PM",
             "apikey": "environnement",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     -21.4756,
@@ -5455,14 +5708,37 @@
             "max_zoom": 16,
             "min_zoom": 6,
             "name": "GeoportailFrance.Protectedareas_Aphn",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "PROTECTEDAREAS.APHN"
         },
+        "Protectedareas_Aplg": {
+            "TileMatrixSet": "PM",
+            "apikey": "environnement",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    -53.6279,
+                    -63.3725
+                ],
+                [
+                    51.3121,
+                    82.645
+                ]
+            ],
+            "format": "image/png",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 16,
+            "min_zoom": 6,
+            "name": "GeoportailFrance.Protectedareas_Aplg",
+            "style": "nolegend",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "PROTECTEDAREAS.APLG"
+        },
         "Protectedareas_Bios": {
             "TileMatrixSet": "PM",
             "apikey": "environnement",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     -21.4756,
@@ -5961,14 +6237,37 @@
             "max_zoom": 16,
             "min_zoom": 6,
             "name": "GeoportailFrance.Protectedareas_Znieff2_Sea",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "PROTECTEDAREAS.ZNIEFF2.SEA"
         },
+        "Protectedareas_Zpr": {
+            "TileMatrixSet": "PM",
+            "apikey": "environnement",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    -53.6279,
+                    -63.3725
+                ],
+                [
+                    51.3121,
+                    82.645
+                ]
+            ],
+            "format": "image/png",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 16,
+            "min_zoom": 6,
+            "name": "GeoportailFrance.Protectedareas_Zpr",
+            "style": "nolegend",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "PROTECTEDAREAS.ZPR"
+        },
         "Protectedareas_Zps": {
             "TileMatrixSet": "PM",
             "apikey": "environnement",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     -21.4756,
@@ -8498,14 +8797,160 @@
             "max_zoom": 19,
             "name": "OpenWeatherMap.Wind",
             "opacity": 0.5,
             "url": "http://{s}.tile.openweathermap.org/map/{variant}/{z}/{x}/{y}.png?appid={apiKey}",
             "variant": "wind"
         }
     },
+    "OrdnanceSurvey": {
+        "Leisure_27700": {
+            "attribution": "Contains OS data (C) Crown copyright and database right 2023",
+            "bounds": [
+                [
+                    0,
+                    0
+                ],
+                [
+                    700000,
+                    1300000
+                ]
+            ],
+            "crs": "EPSG:27700",
+            "html_attribution": "Contains OS data &copy Crown copyright and database right 2023",
+            "key": "<insert your valid OS MapsAPI Key. Get a free key here - https://osdatahub.os.uk/>",
+            "max_zoom": 5,
+            "max_zoom_premium": 9,
+            "min_zoom": 0,
+            "name": "OrdnanceSurvey.Leisure_27700",
+            "url": "https://api.os.uk/maps/raster/v1/zxy/Leisure_27700/{z}/{x}/{y}.png?key={key}"
+        },
+        "Light": {
+            "attribution": "Contains OS data (C) Crown copyright and database right 2023",
+            "bounds": [
+                [
+                    49.766807,
+                    -9.496386
+                ],
+                [
+                    61.465189,
+                    3.634745
+                ]
+            ],
+            "html_attribution": "Contains OS data &copy Crown copyright and database right 2023",
+            "key": "<insert your valid OS MapsAPI Key. Get a free key here - https://osdatahub.os.uk/>",
+            "max_zoom": 16,
+            "max_zoom_premium": 20,
+            "min_zoom": 7,
+            "name": "OrdnanceSurvey.Light",
+            "url": "https://api.os.uk/maps/raster/v1/zxy/Light_3857/{z}/{x}/{y}.png?key={key}"
+        },
+        "Light_27700": {
+            "attribution": "Contains OS data (C) Crown copyright and database right 2023",
+            "bounds": [
+                [
+                    0,
+                    0
+                ],
+                [
+                    700000,
+                    1300000
+                ]
+            ],
+            "crs": "EPSG:27700",
+            "html_attribution": "Contains OS data &copy Crown copyright and database right 2023",
+            "key": "<insert your valid OS MapsAPI Key. Get a free key here - https://osdatahub.os.uk/>",
+            "max_zoom": 9,
+            "max_zoom_premium": 13,
+            "min_zoom": 0,
+            "name": "OrdnanceSurvey.Light_27700",
+            "url": "https://api.os.uk/maps/raster/v1/zxy/Light_27700/{z}/{x}/{y}.png?key={key}"
+        },
+        "Outdoor": {
+            "attribution": "Contains OS data (C) Crown copyright and database right 2023",
+            "bounds": [
+                [
+                    49.766807,
+                    -9.496386
+                ],
+                [
+                    61.465189,
+                    3.634745
+                ]
+            ],
+            "html_attribution": "Contains OS data &copy Crown copyright and database right 2023",
+            "key": "<insert your valid OS MapsAPI Key. Get a free key here - https://osdatahub.os.uk/>",
+            "max_zoom": 16,
+            "max_zoom_premium": 20,
+            "min_zoom": 7,
+            "name": "OrdnanceSurvey.Outdoor",
+            "url": "https://api.os.uk/maps/raster/v1/zxy/Outdoor_3857/{z}/{x}/{y}.png?key={key}"
+        },
+        "Outdoor_27700": {
+            "attribution": "Contains OS data (C) Crown copyright and database right 2023",
+            "bounds": [
+                [
+                    0,
+                    0
+                ],
+                [
+                    700000,
+                    1300000
+                ]
+            ],
+            "crs": "EPSG:27700",
+            "html_attribution": "Contains OS data &copy Crown copyright and database right 2023",
+            "key": "<insert your valid OS MapsAPI Key. Get a free key here - https://osdatahub.os.uk/>",
+            "max_zoom": 9,
+            "max_zoom_premium": 13,
+            "min_zoom": 0,
+            "name": "OrdnanceSurvey.Outdoor_27700",
+            "url": "https://api.os.uk/maps/raster/v1/zxy/Outdoor_27700/{z}/{x}/{y}.png?key={key}"
+        },
+        "Road": {
+            "attribution": "Contains OS data (C) Crown copyright and database right 2023",
+            "bounds": [
+                [
+                    49.766807,
+                    -9.496386
+                ],
+                [
+                    61.465189,
+                    3.634745
+                ]
+            ],
+            "html_attribution": "Contains OS data &copy Crown copyright and database right 2023",
+            "key": "<insert your valid OS MapsAPI Key. Get a free key here - https://osdatahub.os.uk/>",
+            "max_zoom": 16,
+            "max_zoom_premium": 20,
+            "min_zoom": 7,
+            "name": "OrdnanceSurvey.Road",
+            "url": "https://api.os.uk/maps/raster/v1/zxy/Road_3857/{z}/{x}/{y}.png?key={key}"
+        },
+        "Road_27700": {
+            "attribution": "Contains OS data (C) Crown copyright and database right 2023",
+            "bounds": [
+                [
+                    0,
+                    0
+                ],
+                [
+                    700000,
+                    1300000
+                ]
+            ],
+            "crs": "EPSG:27700",
+            "html_attribution": "Contains OS data &copy Crown copyright and database right 2023",
+            "key": "<insert your valid OS MapsAPI Key. Get a free key here - https://osdatahub.os.uk/>",
+            "max_zoom": 9,
+            "max_zoom_premium": 13,
+            "min_zoom": 0,
+            "name": "OrdnanceSurvey.Road_27700",
+            "url": "https://api.os.uk/maps/raster/v1/zxy/Road_27700/{z}/{x}/{y}.png?key={key}"
+        }
+    },
     "SafeCast": {
         "attribution": "Map data: (C) OpenStreetMap contributors | Map style: (C) SafeCast (CC-BY-SA)",
         "html_attribution": "Map data: &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors | Map style: &copy; <a href=\"https://blog.safecast.org/about/\">SafeCast</a> (<a href=\"https://creativecommons.org/licenses/by-sa/3.0/\">CC-BY-SA</a>)",
         "max_zoom": 16,
         "name": "SafeCast",
         "url": "https://s3.amazonaws.com/te512.safecast.org/{z}/{x}/{y}.png"
     },
```

### Comparing `xyzservices-2023.2.0/xyzservices/lib.py` & `xyzservices-2023.5.0/xyzservices/lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Utilities to support XYZservices
 """
 from __future__ import annotations
 
 import json
-import uuid
 import urllib.request
-from typing import Optional, Callable, Union
+import uuid
+from typing import Callable
 from urllib.parse import quote
 
 QUERY_NAME_TRANSLATION = str.maketrans({x: "" for x in "., -_/"})
 
 
 class Bunch(dict):
     """A dict with attribute-access
@@ -38,24 +38,23 @@
     >>> MyTiles.BlackAndWhite.url
     'https://myserver.com/bw/{z}/{x}/{y}'
     """
 
     def __getattr__(self, key):
         try:
             return self.__getitem__(key)
-        except KeyError:
-            raise AttributeError(key)
+        except KeyError as err:
+            raise AttributeError(key) from err
 
     def __dir__(self):
         return self.keys()
 
     def _repr_html_(self, inside=False):
-
         children = ""
-        for key in self.keys():
+        for key in self:
             if isinstance(self[key], TileProvider):
                 obj = "xyzservices.TileProvider"
             else:
                 obj = "xyzservices.Bunch"
             uid = str(uuid.uuid4())
             children += f"""
             <li class="xyz-child">
@@ -121,17 +120,17 @@
 
         _get_providers(self)
 
         return flat
 
     def filter(
         self,
-        keyword: Optional[str] = None,
-        name: Optional[str] = None,
-        requires_token: Optional[bool] = None,
+        keyword: str | None = None,
+        name: str | None = None,
+        requires_token: bool | None = None,
         function: Callable[[TileProvider], bool] = None,
     ) -> Bunch:
         """Return a subset of the :class:`Bunch` matching the filter conditions
 
         Each :class:`TileProvider` within a :class:`Bunch` is checked against one or
         more specified conditions and kept if they are satisfied or removed if at least
         one condition is not met.
@@ -186,24 +185,22 @@
         ...    if hasattr(provider, "max_zoom") and provider.max_zoom < 18:
         ...        return True
         ...    return False
         >>> small_zoom = xyz.filter(function=zoom18)
         """
 
         def _validate(provider, keyword, name, requires_token):
-
             cond = []
 
             if keyword is not None:
                 keyword_match = False
                 for v in provider.values():
-                    if isinstance(v, str):
-                        if keyword.lower() in v.lower():
-                            keyword_match = True
-                            break
+                    if isinstance(v, str) and keyword.lower() in v.lower():
+                        keyword_match = True
+                        break
                 cond.append(keyword_match)
 
             if name is not None:
                 name_match = False
                 if name.lower() in provider.name.lower():
                     name_match = True
                 cond.append(name_match)
@@ -216,15 +213,14 @@
 
             return all(cond)
 
         def _filter_bunch(bunch, keyword, name, requires_token, function):
             new = Bunch()
             for key, value in bunch.items():
                 if isinstance(value, TileProvider):
-
                     if function is None:
                         if _validate(
                             value,
                             keyword=keyword,
                             name=name,
                             requires_token=requires_token,
                         ):
@@ -374,25 +370,25 @@
             raise AttributeError(msg)
 
     def __call__(self, **kwargs) -> TileProvider:
         new = TileProvider(self)  # takes a copy preserving the class
         new.update(kwargs)
         return new
 
-    def copy(self, **kwargs) -> TileProvider:
+    def copy(self) -> TileProvider:
         new = TileProvider(self)  # takes a copy preserving the class
         return new
 
     def build_url(
         self,
-        x: Optional[Union[int, str]] = None,
-        y: Optional[Union[int, str]] = None,
-        z: Optional[Union[int, str]] = None,
-        scale_factor: Optional[str] = None,
-        fill_subdomain: Optional[bool] = True,
+        x: int | str | None = None,
+        y: int | str | None = None,
+        z: int | str | None = None,
+        scale_factor: str | None = None,
+        fill_subdomain: bool | None = True,
         **kwargs,
     ) -> str:
         """
         Build the URL of tiles from the :class:`TileProvider` object
 
         Can return URL with placeholders or the final tile URL.
 
@@ -502,22 +498,21 @@
 
         >>> xyz.OpenWeatherMap.Clouds(apiKey="my-private-api-key")
 
 
         """
         # both attribute and placeholder in url are required to make it work
         for key, val in self.items():
-            if isinstance(val, str) and "<insert your" in val:
-                if key in self.url:
-                    return True
+            if isinstance(val, str) and "<insert your" in val and key in self.url:
+                return True
         return False
 
     @property
     def html_attribution(self):
-        if "html_attribution" in self.keys():
+        if "html_attribution" in self:
             return self["html_attribution"]
         return self["attribution"]
 
     def _repr_html_(self, inside=False):
         provider_info = ""
         for key, val in self.items():
             if key != "name":
@@ -559,50 +554,49 @@
         :class:`TileProvider`
 
         Examples
         --------
         >>> from xyzservices.lib import TileProvider
         >>> provider = TileProvider.from_qms("OpenTopoMap")
         """
-        QMS_API_URL = "https://qms.nextgis.com/api/v1/geoservices"
+        qms_api_url = "https://qms.nextgis.com/api/v1/geoservices"
 
         services = json.load(
-            urllib.request.urlopen(f"{QMS_API_URL}/?search={quote(name)}&type=tms")
+            urllib.request.urlopen(f"{qms_api_url}/?search={quote(name)}&type=tms")
         )
 
         for service in services:
             if service["name"] == name:
                 break
         else:
             raise ValueError(f"Service '{name}' not found.")
 
         service_id = service["id"]
         service_details = json.load(
-            urllib.request.urlopen(f"{QMS_API_URL}/{service_id}")
+            urllib.request.urlopen(f"{qms_api_url}/{service_id}")
         )
 
         return cls(
             name=service_details["name"],
             url=service_details["url"],
             min_zoom=service_details.get("z_min"),
             max_zoom=service_details.get("z_max"),
             attribution=service_details.get("copyright_text"),
         )
 
 
 def _load_json(f):
-
     data = json.loads(f)
 
     providers = Bunch()
 
-    for provider_name in data.keys():
+    for provider_name in data:
         provider = data[provider_name]
 
-        if "url" in provider.keys():
+        if "url" in provider:
             providers[provider_name] = TileProvider(provider)
 
         else:
             providers[provider_name] = Bunch(
                 {i: TileProvider(provider[i]) for i in provider}
             )
```

### Comparing `xyzservices-2023.2.0/xyzservices/tests/test_lib.py` & `xyzservices-2023.5.0/xyzservices/tests/test_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import pytest
 from urllib.error import URLError
 
+import pytest
+
 import xyzservices.providers as xyz
-from xyzservices import TileProvider, Bunch
+from xyzservices import Bunch, TileProvider
 
 
 @pytest.fixture
 def basic_provider():
     return TileProvider(
         url="https://myserver.com/tiles/{z}/{x}/{y}.png",
         attribution="(C) xyzservices",
```

### Comparing `xyzservices-2023.2.0/xyzservices/tests/test_providers.py` & `xyzservices-2023.5.0/xyzservices/tests/test_providers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 
+import mercantile
 import pytest
-import xyzservices.providers as xyz
 import requests
-import mercantile
+
+import xyzservices.providers as xyz
 
 flat_free = xyz.filter(requires_token=False).flatten()
 
 
 def check_provider(provider):
     for key in ["attribution", "name"]:
-        assert key in provider.keys()
+        assert key in provider
     assert provider.url.startswith("http")
     for option in ["{z}", "{y}", "{x}"]:
         assert option in provider.url
 
 
 def get_tile(provider):
     bounds = provider.get("bounds", [[-180, -90], [180, 90]])
@@ -81,15 +82,15 @@
                 (12, 2074, 1410),
             ]
             results = []
             for o in options:
                 z, x, y = o
                 r = get_response(provider.build_url(z=z, x=x, y=y))
                 results.append(r)
-            if not any([x == requests.codes.ok for x in results]):
+            if not any(x == requests.codes.ok for x in results):
                 raise ValueError(f"Response code: {r}")
         else:
             raise ValueError(f"Response code: {r}")
 
 
 @pytest.mark.parametrize("provider_name", xyz.flatten())
 def test_minimal_provider_metadata(provider_name):
@@ -97,14 +98,16 @@
     check_provider(provider)
 
 
 @pytest.mark.request
 @pytest.mark.parametrize("name", flat_free)
 def test_free_providers(name):
     provider = flat_free[name]
+    if "Stadia" in name:
+        pytest.skip("Stadia doesn't support tile download in this way.")
     get_test_result(provider)
 
 
 # test providers requiring API keys. Store API keys in GitHub secrets and load them as
 # environment variables in CI Action. Note that env variable is loaded as empty on PRs
 # from a fork.
 
@@ -217,9 +220,23 @@
         pytest.xfail("Token empty.")
 
     provider = xyz.Stadia[provider_name](api_key=token)
     provider["url"] = provider["url"] + "?api_key={api_key}"
     get_test_result(provider, allow_403=False)
 
 
+@pytest.mark.request
+@pytest.mark.parametrize("provider_name", xyz.OrdnanceSurvey)
+def test_os(provider_name):
+    try:
+        token = os.environ["ORDNANCESURVEY"]
+    except KeyError:
+        pytest.xfail("Missing API token.")
+    if token == "":
+        pytest.xfail("Token empty.")
+
+    provider = xyz.OrdnanceSurvey[provider_name](key=token)
+    get_test_result(provider, allow_403=False)
+
+
 # NOTE: AzureMaps are not tested as their free account is limited to
 # 5000 downloads (total, not per month)
```

### Comparing `xyzservices-2023.2.0/xyzservices.egg-info/PKG-INFO` & `xyzservices-2023.5.0/xyzservices.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: xyzservices
-Version: 2023.2.0
+Version: 2023.5.0
 Summary: Source of XYZ tiles providers
 Home-page: https://github.com/geopandas/xyzservices
 Author: Dani Arribas-Bel, Martin Fleischmann
 Author-email: daniel.arribas.bel@gmail.com, martin@martinfleischmann.net
 License: 3-Clause BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # xyzservices - Source of XYZ tiles providers
 
 `xyzservices` is a lightweight library providing a repository of available XYZ services
 offering raster basemap tiles. The repository is provided via Python API and as a
```

