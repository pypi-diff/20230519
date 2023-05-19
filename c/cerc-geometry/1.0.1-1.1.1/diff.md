# Comparing `tmp/cerc-geometry-1.0.1.tar.gz` & `tmp/cerc-geometry-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-mrjemjyz/cerc-geometry-1.0.1.tar", last modified: Tue May 16 00:07:09 2023, max compression
+gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-ut4epg4e/cerc-geometry-1.1.1.tar", last modified: Thu May 18 23:55:06 2023, max compression
```

## Comparing `cerc-geometry-1.0.1.tar` & `cerc-geometry-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-16 00:07:09.424671 cerc-geometry-1.0.1/
--rw-r--r--   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-1.0.1/LICENSE.md
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-16 00:07:09.424296 cerc-geometry-1.0.1/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-1.0.1/README.md
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-16 00:07:09.414983 cerc-geometry-1.0.1/cerc_geometry.egg-info/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-16 00:07:09.000000 cerc-geometry-1.0.1/cerc_geometry.egg-info/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      472 2023-05-16 00:07:09.000000 cerc-geometry-1.0.1/cerc_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-16 00:07:09.000000 cerc-geometry-1.0.1/cerc_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       41 2023-05-16 00:07:09.000000 cerc-geometry-1.0.1/cerc_geometry.egg-info/requires.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-16 00:07:09.000000 cerc-geometry-1.0.1/cerc_geometry.egg-info/top_level.txt
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-16 00:07:09.419933 cerc-geometry-1.0.1/geometry/
--rw-r--r--   0 peteryefi   (501) staff       (20)      140 2023-05-15 23:39:05.000000 cerc-geometry-1.0.1/geometry/__init__.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     5398 2023-05-16 00:05:51.000000 cerc-geometry-1.0.1/geometry/helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-1.0.1/geometry/plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-1.0.1/geometry/point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-1.0.1/geometry/polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-1.0.1/geometry/polyhedron.py
--rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-1.0.1/pyproject.toml
--rw-r--r--   0 peteryefi   (501) staff       (20)       30 2023-05-12 21:28:55.000000 cerc-geometry-1.0.1/requirements.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-16 00:07:09.424796 cerc-geometry-1.0.1/setup.cfg
--rw-r--r--   0 peteryefi   (501) staff       (20)     1320 2023-05-16 00:06:45.000000 cerc-geometry-1.0.1/setup.py
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-16 00:07:09.423680 cerc-geometry-1.0.1/tests/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-1.0.1/tests/test_helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-1.0.1/tests/test_plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-1.0.1/tests/test_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-1.0.1/tests/test_polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-1.0.1/tests/test_polyhedron.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-18 23:55:06.803742 cerc-geometry-1.1.1/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-1.1.1/LICENSE.md
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-18 23:55:06.803324 cerc-geometry-1.1.1/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-1.1.1/README.md
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-18 23:55:06.789291 cerc-geometry-1.1.1/cerc_geometry.egg-info/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-18 23:55:06.000000 cerc-geometry-1.1.1/cerc_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      535 2023-05-18 23:55:06.000000 cerc-geometry-1.1.1/cerc_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-18 23:55:06.000000 cerc-geometry-1.1.1/cerc_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       48 2023-05-18 23:55:06.000000 cerc-geometry-1.1.1/cerc_geometry.egg-info/requires.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-18 23:55:06.000000 cerc-geometry-1.1.1/cerc_geometry.egg-info/top_level.txt
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-18 23:55:06.797139 cerc-geometry-1.1.1/geometry/
+-rw-r--r--   0 peteryefi   (501) staff       (20)      140 2023-05-15 23:39:05.000000 cerc-geometry-1.1.1/geometry/__init__.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     5398 2023-05-16 00:05:51.000000 cerc-geometry-1.1.1/geometry/helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    11268 2023-05-18 23:49:06.000000 cerc-geometry-1.1.1/geometry/library.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      574 2023-05-18 23:39:06.000000 cerc-geometry-1.1.1/geometry/location.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      707 2023-05-18 23:38:20.000000 cerc-geometry-1.1.1/geometry/map_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-1.1.1/geometry/plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-1.1.1/geometry/point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-1.1.1/geometry/polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-1.1.1/geometry/polyhedron.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-1.1.1/pyproject.toml
+-rw-r--r--   0 peteryefi   (501) staff       (20)       37 2023-05-18 23:51:47.000000 cerc-geometry-1.1.1/requirements.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-18 23:55:06.803888 cerc-geometry-1.1.1/setup.cfg
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1320 2023-05-18 23:51:29.000000 cerc-geometry-1.1.1/setup.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-18 23:55:06.802554 cerc-geometry-1.1.1/tests/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-1.1.1/tests/test_helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-1.1.1/tests/test_plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-1.1.1/tests/test_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-1.1.1/tests/test_polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-1.1.1/tests/test_polyhedron.py
```

### Comparing `cerc-geometry-1.0.1/LICENSE.md` & `cerc-geometry-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.0.1/PKG-INFO` & `cerc-geometry-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 1.0.1
+Version: 1.1.1
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-1.0.1/README.md` & `cerc-geometry-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.0.1/cerc_geometry.egg-info/PKG-INFO` & `cerc-geometry-1.1.1/cerc_geometry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 1.0.1
+Version: 1.1.1
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-1.0.1/geometry/helper.py` & `cerc-geometry-1.1.1/geometry/helper.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.0.1/geometry/plane.py` & `cerc-geometry-1.1.1/geometry/plane.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.0.1/geometry/point.py` & `cerc-geometry-1.1.1/geometry/point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.0.1/geometry/polygon.py` & `cerc-geometry-1.1.1/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.0.1/geometry/polyhedron.py` & `cerc-geometry-1.1.1/geometry/polyhedron.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.0.1/setup.py` & `cerc-geometry-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     for requirement
     in pkg_resources.parse_requirements(r)
   ]
 install_requires.append('setuptools')
 
 setuptools.setup(
   name="cerc-geometry",
-  version="1.0.1",
+  version="1.1.1",
   author="CERC",
   author_email=" cerc@concordia.ca",
   description="CERC Geometry Library with different modules to manipulate geometric objects",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry",
   project_urls={
```

### Comparing `cerc-geometry-1.0.1/tests/test_helper.py` & `cerc-geometry-1.1.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.0.1/tests/test_plane.py` & `cerc-geometry-1.1.1/tests/test_plane.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.0.1/tests/test_point.py` & `cerc-geometry-1.1.1/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.0.1/tests/test_polygon.py` & `cerc-geometry-1.1.1/tests/test_polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-1.0.1/tests/test_polyhedron.py` & `cerc-geometry-1.1.1/tests/test_polyhedron.py`

 * *Files identical despite different names*

