# Comparing `tmp/ssgpy-0.1.7.tar.gz` & `tmp/ssgpy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssgpy-0.1.7.tar", last modified: Fri Mar 17 06:38:45 2023, max compression
+gzip compressed data, was "ssgpy-0.1.8.tar", last modified: Fri May 19 15:20:50 2023, max compression
```

## Comparing `ssgpy-0.1.7.tar` & `ssgpy-0.1.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.605887 ssgpy-0.1.7/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-12 18:45:07.000000 ssgpy-0.1.7/LICENSE
--rwxr-xr-x   0 mardix     (501) staff       (20)       54 2023-03-13 07:26:52.000000 ssgpy-0.1.7/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1136 2023-03-17 06:38:45.605986 ssgpy-0.1.7/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)     7095 2023-03-17 03:43:04.000000 ssgpy-0.1.7/README.md
--rw-r--r--   0 mardix     (501) staff       (20)      116 2023-03-15 15:53:12.000000 ssgpy-0.1.7/requirements.txt
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-03-17 06:38:45.606469 ssgpy-0.1.7/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)     1727 2023-03-13 07:19:40.000000 ssgpy-0.1.7/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.586573 ssgpy-0.1.7/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.589795 ssgpy-0.1.7/src/ssg/
--rw-r--r--   0 mardix     (501) staff       (20)      636 2023-03-17 06:38:39.000000 ssgpy-0.1.7/src/ssg/__about__.py
--rw-r--r--   0 mardix     (501) staff       (20)       28 2023-03-12 11:59:25.000000 ssgpy-0.1.7/src/ssg/__init__.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.594023 ssgpy-0.1.7/src/ssg/__pycache__/
--rw-r--r--   0 mardix     (501) staff       (20)      775 2023-03-15 18:30:15.000000 ssgpy-0.1.7/src/ssg/__pycache__/__about__.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)      223 2023-03-12 12:03:44.000000 ssgpy-0.1.7/src/ssg/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)    17473 2023-03-16 05:39:25.000000 ssgpy-0.1.7/src/ssg/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)    15441 2023-03-12 03:53:56.000000 ssgpy-0.1.7/src/ssg/__pycache__/ext.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)    29419 2023-03-11 23:46:27.000000 ssgpy-0.1.7/src/ssg/__pycache__/kolibri.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)    19404 2023-03-16 05:39:25.000000 ssgpy-0.1.7/src/ssg/__pycache__/lib.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)    30239 2023-03-12 11:14:09.000000 ssgpy-0.1.7/src/ssg/__pycache__/migos.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)    35122 2023-03-16 07:00:01.000000 ssgpy-0.1.7/src/ssg/__pycache__/ssg.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)     8065 2023-03-12 18:52:02.000000 ssgpy-0.1.7/src/ssg/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)     8090 2023-03-16 05:21:33.000000 ssgpy-0.1.7/src/ssg/cli.py
--rw-r--r--   0 mardix     (501) staff       (20)     9533 2023-03-12 03:51:00.000000 ssgpy-0.1.7/src/ssg/ext.py
--rw-r--r--   0 mardix     (501) staff       (20)    10638 2023-03-17 03:25:15.000000 ssgpy-0.1.7/src/ssg/lib.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.594518 ssgpy-0.1.7/src/ssg/skel/
--rw-r--r--   0 mardix     (501) staff       (20)     1626 2023-03-13 03:17:40.000000 ssgpy-0.1.7/src/ssg/skel/README.md
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.595116 ssgpy-0.1.7/src/ssg/skel/content/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2023-03-13 03:17:39.000000 ssgpy-0.1.7/src/ssg/skel/content/hello-world.md
--rw-r--r--   0 mardix     (501) staff       (20)       67 2023-03-13 03:17:39.000000 ssgpy-0.1.7/src/ssg/skel/content/more-details.md
--rw-r--r--   0 mardix     (501) staff       (20)      115 2023-03-13 03:17:39.000000 ssgpy-0.1.7/src/ssg/skel/content/readme.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.595726 ssgpy-0.1.7/src/ssg/skel/data/
--rw-r--r--   0 mardix     (501) staff       (20)      326 2023-03-17 06:36:17.000000 ssgpy-0.1.7/src/ssg/skel/data/articles.json
--rw-r--r--   0 mardix     (501) staff       (20)      118 2023-03-13 03:17:39.000000 ssgpy-0.1.7/src/ssg/skel/data/cars.json
--rw-r--r--   0 mardix     (501) staff       (20)      149 2023-03-13 03:17:39.000000 ssgpy-0.1.7/src/ssg/skel/data/readme.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.598083 ssgpy-0.1.7/src/ssg/skel/pages/
--rw-r--r--   0 mardix     (501) staff       (20)       99 2023-03-17 06:35:48.000000 ssgpy-0.1.7/src/ssg/skel/pages/_generated.html
--rw-r--r--   0 mardix     (501) staff       (20)      373 2023-03-17 06:35:48.000000 ssgpy-0.1.7/src/ssg/skel/pages/about.html
--rw-r--r--   0 mardix     (501) staff       (20)     1023 2023-03-17 06:35:48.000000 ssgpy-0.1.7/src/ssg/skel/pages/advanced.html
--rw-r--r--   0 mardix     (501) staff       (20)      119 2023-03-17 06:35:48.000000 ssgpy-0.1.7/src/ssg/skel/pages/article_generator.html
--rw-r--r--   0 mardix     (501) staff       (20)     1009 2023-03-17 06:35:48.000000 ssgpy-0.1.7/src/ssg/skel/pages/contact.html
--rw-r--r--   0 mardix     (501) staff       (20)      441 2023-03-17 06:35:48.000000 ssgpy-0.1.7/src/ssg/skel/pages/error.html
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.598333 ssgpy-0.1.7/src/ssg/skel/pages/folder2/
--rw-r--r--   0 mardix     (501) staff       (20)       46 2023-03-17 06:35:48.000000 ssgpy-0.1.7/src/ssg/skel/pages/folder2/index.html
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.598525 ssgpy-0.1.7/src/ssg/skel/pages/folder2/join/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2023-03-17 06:35:48.000000 ssgpy-0.1.7/src/ssg/skel/pages/folder2/join/new-stuff.html
--rw-r--r--   0 mardix     (501) staff       (20)     1815 2023-03-17 06:35:48.000000 ssgpy-0.1.7/src/ssg/skel/pages/index.html
--rw-r--r--   0 mardix     (501) staff       (20)      136 2023-03-17 06:35:48.000000 ssgpy-0.1.7/src/ssg/skel/pages/info.md
--rw-r--r--   0 mardix     (501) staff       (20)       60 2023-03-17 06:35:48.000000 ssgpy-0.1.7/src/ssg/skel/pages/redirectme.html
--rw-r--r--   0 mardix     (501) staff       (20)      159 2023-03-17 06:35:48.000000 ssgpy-0.1.7/src/ssg/skel/pages/starwars_planet_generator.html
--rw-r--r--   0 mardix     (501) staff       (20)      585 2023-03-17 06:35:48.000000 ssgpy-0.1.7/src/ssg/skel/pages/sub.html
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.598652 ssgpy-0.1.7/src/ssg/skel/plugins/
--rw-r--r--   0 mardix     (501) staff       (20)     1370 2023-03-13 03:17:40.000000 ssgpy-0.1.7/src/ssg/skel/plugins/default.py
--rw-r--r--   0 mardix     (501) staff       (20)     3026 2023-03-17 06:38:13.000000 ssgpy-0.1.7/src/ssg/skel/ssg.yml
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.586181 ssgpy-0.1.7/src/ssg/skel/static/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.598867 ssgpy-0.1.7/src/ssg/skel/static/css/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2023-03-13 03:17:40.000000 ssgpy-0.1.7/src/ssg/skel/static/css/main.css
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.598982 ssgpy-0.1.7/src/ssg/skel/static/images/
--rw-r--r--   0 mardix     (501) staff       (20)    28358 2023-03-13 03:17:40.000000 ssgpy-0.1.7/src/ssg/skel/static/images/kolibri.png
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.601396 ssgpy-0.1.7/src/ssg/skel/static/js/
--rw-r--r--   0 mardix     (501) staff       (20)       85 2023-03-13 03:17:40.000000 ssgpy-0.1.7/src/ssg/skel/static/js/main.js
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.602889 ssgpy-0.1.7/src/ssg/skel/static/vendor/
--rw-r--r--   0 mardix     (501) staff       (20)    30383 2023-03-13 03:17:40.000000 ssgpy-0.1.7/src/ssg/skel/static/vendor/kolibri.css
--rw-r--r--   0 mardix     (501) staff       (20)     6138 2023-03-13 03:17:40.000000 ssgpy-0.1.7/src/ssg/skel/static/vendor/normalize.css
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.586469 ssgpy-0.1.7/src/ssg/skel/templates/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.603105 ssgpy-0.1.7/src/ssg/skel/templates/layouts/
--rw-r--r--   0 mardix     (501) staff       (20)     6172 2023-03-17 06:37:08.000000 ssgpy-0.1.7/src/ssg/skel/templates/layouts/default.html
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.603376 ssgpy-0.1.7/src/ssg/skel/templates/partials/
--rw-r--r--   0 mardix     (501) staff       (20)      483 2023-03-17 06:37:08.000000 ssgpy-0.1.7/src/ssg/skel/templates/partials/my_table.html
--rw-r--r--   0 mardix     (501) staff       (20)    33993 2023-03-17 06:33:13.000000 ssgpy-0.1.7/src/ssg/ssg.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-03-17 06:38:45.605743 ssgpy-0.1.7/src/ssgpy.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1136 2023-03-17 06:38:45.000000 ssgpy-0.1.7/src/ssgpy.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)     1777 2023-03-17 06:38:45.000000 ssgpy-0.1.7/src/ssgpy.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-03-17 06:38:45.000000 ssgpy-0.1.7/src/ssgpy.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       36 2023-03-17 06:38:45.000000 ssgpy-0.1.7/src/ssgpy.egg-info/entry_points.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-03-12 12:03:37.000000 ssgpy-0.1.7/src/ssgpy.egg-info/not-zip-safe
--rw-r--r--   0 mardix     (501) staff       (20)      114 2023-03-17 06:38:45.000000 ssgpy-0.1.7/src/ssgpy.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        4 2023-03-17 06:38:45.000000 ssgpy-0.1.7/src/ssgpy.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.820921 ssgpy-0.1.8/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-12 18:45:07.000000 ssgpy-0.1.8/LICENSE
+-rwxr-xr-x   0 mardix     (501) staff       (20)       54 2023-03-13 07:26:52.000000 ssgpy-0.1.8/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1136 2023-05-19 15:20:50.821015 ssgpy-0.1.8/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)     7406 2023-05-19 15:19:49.000000 ssgpy-0.1.8/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)      116 2023-03-15 15:53:12.000000 ssgpy-0.1.8/requirements.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-05-19 15:20:50.821497 ssgpy-0.1.8/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)     1727 2023-03-13 07:19:40.000000 ssgpy-0.1.8/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.806523 ssgpy-0.1.8/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.809271 ssgpy-0.1.8/src/ssg/
+-rw-r--r--   0 mardix     (501) staff       (20)      636 2023-05-19 15:20:09.000000 ssgpy-0.1.8/src/ssg/__about__.py
+-rw-r--r--   0 mardix     (501) staff       (20)       28 2023-03-12 11:59:25.000000 ssgpy-0.1.8/src/ssg/__init__.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.812777 ssgpy-0.1.8/src/ssg/__pycache__/
+-rw-r--r--   0 mardix     (501) staff       (20)      775 2023-03-15 18:30:15.000000 ssgpy-0.1.8/src/ssg/__pycache__/__about__.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)      223 2023-03-12 12:03:44.000000 ssgpy-0.1.8/src/ssg/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)    17473 2023-03-16 05:39:25.000000 ssgpy-0.1.8/src/ssg/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)    15441 2023-03-12 03:53:56.000000 ssgpy-0.1.8/src/ssg/__pycache__/ext.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)    29419 2023-03-11 23:46:27.000000 ssgpy-0.1.8/src/ssg/__pycache__/kolibri.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)    19404 2023-03-16 05:39:25.000000 ssgpy-0.1.8/src/ssg/__pycache__/lib.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)    30239 2023-03-12 11:14:09.000000 ssgpy-0.1.8/src/ssg/__pycache__/migos.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)    35122 2023-03-16 07:00:01.000000 ssgpy-0.1.8/src/ssg/__pycache__/ssg.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)     8065 2023-03-12 18:52:02.000000 ssgpy-0.1.8/src/ssg/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)     8090 2023-03-16 05:21:33.000000 ssgpy-0.1.8/src/ssg/cli.py
+-rw-r--r--   0 mardix     (501) staff       (20)     9533 2023-03-12 03:51:00.000000 ssgpy-0.1.8/src/ssg/ext.py
+-rw-r--r--   0 mardix     (501) staff       (20)    10616 2023-05-19 15:15:06.000000 ssgpy-0.1.8/src/ssg/lib.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.813412 ssgpy-0.1.8/src/ssg/skel/
+-rw-r--r--   0 mardix     (501) staff       (20)     1626 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/README.md
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.814121 ssgpy-0.1.8/src/ssg/skel/content/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2023-03-13 03:17:39.000000 ssgpy-0.1.8/src/ssg/skel/content/hello-world.md
+-rw-r--r--   0 mardix     (501) staff       (20)       67 2023-03-13 03:17:39.000000 ssgpy-0.1.8/src/ssg/skel/content/more-details.md
+-rw-r--r--   0 mardix     (501) staff       (20)      115 2023-03-13 03:17:39.000000 ssgpy-0.1.8/src/ssg/skel/content/readme.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.814916 ssgpy-0.1.8/src/ssg/skel/data/
+-rw-r--r--   0 mardix     (501) staff       (20)      326 2023-03-17 06:36:17.000000 ssgpy-0.1.8/src/ssg/skel/data/articles.json
+-rw-r--r--   0 mardix     (501) staff       (20)      118 2023-03-13 03:17:39.000000 ssgpy-0.1.8/src/ssg/skel/data/cars.json
+-rw-r--r--   0 mardix     (501) staff       (20)      149 2023-03-13 03:17:39.000000 ssgpy-0.1.8/src/ssg/skel/data/readme.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.817283 ssgpy-0.1.8/src/ssg/skel/pages/
+-rw-r--r--   0 mardix     (501) staff       (20)       99 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/_generated.html
+-rw-r--r--   0 mardix     (501) staff       (20)      373 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/about.html
+-rw-r--r--   0 mardix     (501) staff       (20)     1023 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/advanced.html
+-rw-r--r--   0 mardix     (501) staff       (20)      119 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/article_generator.html
+-rw-r--r--   0 mardix     (501) staff       (20)     1009 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/contact.html
+-rw-r--r--   0 mardix     (501) staff       (20)      441 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/error.html
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.817473 ssgpy-0.1.8/src/ssg/skel/pages/folder2/
+-rw-r--r--   0 mardix     (501) staff       (20)       46 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/folder2/index.html
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.817676 ssgpy-0.1.8/src/ssg/skel/pages/folder2/join/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/folder2/join/new-stuff.html
+-rw-r--r--   0 mardix     (501) staff       (20)     1815 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/index.html
+-rw-r--r--   0 mardix     (501) staff       (20)      136 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/info.md
+-rw-r--r--   0 mardix     (501) staff       (20)       60 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/redirectme.html
+-rw-r--r--   0 mardix     (501) staff       (20)      159 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/starwars_planet_generator.html
+-rw-r--r--   0 mardix     (501) staff       (20)      585 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/sub.html
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.817825 ssgpy-0.1.8/src/ssg/skel/plugins/
+-rw-r--r--   0 mardix     (501) staff       (20)     1370 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/plugins/default.py
+-rw-r--r--   0 mardix     (501) staff       (20)     3026 2023-03-17 06:38:13.000000 ssgpy-0.1.8/src/ssg/skel/ssg.yml
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.806205 ssgpy-0.1.8/src/ssg/skel/static/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.818029 ssgpy-0.1.8/src/ssg/skel/static/css/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/static/css/main.css
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.818155 ssgpy-0.1.8/src/ssg/skel/static/images/
+-rw-r--r--   0 mardix     (501) staff       (20)    28358 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/static/images/kolibri.png
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.818411 ssgpy-0.1.8/src/ssg/skel/static/js/
+-rw-r--r--   0 mardix     (501) staff       (20)       85 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/static/js/main.js
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.818869 ssgpy-0.1.8/src/ssg/skel/static/vendor/
+-rw-r--r--   0 mardix     (501) staff       (20)    30383 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/static/vendor/kolibri.css
+-rw-r--r--   0 mardix     (501) staff       (20)     6138 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/static/vendor/normalize.css
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.806413 ssgpy-0.1.8/src/ssg/skel/templates/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.819114 ssgpy-0.1.8/src/ssg/skel/templates/layouts/
+-rw-r--r--   0 mardix     (501) staff       (20)     6172 2023-03-17 06:37:08.000000 ssgpy-0.1.8/src/ssg/skel/templates/layouts/default.html
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.819423 ssgpy-0.1.8/src/ssg/skel/templates/partials/
+-rw-r--r--   0 mardix     (501) staff       (20)      483 2023-03-17 06:37:08.000000 ssgpy-0.1.8/src/ssg/skel/templates/partials/my_table.html
+-rw-r--r--   0 mardix     (501) staff       (20)    35553 2023-05-19 15:15:06.000000 ssgpy-0.1.8/src/ssg/ssg.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.820715 ssgpy-0.1.8/src/ssgpy.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1136 2023-05-19 15:20:50.000000 ssgpy-0.1.8/src/ssgpy.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)     1777 2023-05-19 15:20:50.000000 ssgpy-0.1.8/src/ssgpy.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-05-19 15:20:50.000000 ssgpy-0.1.8/src/ssgpy.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       36 2023-05-19 15:20:50.000000 ssgpy-0.1.8/src/ssgpy.egg-info/entry_points.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-03-12 12:03:37.000000 ssgpy-0.1.8/src/ssgpy.egg-info/not-zip-safe
+-rw-r--r--   0 mardix     (501) staff       (20)      114 2023-05-19 15:20:50.000000 ssgpy-0.1.8/src/ssgpy.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        4 2023-05-19 15:20:50.000000 ssgpy-0.1.8/src/ssgpy.egg-info/top_level.txt
```

### Comparing `ssgpy-0.1.7/LICENSE` & `ssgpy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/PKG-INFO` & `ssgpy-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssgpy
-Version: 0.1.7
+Version: 0.1.8
 Summary: SSG is an elegant and modern static site generator for the common folks!
 Home-page: https://github.com/mardix/ssg
 Author: Mardix
 Author-email: mardix@illybee.com
 License: MIT
 Keywords: static site generator
 Platform: any
```

### Comparing `ssgpy-0.1.7/README.md` & `ssgpy-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -346,11 +346,29 @@
 - get_page_url 
 - get_static_url 
 - get_resources 
 - get_static_bundle 
 - format_date
 - current_date
 
+---
+
+## ssg.yml
+
+### ssg.yml advanced
+
+When dealing with multiple build, you can leverage multi directories
+
+
+```
+---
+base_dir: artifact # the directory relative to ssg.yml that contains the artifacts
+build_dir: output # the directory relative to ssg.yml that contains the output
+site:
+    ...
+env:
+    ...
+```
 
 ## TODO
  
 RSS
```

### Comparing `ssgpy-0.1.7/setup.py` & `ssgpy-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/__about__.py` & `ssgpy-0.1.8/src/ssg/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "__email__",
     "__license__",
     "__copyright__",
     "__long_description__"
 ]
 
 __title__ = "SSG"
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 __summary__ = "SSG is an elegant and modern static site generator for the common folks!"
 __uri__ = "https://github.com/mardix/ssg"
 __author__ = "Mardix"
 __email__ = "mardix@illybee.com"
 __license__ = "MIT"
 __copyright__ = "(c) 2023 %s" % __author__
 __long_description__ = """
```

### Comparing `ssgpy-0.1.7/src/ssg/__pycache__/__about__.cpython-311.pyc` & `ssgpy-0.1.8/src/ssg/__pycache__/__about__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/__pycache__/cli.cpython-311.pyc` & `ssgpy-0.1.8/src/ssg/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/__pycache__/ext.cpython-311.pyc` & `ssgpy-0.1.8/src/ssg/__pycache__/ext.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/__pycache__/kolibri.cpython-311.pyc` & `ssgpy-0.1.8/src/ssg/__pycache__/kolibri.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/__pycache__/lib.cpython-311.pyc` & `ssgpy-0.1.8/src/ssg/__pycache__/lib.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/__pycache__/migos.cpython-311.pyc` & `ssgpy-0.1.8/src/ssg/__pycache__/migos.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/__pycache__/ssg.cpython-311.pyc` & `ssgpy-0.1.8/src/ssg/__pycache__/ssg.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/__pycache__/utils.cpython-311.pyc` & `ssgpy-0.1.8/src/ssg/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/cli.py` & `ssgpy-0.1.8/src/ssg/cli.py`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/ext.py` & `ssgpy-0.1.8/src/ssg/ext.py`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/lib.py` & `ssgpy-0.1.8/src/ssg/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             if isinstance(d, dict):
                 return dictdot(d)
             return d
     return None
 
 def load_json_file(file):
     with open(file) as f:
-        if d := json.loads(f.read()):#json_loads(f.read()):
+        if d := json.loads(f.read()):
             if isinstance(d, dict):
                 return dictdot(d)
             return d
     return None
 
 def make_http_requests(url, method="GET", headers=None, data=None, params=None, resolve_path=None, **kw) -> dict:
     """
```

### Comparing `ssgpy-0.1.7/src/ssg/skel/README.md` & `ssgpy-0.1.8/src/ssg/skel/README.md`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/skel/pages/advanced.html` & `ssgpy-0.1.8/src/ssg/skel/pages/advanced.html`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/skel/pages/contact.html` & `ssgpy-0.1.8/src/ssg/skel/pages/contact.html`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/skel/pages/index.html` & `ssgpy-0.1.8/src/ssg/skel/pages/index.html`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/skel/pages/sub.html` & `ssgpy-0.1.8/src/ssg/skel/pages/sub.html`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/skel/plugins/default.py` & `ssgpy-0.1.8/src/ssg/skel/plugins/default.py`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/skel/ssg.yml` & `ssgpy-0.1.8/src/ssg/skel/ssg.yml`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/skel/static/images/kolibri.png` & `ssgpy-0.1.8/src/ssg/skel/static/images/kolibri.png`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/skel/static/vendor/kolibri.css` & `ssgpy-0.1.8/src/ssg/skel/static/vendor/kolibri.css`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/skel/static/vendor/normalize.css` & `ssgpy-0.1.8/src/ssg/skel/static/vendor/normalize.css`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/skel/templates/layouts/default.html` & `ssgpy-0.1.8/src/ssg/skel/templates/layouts/default.html`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.7/src/ssg/ssg.py` & `ssgpy-0.1.8/src/ssg/ssg.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,42 +80,56 @@
         "template": None,       # The page template.
         "sfc": True,            # For single file component
         "__assets": {           # Contains all assets generated
             "js": [],           # List of all js url in the page
             "css": []           # List of all CSS url in the page
         }
     }
+    root_dir = None 
+    base_dir = None
     tpl_env = None
     _templates = {}
     #pages_data__ = {}
 
     def __init__(self, root_dir, options={}):
         """
 
-        :param root_dir: The application root dir
+        :param root_dir: The application root dir, where ssg.yml exists
         :param options: options to build
         """
 
-        self.root_dir = root_dir
-        self.build_dir = os.path.join(self.root_dir, "build")
-        self.static_dir = os.path.join(self.root_dir, "static")
-        self.content_dir = os.path.join(self.root_dir, "content")
-        self.pages_dir = os.path.join(self.root_dir, "pages")
-        self.templates_dir = os.path.join(self.root_dir, "templates")
-        self.data_dir = os.path.join(self.root_dir, "data")
-        self.build_static_dir = os.path.join(self.build_dir, "static")
-        self.build_static_gen_dir = os.path.join(self.build_static_dir, "_gen")
-
+        self.root_dir = self.base_dir = root_dir
         self.config_file = os.path.join(self.root_dir, "ssg.yml")
         self.config = lib.load_conf(self.config_file)
         self.config.setdefault("env", {})
         self.config.setdefault("serve", {})
         self.config.setdefault("build", {})
         self.config.setdefault("globals", {})
         self.config.setdefault("assets_bundles", {})
+
+        # * base_dir
+        # base_dir: relative to the ssg.yml, the dir containing the artifact
+        if base_dir := self.config.get("base_dir"):
+            self.base_dir = os.path.join(self.root_dir, base_dir)
+
+        # * build_dir
+        # build_dir: relative to the ssg.yml, the dir that contains the output
+        if build_dir := self.config.get("build_dir"):
+            self.build_dir = os.path.join(self.root_dir, build_dir)
+        else:
+            self.build_dir = os.path.join(self.base_dir, "_build")
+
+        self.static_dir = os.path.join(self.base_dir, "static")
+        self.content_dir = os.path.join(self.base_dir, "content")
+        self.pages_dir = os.path.join(self.base_dir, "pages")
+        self.templates_dir = os.path.join(self.base_dir, "templates")
+        self.data_dir = os.path.join(self.base_dir, "data")
+        self.build_static_dir = os.path.join(self.build_dir, "static")
+        self.build_static_gen_dir = os.path.join(self.build_static_dir, "_gen")
+
         self.layout = self.config.get("globals.layout", DEFAULT_LAYOUT)
 
         build_type = options.get("build", "build")
 
         self.build_config = lib.dictdot(self.config[build_type])
         site_env = self.build_config.get("env")
         if options and options.get("env") is not None:
@@ -395,16 +409,25 @@
                     """
                     #!== Generator 
                     Generators generates pages from data sources.
                     A data source can be from the data folder, or from a `data_requests` in ssg.yml
 
                     Properties:
                         - resources: somename_from_dataDir_or_remoteResources
-                        - type: single|paged
+                        - type: single|list
 
+                    # single 
+                    To display a single entry. 
+                    The page reference will be $pagename:$page_id or a $permalink
+
+                    # list
+                    To create a list of item. 
+                    Optionally, individual pages can exist for more details
+                    href = $pagename:page_num or $permalink
+                    
 
                     Example: 
                     Having the data `data/articles.json` -> [{title, slug, content, ...},...]
                     and the page `pages/article_generator.html`
 
                     ``` pages/article_generator.html
                     ---
@@ -424,16 +447,17 @@
                     _gen_type = _generator.get("type", "single") # The generator type: single|list
                     _resources_name = _generator.get("resources")
                     rdata = resources__.get(_resources_name)
                     # expecting data to be a list to iterate over
                     if not isinstance(rdata, list):
                         raise Exception("BUILD ERROR: Generator data type must be of List|Array for '%s'" % _resources_name)
 
-                    # SINGLE
+                    # ::SINGLE
                     # generates single pages off of the data
+
                     if not _gen_type or _gen_type.upper() == "SINGLE":
                         
                         for data in rdata:
                             dmeta = copy.deepcopy(mdata)
 
                             for _ in special_meta:
                                 if _ in data:
@@ -465,18 +489,27 @@
                                 },
                                 "content": mdata.get("content"),
                                 "markup": mdata.get("markup"),
                                 "template": mdata.get("template"),
                                 "layout": mdata.get("layout") or self.layout
                             })
    
-                    # LIST
+                    # ::LIST
+                    # To create a paginated listing page similar to a blog page. 
+                    # Each page will contain a chunk list of the data
+                    # This can be use to show a list.
+                    # NOTE: While a list contain the list of the content, 
+                    # it's can be necessary to create another Generator to show single/indivual page.
+                    # This way you can link to them.
+                    #
+                    #
                     # create a paginated with [Prev] [Next]
                     # Each page will contain a chunk of the data
-                    # will split the content into multi pages
+                    # will split the content into multi pages.
+                    # Also a index/default page will be created for the first page
                     if _gen_type.upper() == "LIST":
                         raise NotImplementedError()
 
                         per_page = int(_generator.get(
                             "per_page", self.site_config.get("pagination.per_page", 10)))
                         left_edge = int(_generator.get(
                             "left_edge", self.site_config.get("pagination.left_edge", 2)))
@@ -516,14 +549,15 @@
                             current_page = i + 1
                             prev_page = current_page - 1
                             has_prev_page = prev_page < 0
                             next_page = current_page + 1
                             has_next_page = next_page < total_pages
 
                             pagination = {
+                                "items_per_page": per_page,
                                 "current_page": current_page,
                                 "prev_page": prev_page,
                                 "has_prev_page": has_prev_page,
                                 "next_page": next_page,
                                 "has_next_page": has_next_page
                             }
```

### Comparing `ssgpy-0.1.7/src/ssgpy.egg-info/PKG-INFO` & `ssgpy-0.1.8/src/ssgpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssgpy
-Version: 0.1.7
+Version: 0.1.8
 Summary: SSG is an elegant and modern static site generator for the common folks!
 Home-page: https://github.com/mardix/ssg
 Author: Mardix
 Author-email: mardix@illybee.com
 License: MIT
 Keywords: static site generator
 Platform: any
```

### Comparing `ssgpy-0.1.7/src/ssgpy.egg-info/SOURCES.txt` & `ssgpy-0.1.8/src/ssgpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

