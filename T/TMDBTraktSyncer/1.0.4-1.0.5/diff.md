# Comparing `tmp/TMDBTraktSyncer-1.0.4.tar.gz` & `tmp/TMDBTraktSyncer-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.0.4.tar", last modified: Thu May 18 22:27:41 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.0.5.tar", last modified: Thu May 18 22:40:03 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.0.4.tar` & `TMDBTraktSyncer-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 22:27:41.727765 TMDBTraktSyncer-1.0.4/
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 TMDBTraktSyncer-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     6468 2023-05-18 22:27:41.726765 TMDBTraktSyncer-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5795 2023-05-18 21:09:58.000000 TMDBTraktSyncer-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 22:27:41.693766 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0     7096 2023-05-18 21:08:07.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-05-18 21:06:55.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0      517 2023-05-18 22:24:38.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     2997 2023-05-18 21:06:57.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/tmdbRatings.py
--rw-rw-rw-   0        0        0     2181 2023-05-18 21:06:45.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1822 2023-05-18 21:06:52.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-18 22:27:41.724766 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6468 2023-05-18 22:27:41.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-05-18 22:27:41.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 22:27:41.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-18 22:27:41.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 22:27:41.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-18 22:27:41.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 22:27:41.728767 TMDBTraktSyncer-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1291 2023-05-18 22:24:09.000000 TMDBTraktSyncer-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:40:03.477143 TMDBTraktSyncer-1.0.5/
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 TMDBTraktSyncer-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     6468 2023-05-18 22:40:03.476143 TMDBTraktSyncer-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5795 2023-05-18 21:09:58.000000 TMDBTraktSyncer-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 22:40:03.426144 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0     7097 2023-05-18 22:37:55.000000 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-05-18 21:06:55.000000 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0      517 2023-05-18 22:24:38.000000 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     2997 2023-05-18 21:06:57.000000 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/tmdbRatings.py
+-rw-rw-rw-   0        0        0     2181 2023-05-18 21:06:45.000000 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     1822 2023-05-18 21:06:52.000000 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:40:03.473143 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6468 2023-05-18 22:40:03.000000 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-05-18 22:40:03.000000 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 22:40:03.000000 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-18 22:40:03.000000 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 22:40:03.000000 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-18 22:40:03.000000 TMDBTraktSyncer-1.0.5/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 22:40:03.478143 TMDBTraktSyncer-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-05-18 22:38:19.000000 TMDBTraktSyncer-1.0.5/setup.py
```

### Comparing `TMDBTraktSyncer-1.0.4/LICENSE` & `TMDBTraktSyncer-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.4/PKG-INFO` & `TMDBTraktSyncer-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.4
+Version: 1.0.5
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.0.4/README.md` & `TMDBTraktSyncer-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         trakt_access_token = verifyCredentials.trakt_access_token
         tmdb_v4_token = verifyCredentials.tmdb_v4_token
             
         trakt_ratings = traktRatings.getTraktRatings(trakt_client_id, trakt_access_token)
         tmdb_ratings = tmdbRatings.getTMDBRatings(tmdb_v4_token)
 
         #Get trakt and tmdb ratings and filter out trakt ratings with missing tmdb id
-        trakt_ratings = [rating for rating in trak_tratings if rating['ID'] is not None]
+        trakt_ratings = [rating for rating in trakt_tratings if rating['ID'] is not None]
         tmdb_ratings = [rating for rating in tmdb_ratings if rating['ID'] is not None]
         #Filter out ratings already set
         tmdb_ratings_to_set = [rating for rating in trakt_ratings if rating['ID'] not in [tmdb_rating['ID'] for tmdb_rating in tmdb_ratings]]
         trakt_ratings_to_set = [rating for rating in tmdb_ratings if rating['ID'] not in [trakt_rating['ID'] for trakt_rating in trakt_ratings]]
 
         if tmdb_ratings_to_set:
             print('Setting TMDB Ratings')
```

### Comparing `TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/tmdbRatings.py` & `TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/tmdbRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/traktRatings.py` & `TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.0.5/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.0.5/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.4
+Version: 1.0.5
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.0.4/setup.py` & `TMDBTraktSyncer-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

