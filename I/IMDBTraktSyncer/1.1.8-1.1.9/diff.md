# Comparing `tmp/IMDBTraktSyncer-1.1.8.tar.gz` & `tmp/IMDBTraktSyncer-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.1.8.tar", last modified: Thu May 18 21:41:01 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.1.9.tar", last modified: Thu May 18 22:19:29 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.1.8.tar` & `IMDBTraktSyncer-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 21:41:01.304183 IMDBTraktSyncer-1.1.8/
-drwxrwxrwx   0        0        0        0 2023-05-18 21:41:01.282190 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    11742 2023-05-18 21:40:27.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-18 18:50:40.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1794 2023-05-18 18:50:40.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4079 2023-05-18 18:50:40.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0      464 2023-05-18 21:36:57.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     2256 2023-05-18 18:50:40.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/imdbRatings.py
--rw-rw-rw-   0        0        0     1846 2023-05-18 18:50:40.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     2524 2023-05-18 18:50:40.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:41:01.302183 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     7733 2023-05-18 21:41:01.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-05-18 21:41:01.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 21:41:01.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-18 21:41:01.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-18 21:41:01.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-18 21:41:01.000000 IMDBTraktSyncer-1.1.8/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-05-18 18:50:40.000000 IMDBTraktSyncer-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     7733 2023-05-18 21:41:01.303184 IMDBTraktSyncer-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     7069 2023-05-18 18:50:40.000000 IMDBTraktSyncer-1.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-18 21:41:01.304183 IMDBTraktSyncer-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1321 2023-05-18 21:40:46.000000 IMDBTraktSyncer-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:19:29.555166 IMDBTraktSyncer-1.1.9/
+drwxrwxrwx   0        0        0        0 2023-05-18 22:19:29.522167 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    11742 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1794 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4079 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0      517 2023-05-18 22:18:58.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     2256 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/imdbRatings.py
+-rw-rw-rw-   0        0        0     1846 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     2524 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:19:29.553166 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     7729 2023-05-18 22:19:29.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-05-18 22:19:29.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 22:19:29.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-18 22:19:29.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-18 22:19:29.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-18 22:19:29.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     7729 2023-05-18 22:19:29.554166 IMDBTraktSyncer-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7069 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 22:19:29.555166 IMDBTraktSyncer-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-05-18 22:18:00.000000 IMDBTraktSyncer-1.1.9/setup.py
```

### Comparing `IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/imdbRatings.py` & `IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/imdbRatings.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/traktRatings.py` & `IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.1.8/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.1.8/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.1.8
+Version: 1.1.9
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDB-Trakt-Syncer
 This Python script syncs user ratings for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Ratings already set will not be overwritten. The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
```

### Comparing `IMDBTraktSyncer-1.1.8/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.1.8/LICENSE` & `IMDBTraktSyncer-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.1.8/PKG-INFO` & `IMDBTraktSyncer-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.1.8
+Version: 1.1.9
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDB-Trakt-Syncer
 This Python script syncs user ratings for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Ratings already set will not be overwritten. The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
```

### Comparing `IMDBTraktSyncer-1.1.8/README.md` & `IMDBTraktSyncer-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.1.8/setup.py` & `IMDBTraktSyncer-1.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.8'
+VERSION = '1.1.9'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
@@ -31,9 +31,9 @@
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
             'IMDBTraktSyncer = IMDBTraktSyncer.IMDBTraktSyncer:main'
         ]
     },
-    python_requires='>=3.6, <4'
+    python_requires='>=3.6'
 )
```

