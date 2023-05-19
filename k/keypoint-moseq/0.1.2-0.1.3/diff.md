# Comparing `tmp/keypoint-moseq-0.1.2.tar.gz` & `tmp/keypoint-moseq-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypoint-moseq-0.1.2.tar", last modified: Fri May 12 21:11:44 2023, max compression
+gzip compressed data, was "keypoint-moseq-0.1.3.tar", last modified: Fri May 19 14:10:19 2023, max compression
```

## Comparing `keypoint-moseq-0.1.2.tar` & `keypoint-moseq-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-12 21:11:44.508317 keypoint-moseq-0.1.2/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.2/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.2/NOTICE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-12 21:11:44.508450 keypoint-moseq-0.1.2/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1426 2023-05-11 19:57:02.000000 keypoint-moseq-0.1.2/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-12 21:11:44.509549 keypoint-moseq-0.1.2/keypoint_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1007 2023-05-11 19:55:30.000000 keypoint-moseq-0.1.2/keypoint_moseq/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-05-12 21:11:44.509630 keypoint-moseq-0.1.2/keypoint_moseq/_version.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-05-04 21:42:40.000000 keypoint-moseq-0.1.2/keypoint_moseq/analysis.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17681 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.2/keypoint_moseq/calibration.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17318 2023-05-11 19:55:30.000000 keypoint-moseq-0.1.2/keypoint_moseq/fitting.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    41843 2023-05-11 21:25:41.000000 keypoint-moseq-0.1.2/keypoint_moseq/io.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    27401 2023-05-11 19:55:30.000000 keypoint-moseq-0.1.2/keypoint_moseq/util.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    68259 2023-05-12 18:45:18.000000 keypoint-moseq-0.1.2/keypoint_moseq/viz.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-12 21:11:44.507974 keypoint-moseq-0.1.2/keypoint_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-12 21:11:44.000000 keypoint-moseq-0.1.2/keypoint_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      455 2023-05-12 21:11:44.000000 keypoint-moseq-0.1.2/keypoint_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-05-12 21:11:44.000000 keypoint-moseq-0.1.2/keypoint_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      170 2023-05-12 21:11:44.000000 keypoint-moseq-0.1.2/keypoint_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-05-12 21:11:44.000000 keypoint-moseq-0.1.2/keypoint_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      752 2023-05-12 21:11:44.509184 keypoint-moseq-0.1.2/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      246 2023-05-04 21:42:40.000000 keypoint-moseq-0.1.2/setup.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.2/versioneer.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-19 14:10:19.455508 keypoint-moseq-0.1.3/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.3/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.3/NOTICE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-19 14:10:19.455619 keypoint-moseq-0.1.3/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1426 2023-05-16 23:54:35.000000 keypoint-moseq-0.1.3/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-19 14:10:19.456438 keypoint-moseq-0.1.3/keypoint_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1007 2023-05-18 03:06:07.000000 keypoint-moseq-0.1.3/keypoint_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-05-19 14:10:19.456518 keypoint-moseq-0.1.3/keypoint_moseq/_version.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-05-18 03:06:07.000000 keypoint-moseq-0.1.3/keypoint_moseq/analysis.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17681 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.3/keypoint_moseq/calibration.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17318 2023-05-16 23:54:35.000000 keypoint-moseq-0.1.3/keypoint_moseq/fitting.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    41843 2023-05-16 23:54:35.000000 keypoint-moseq-0.1.3/keypoint_moseq/io.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    27401 2023-05-18 03:06:07.000000 keypoint-moseq-0.1.3/keypoint_moseq/util.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    68264 2023-05-19 14:06:57.000000 keypoint-moseq-0.1.3/keypoint_moseq/viz.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-19 14:10:19.455263 keypoint-moseq-0.1.3/keypoint_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-19 14:10:19.000000 keypoint-moseq-0.1.3/keypoint_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      455 2023-05-19 14:10:19.000000 keypoint-moseq-0.1.3/keypoint_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-05-19 14:10:19.000000 keypoint-moseq-0.1.3/keypoint_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      170 2023-05-19 14:10:19.000000 keypoint-moseq-0.1.3/keypoint_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-05-19 14:10:19.000000 keypoint-moseq-0.1.3/keypoint_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      752 2023-05-19 14:10:19.456155 keypoint-moseq-0.1.3/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      246 2023-05-18 03:06:07.000000 keypoint-moseq-0.1.3/setup.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.3/versioneer.py
```

### Comparing `keypoint-moseq-0.1.2/LICENSE.md` & `keypoint-moseq-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.2/NOTICE.md` & `keypoint-moseq-0.1.3/NOTICE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.2/README.md` & `keypoint-moseq-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.2/keypoint_moseq/__init__.py` & `keypoint-moseq-0.1.3/keypoint_moseq/__init__.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.2/keypoint_moseq/analysis.py` & `keypoint-moseq-0.1.3/keypoint_moseq/analysis.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.2/keypoint_moseq/calibration.py` & `keypoint-moseq-0.1.3/keypoint_moseq/calibration.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.2/keypoint_moseq/fitting.py` & `keypoint-moseq-0.1.3/keypoint_moseq/fitting.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.2/keypoint_moseq/io.py` & `keypoint-moseq-0.1.3/keypoint_moseq/io.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.2/keypoint_moseq/util.py` & `keypoint-moseq-0.1.3/keypoint_moseq/util.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.2/keypoint_moseq/viz.py` & `keypoint-moseq-0.1.3/keypoint_moseq/viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -657,16 +657,16 @@
         Window size is rounded up to the nearest multiple of `blocksize`.
     """
     all_trajectories = get_trajectories(
         sum(sampled_instances.values(), []), coordinates, pre=pre, 
         post=post, centroids=centroids, headings=headings)
     
     all_trajectories = np.concatenate(all_trajectories, axis=0)
-    ax_distances = np.max(np.abs(all_trajectories), axis=1)
-    window_size = np.percentile(ax_distances, pctl) * fudge_factor * 2
+    max_distances = np.nanmax(np.abs(all_trajectories), axis=1)
+    window_size = np.percentile(max_distances, pctl) * fudge_factor * 2
     window_size = int(np.ceil(window_size / blocksize) * blocksize)
     return window_size
 
 
 def generate_grid_movies(
     results=None, output_dir=None, name=None, project_dir=None,
     results_path=None, video_dir=None, video_paths=None, rows=4,
```

### Comparing `keypoint-moseq-0.1.2/setup.cfg` & `keypoint-moseq-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.2/versioneer.py` & `keypoint-moseq-0.1.3/versioneer.py`

 * *Files identical despite different names*

