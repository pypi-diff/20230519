# Comparing `tmp/TMDBTraktSyncer-1.0.3.tar.gz` & `tmp/TMDBTraktSyncer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.0.3.tar", last modified: Thu May 18 21:31:09 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.0.4.tar", last modified: Thu May 18 22:27:41 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.0.3.tar` & `TMDBTraktSyncer-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 21:31:09.963621 TMDBTraktSyncer-1.0.3/
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 TMDBTraktSyncer-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     6472 2023-05-18 21:31:09.962624 TMDBTraktSyncer-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5795 2023-05-18 21:09:58.000000 TMDBTraktSyncer-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 21:31:09.941454 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0     7096 2023-05-18 21:08:07.000000 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-05-18 21:06:55.000000 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0      464 2023-05-18 21:07:12.000000 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     2997 2023-05-18 21:06:57.000000 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer/tmdbRatings.py
--rw-rw-rw-   0        0        0     2181 2023-05-18 21:06:45.000000 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1822 2023-05-18 21:06:52.000000 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:31:09.960620 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6472 2023-05-18 21:31:09.000000 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-05-18 21:31:09.000000 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 21:31:09.000000 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-18 21:31:09.000000 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 21:31:09.000000 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-18 21:31:09.000000 TMDBTraktSyncer-1.0.3/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 21:31:09.963621 TMDBTraktSyncer-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1295 2023-05-18 21:30:54.000000 TMDBTraktSyncer-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:27:41.727765 TMDBTraktSyncer-1.0.4/
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 TMDBTraktSyncer-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     6468 2023-05-18 22:27:41.726765 TMDBTraktSyncer-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5795 2023-05-18 21:09:58.000000 TMDBTraktSyncer-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 22:27:41.693766 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0     7096 2023-05-18 21:08:07.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-05-18 21:06:55.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0      517 2023-05-18 22:24:38.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     2997 2023-05-18 21:06:57.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/tmdbRatings.py
+-rw-rw-rw-   0        0        0     2181 2023-05-18 21:06:45.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     1822 2023-05-18 21:06:52.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:27:41.724766 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6468 2023-05-18 22:27:41.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-05-18 22:27:41.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 22:27:41.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-18 22:27:41.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 22:27:41.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-18 22:27:41.000000 TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 22:27:41.728767 TMDBTraktSyncer-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-05-18 22:24:09.000000 TMDBTraktSyncer-1.0.4/setup.py
```

### Comparing `TMDBTraktSyncer-1.0.3/LICENSE` & `TMDBTraktSyncer-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.3/PKG-INFO` & `TMDBTraktSyncer-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.3
+Version: 1.0.4
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # TMDB-Trakt-Syncer
 
 This Python script syncs user ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
```

### Comparing `TMDBTraktSyncer-1.0.3/README.md` & `TMDBTraktSyncer-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.3/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.3/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.3/TMDBTraktSyncer/tmdbRatings.py` & `TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/tmdbRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.3/TMDBTraktSyncer/traktRatings.py` & `TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.3/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.0.4/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.3/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.0.4/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.3
+Version: 1.0.4
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # TMDB-Trakt-Syncer
 
 This Python script syncs user ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Ratings already set will not be overwritten. The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
```

### Comparing `TMDBTraktSyncer-1.0.3/setup.py` & `TMDBTraktSyncer-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
@@ -31,9 +31,9 @@
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
             'TMDBTraktSyncer = TMDBTraktSyncer.TMDBTraktSyncer:main'
         ]
     },
-    python_requires='>=3.6, <4'
+    python_requires='>=3.6'
 )
```

