# Comparing `tmp/PlexPreferNonForcedSubs-2.1.6.tar.gz` & `tmp/PlexPreferNonForcedSubs-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlexPreferNonForcedSubs-2.1.6.tar", last modified: Thu May 18 22:12:15 2023, max compression
+gzip compressed data, was "PlexPreferNonForcedSubs-2.1.7.tar", last modified: Thu May 18 22:46:17 2023, max compression
```

## Comparing `PlexPreferNonForcedSubs-2.1.6.tar` & `PlexPreferNonForcedSubs-2.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 22:12:15.904514 PlexPreferNonForcedSubs-2.1.6/
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.1.6/LICENSE
--rw-rw-rw-   0        0        0     6139 2023-05-18 22:12:15.904514 PlexPreferNonForcedSubs-2.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 22:12:15.870506 PlexPreferNonForcedSubs-2.1.6/PlexPreferNonForcedSubs/
--rw-rw-rw-   0        0        0     7502 2023-05-18 21:59:15.000000 PlexPreferNonForcedSubs-2.1.6/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
--rw-rw-rw-   0        0        0        0 2023-05-18 18:48:34.000000 PlexPreferNonForcedSubs-2.1.6/PlexPreferNonForcedSubs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 22:12:15.902515 PlexPreferNonForcedSubs-2.1.6/PlexPreferNonForcedSubs.egg-info/
--rw-rw-rw-   0        0        0     6139 2023-05-18 22:12:15.000000 PlexPreferNonForcedSubs-2.1.6/PlexPreferNonForcedSubs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-05-18 22:12:15.000000 PlexPreferNonForcedSubs-2.1.6/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 22:12:15.000000 PlexPreferNonForcedSubs-2.1.6/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-05-18 22:12:15.000000 PlexPreferNonForcedSubs-2.1.6/PlexPreferNonForcedSubs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 22:12:15.000000 PlexPreferNonForcedSubs-2.1.6/PlexPreferNonForcedSubs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-18 22:12:15.000000 PlexPreferNonForcedSubs-2.1.6/PlexPreferNonForcedSubs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5455 2023-05-18 22:03:50.000000 PlexPreferNonForcedSubs-2.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-18 22:12:15.905504 PlexPreferNonForcedSubs-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1546 2023-05-18 22:12:04.000000 PlexPreferNonForcedSubs-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:46:17.818896 PlexPreferNonForcedSubs-2.1.7/
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.1.7/LICENSE
+-rw-rw-rw-   0        0        0     6139 2023-05-18 22:46:17.818896 PlexPreferNonForcedSubs-2.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 22:46:17.785897 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs/
+-rw-rw-rw-   0        0        0     7512 2023-05-18 22:42:10.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 18:48:34.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 22:46:17.815895 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/
+-rw-rw-rw-   0        0        0     6139 2023-05-18 22:46:17.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-05-18 22:46:17.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 22:46:17.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-05-18 22:46:17.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 22:46:17.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-18 22:46:17.000000 PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5455 2023-05-18 22:03:50.000000 PlexPreferNonForcedSubs-2.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 22:46:17.819896 PlexPreferNonForcedSubs-2.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1546 2023-05-18 22:43:08.000000 PlexPreferNonForcedSubs-2.1.7/setup.py
```

### Comparing `PlexPreferNonForcedSubs-2.1.6/LICENSE` & `PlexPreferNonForcedSubs-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexPreferNonForcedSubs-2.1.6/PKG-INFO` & `PlexPreferNonForcedSubs-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.1.6
+Version: 2.1.7
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexPreferNonForcedSubs-2.1.6/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py` & `PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     print("-" * 50)
     print(traceback_info)
     print("-" * 50)
     print(f"Submit the error here: {github_issue_url}")
     print("-" * 50)
 
 def main():
+    try:
         # Connect to Plex Media Server. Replace PLEX_TOKEN below with your Plex token. How to get token: https://www.plexopedia.com/plex-media-server/general/plex-token/
         baseurl = 'http://localhost:32400'
         token = 'PLEX_TOKEN'
 
         script_dir = os.path.dirname(os.path.abspath(__file__))
         token_file = os.path.join(script_dir, 'token.txt')
```

### Comparing `PlexPreferNonForcedSubs-2.1.6/PlexPreferNonForcedSubs.egg-info/PKG-INFO` & `PlexPreferNonForcedSubs-2.1.7/PlexPreferNonForcedSubs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.1.6
+Version: 2.1.7
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexPreferNonForcedSubs-2.1.6/README.md` & `PlexPreferNonForcedSubs-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `PlexPreferNonForcedSubs-2.1.6/setup.py` & `PlexPreferNonForcedSubs-2.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '2.1.6'
+VERSION = '2.1.7'
 DESCRIPTION = 'This script will set all movies and shows in your local Plex library to English non forced subtitles by default.'
 LONG_DESCRIPTION = 'This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices.'
 
 # Setting up
 setup(
     name="PlexPreferNonForcedSubs",
     version=VERSION,
```

