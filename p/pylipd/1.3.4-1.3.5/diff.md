# Comparing `tmp/pylipd-1.3.4.tar.gz` & `tmp/pylipd-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylipd-1.3.4.tar", last modified: Fri May 19 17:04:10 2023, max compression
+gzip compressed data, was "pylipd-1.3.5.tar", last modified: Fri May 19 17:48:29 2023, max compression
```

## Comparing `pylipd-1.3.4.tar` & `pylipd-1.3.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:04:10.074458 pylipd-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 17:04:01.000000 pylipd-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-19 17:04:10.074458 pylipd-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 17:04:01.000000 pylipd-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:04:10.066457 pylipd-1.3.4/pylipd/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:04:10.070457 pylipd-1.3.4/pylipd/globals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/globals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/globals/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/globals/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/globals/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/globals/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    29684 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/lipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/lipd_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:04:10.070457 pylipd-1.3.4/pylipd/series/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/series/regexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/usage_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:04:10.070457 pylipd-1.3.4/pylipd/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16043 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/utils/legacy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    43569 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/utils/lipd_to_rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/utils/multi_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/utils/rdf_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/utils/rdf_to_lipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-19 17:04:01.000000 pylipd-1.3.4/pylipd/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:04:10.074458 pylipd-1.3.4/pylipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-19 17:04:10.000000 pylipd-1.3.4/pylipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-19 17:04:10.000000 pylipd-1.3.4/pylipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:04:10.000000 pylipd-1.3.4/pylipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:04:10.000000 pylipd-1.3.4/pylipd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 17:04:10.000000 pylipd-1.3.4/pylipd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 17:04:10.000000 pylipd-1.3.4/pylipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 17:04:01.000000 pylipd-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 17:04:10.074458 pylipd-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-19 17:04:01.000000 pylipd-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:29.209162 pylipd-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 17:48:22.000000 pylipd-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-19 17:48:29.209162 pylipd-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 17:48:22.000000 pylipd-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:29.209162 pylipd-1.3.5/pylipd/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:29.209162 pylipd-1.3.5/pylipd/globals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/globals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/globals/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/globals/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/globals/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/globals/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29677 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/lipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/lipd_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:29.209162 pylipd-1.3.5/pylipd/series/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/series/regexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/usage_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:29.209162 pylipd-1.3.5/pylipd/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16043 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/legacy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43683 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/lipd_to_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/multi_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/rdf_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/rdf_to_lipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:29.209162 pylipd-1.3.5/pylipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-19 17:48:29.000000 pylipd-1.3.5/pylipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-19 17:48:29.000000 pylipd-1.3.5/pylipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:48:29.000000 pylipd-1.3.5/pylipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:48:29.000000 pylipd-1.3.5/pylipd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 17:48:29.000000 pylipd-1.3.5/pylipd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 17:48:29.000000 pylipd-1.3.5/pylipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 17:48:22.000000 pylipd-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 17:48:29.209162 pylipd-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-19 17:48:22.000000 pylipd-1.3.5/setup.py
```

### Comparing `pylipd-1.3.4/LICENSE` & `pylipd-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.4/PKG-INFO` & `pylipd-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.4
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.5
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.0
```

### Comparing `pylipd-1.3.4/README.md` & `pylipd-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.4/pylipd/globals/queries.py` & `pylipd-1.3.5/pylipd/globals/queries.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.4/pylipd/globals/schema.py` & `pylipd-1.3.5/pylipd/globals/schema.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.4/pylipd/lipd.py` & `pylipd-1.3.5/pylipd/lipd.py`

 * *Files 1% similar despite different names*

```diff
@@ -701,15 +701,15 @@
                 "../examples/data/MD98_2181.Stott.2007.lpd"
             ])
             print(lipd.get_all_archiveTypes())
 
         '''
         
         qres, qres_df = self.query(QUERY_UNIQUE_ARCHIVE_TYPE)
-        return [sanitizeId(row.archiveType) for row in qres]
+        return [str(row.archiveType) for row in qres]
         
         
 
     def get_ensemble_tables(self, dsname = None, ensembleVarName = None, ensembleDepthVarName = 'depth'):
         '''Gets ensemble tables from the LiPD graph
 
         Parameters
```

### Comparing `pylipd-1.3.4/pylipd/lipd_series.py` & `pylipd-1.3.5/pylipd/lipd_series.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.4/pylipd/series/regexes.py` & `pylipd-1.3.5/pylipd/series/regexes.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.4/pylipd/usage.py` & `pylipd-1.3.5/pylipd/usage.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.4/pylipd/usage_parallel.py` & `pylipd-1.3.5/pylipd/usage_parallel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 if __name__ == "__main__":
     from pylipd.lipd import LiPD
 
     local_lipd_dir = "/Users/varun/git/LiPD/PyLiPD/data/lpd.latest"
 
     L = LiPD()
 
+    L.load_from_dir("examples/data/Euro2k", parallel=True, cutoff=1000)
+    Lfiltered = L.filter_by_archive_type("marine")
+    print(len(Lfiltered.get_all_dataset_names()))
+    print(Lfiltered.get_all_archiveTypes())
+
     # Convert LiPD files to RDF    
-    L.convert_lipd_dir_to_rdf(
-        local_lipd_dir,
-        local_lipd_dir+".nq", 
-        parallel=True)
+    # L.convert_lipd_dir_to_rdf(
+    #     local_lipd_dir,
+    #     local_lipd_dir+".nq", 
+    #     parallel=True)
     
     '''
     L.load_from_dir(local_lipd_dir, parallel=True, cutoff=1000)
     
     print(f"Total number of datasets: {len(L.get_all_dataset_names())}")
 
     print("Filtering by archive type and bounding box")
```

### Comparing `pylipd-1.3.4/pylipd/utils/dataset.py` & `pylipd-1.3.5/pylipd/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.4/pylipd/utils/legacy_utils.py` & `pylipd-1.3.5/pylipd/utils/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.4/pylipd/utils/lipd_to_rdf.py` & `pylipd-1.3.5/pylipd/utils/lipd_to_rdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1122,14 +1122,16 @@
 
     def _load_lipd_json_to_graph(self, jsonpath, url=None):
         self.graph = ConjunctiveGraph()
         objhash = {}
         
         with open(jsonpath) as f:
             obj = json.load(f)
+            if "dataSetName" in obj:
+                self.graphurl = NSURL + "/" + sanitizeId(obj["dataSetName"])
             
             self._map_lipd_to_json(obj, None, None, "Dataset", "Dataset", objhash)
             if url:
                 objhash[obj["@id"]]["hasUrl"] = url
             else:
                 objhash[obj["@id"]]["hasUrl"] = DATAURL + "/" + obj["@id"] + ".lpd"
```

### Comparing `pylipd-1.3.4/pylipd/utils/multi_processing.py` & `pylipd-1.3.5/pylipd/utils/multi_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         args = [(lipdfile, rdffile) for lipdfile, rdffile in filemap.items()]
         pool = mp.Pool(mp.cpu_count())
         for file in tqdm(pool.imap_unordered(convert_to_rdf, args, chunksize=1), total=len(args)):
             pass
         pool.close()
     else:
         for lipdfile, rdffile in filemap.items():
-            convert_to_rdf(lipdfile, rdffile)
+            convert_to_rdf((lipdfile, rdffile))
 
 
 def convert_lipd_to_graph(lipdfile):
     """Worker that converts one lipdfile to an RDF graph"""
     try:
         converter = LipdToRDF()
         converter.convert(lipdfile)
```

### Comparing `pylipd-1.3.4/pylipd/utils/rdf_graph.py` & `pylipd-1.3.5/pylipd/utils/rdf_graph.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.4/pylipd/utils/rdf_to_lipd.py` & `pylipd-1.3.5/pylipd/utils/rdf_to_lipd.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.4/pylipd/utils/utils.py` & `pylipd-1.3.5/pylipd/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.4/pylipd.egg-info/PKG-INFO` & `pylipd-1.3.5/pylipd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.4
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.5
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.0
```

### Comparing `pylipd-1.3.4/pylipd.egg-info/SOURCES.txt` & `pylipd-1.3.5/pylipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.4/setup.cfg` & `pylipd-1.3.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylipd
-version = 1.3.3
+version = 1.3.5
 author = Varun Ratnakar
 author_email = varunratnakar@gmail.com
 description = Python utilities for handling LiPD data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/linkedearth/pylipd
 project_urls =
```

### Comparing `pylipd-1.3.4/setup.py` & `pylipd-1.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
-
 from setuptools import setup, find_packages
 
-
-version = '1.3.4'
+version = '1.3.5'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pylipd',
```

