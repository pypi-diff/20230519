# Comparing `tmp/ssgpy-0.1.8.tar.gz` & `tmp/ssgpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssgpy-0.1.8.tar", last modified: Fri May 19 15:20:50 2023, max compression
+gzip compressed data, was "ssgpy-0.1.9.tar", last modified: Fri May 19 16:34:07 2023, max compression
```

## Comparing `ssgpy-0.1.8.tar` & `ssgpy-0.1.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.820921 ssgpy-0.1.8/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-12 18:45:07.000000 ssgpy-0.1.8/LICENSE
--rwxr-xr-x   0 mardix     (501) staff       (20)       54 2023-03-13 07:26:52.000000 ssgpy-0.1.8/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1136 2023-05-19 15:20:50.821015 ssgpy-0.1.8/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)     7406 2023-05-19 15:19:49.000000 ssgpy-0.1.8/README.md
--rw-r--r--   0 mardix     (501) staff       (20)      116 2023-03-15 15:53:12.000000 ssgpy-0.1.8/requirements.txt
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-05-19 15:20:50.821497 ssgpy-0.1.8/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)     1727 2023-03-13 07:19:40.000000 ssgpy-0.1.8/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.806523 ssgpy-0.1.8/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.809271 ssgpy-0.1.8/src/ssg/
--rw-r--r--   0 mardix     (501) staff       (20)      636 2023-05-19 15:20:09.000000 ssgpy-0.1.8/src/ssg/__about__.py
--rw-r--r--   0 mardix     (501) staff       (20)       28 2023-03-12 11:59:25.000000 ssgpy-0.1.8/src/ssg/__init__.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.812777 ssgpy-0.1.8/src/ssg/__pycache__/
--rw-r--r--   0 mardix     (501) staff       (20)      775 2023-03-15 18:30:15.000000 ssgpy-0.1.8/src/ssg/__pycache__/__about__.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)      223 2023-03-12 12:03:44.000000 ssgpy-0.1.8/src/ssg/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)    17473 2023-03-16 05:39:25.000000 ssgpy-0.1.8/src/ssg/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)    15441 2023-03-12 03:53:56.000000 ssgpy-0.1.8/src/ssg/__pycache__/ext.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)    29419 2023-03-11 23:46:27.000000 ssgpy-0.1.8/src/ssg/__pycache__/kolibri.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)    19404 2023-03-16 05:39:25.000000 ssgpy-0.1.8/src/ssg/__pycache__/lib.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)    30239 2023-03-12 11:14:09.000000 ssgpy-0.1.8/src/ssg/__pycache__/migos.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)    35122 2023-03-16 07:00:01.000000 ssgpy-0.1.8/src/ssg/__pycache__/ssg.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)     8065 2023-03-12 18:52:02.000000 ssgpy-0.1.8/src/ssg/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 mardix     (501) staff       (20)     8090 2023-03-16 05:21:33.000000 ssgpy-0.1.8/src/ssg/cli.py
--rw-r--r--   0 mardix     (501) staff       (20)     9533 2023-03-12 03:51:00.000000 ssgpy-0.1.8/src/ssg/ext.py
--rw-r--r--   0 mardix     (501) staff       (20)    10616 2023-05-19 15:15:06.000000 ssgpy-0.1.8/src/ssg/lib.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.813412 ssgpy-0.1.8/src/ssg/skel/
--rw-r--r--   0 mardix     (501) staff       (20)     1626 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/README.md
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.814121 ssgpy-0.1.8/src/ssg/skel/content/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2023-03-13 03:17:39.000000 ssgpy-0.1.8/src/ssg/skel/content/hello-world.md
--rw-r--r--   0 mardix     (501) staff       (20)       67 2023-03-13 03:17:39.000000 ssgpy-0.1.8/src/ssg/skel/content/more-details.md
--rw-r--r--   0 mardix     (501) staff       (20)      115 2023-03-13 03:17:39.000000 ssgpy-0.1.8/src/ssg/skel/content/readme.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.814916 ssgpy-0.1.8/src/ssg/skel/data/
--rw-r--r--   0 mardix     (501) staff       (20)      326 2023-03-17 06:36:17.000000 ssgpy-0.1.8/src/ssg/skel/data/articles.json
--rw-r--r--   0 mardix     (501) staff       (20)      118 2023-03-13 03:17:39.000000 ssgpy-0.1.8/src/ssg/skel/data/cars.json
--rw-r--r--   0 mardix     (501) staff       (20)      149 2023-03-13 03:17:39.000000 ssgpy-0.1.8/src/ssg/skel/data/readme.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.817283 ssgpy-0.1.8/src/ssg/skel/pages/
--rw-r--r--   0 mardix     (501) staff       (20)       99 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/_generated.html
--rw-r--r--   0 mardix     (501) staff       (20)      373 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/about.html
--rw-r--r--   0 mardix     (501) staff       (20)     1023 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/advanced.html
--rw-r--r--   0 mardix     (501) staff       (20)      119 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/article_generator.html
--rw-r--r--   0 mardix     (501) staff       (20)     1009 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/contact.html
--rw-r--r--   0 mardix     (501) staff       (20)      441 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/error.html
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.817473 ssgpy-0.1.8/src/ssg/skel/pages/folder2/
--rw-r--r--   0 mardix     (501) staff       (20)       46 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/folder2/index.html
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.817676 ssgpy-0.1.8/src/ssg/skel/pages/folder2/join/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/folder2/join/new-stuff.html
--rw-r--r--   0 mardix     (501) staff       (20)     1815 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/index.html
--rw-r--r--   0 mardix     (501) staff       (20)      136 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/info.md
--rw-r--r--   0 mardix     (501) staff       (20)       60 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/redirectme.html
--rw-r--r--   0 mardix     (501) staff       (20)      159 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/starwars_planet_generator.html
--rw-r--r--   0 mardix     (501) staff       (20)      585 2023-03-17 06:35:48.000000 ssgpy-0.1.8/src/ssg/skel/pages/sub.html
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.817825 ssgpy-0.1.8/src/ssg/skel/plugins/
--rw-r--r--   0 mardix     (501) staff       (20)     1370 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/plugins/default.py
--rw-r--r--   0 mardix     (501) staff       (20)     3026 2023-03-17 06:38:13.000000 ssgpy-0.1.8/src/ssg/skel/ssg.yml
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.806205 ssgpy-0.1.8/src/ssg/skel/static/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.818029 ssgpy-0.1.8/src/ssg/skel/static/css/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/static/css/main.css
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.818155 ssgpy-0.1.8/src/ssg/skel/static/images/
--rw-r--r--   0 mardix     (501) staff       (20)    28358 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/static/images/kolibri.png
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.818411 ssgpy-0.1.8/src/ssg/skel/static/js/
--rw-r--r--   0 mardix     (501) staff       (20)       85 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/static/js/main.js
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.818869 ssgpy-0.1.8/src/ssg/skel/static/vendor/
--rw-r--r--   0 mardix     (501) staff       (20)    30383 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/static/vendor/kolibri.css
--rw-r--r--   0 mardix     (501) staff       (20)     6138 2023-03-13 03:17:40.000000 ssgpy-0.1.8/src/ssg/skel/static/vendor/normalize.css
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.806413 ssgpy-0.1.8/src/ssg/skel/templates/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.819114 ssgpy-0.1.8/src/ssg/skel/templates/layouts/
--rw-r--r--   0 mardix     (501) staff       (20)     6172 2023-03-17 06:37:08.000000 ssgpy-0.1.8/src/ssg/skel/templates/layouts/default.html
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.819423 ssgpy-0.1.8/src/ssg/skel/templates/partials/
--rw-r--r--   0 mardix     (501) staff       (20)      483 2023-03-17 06:37:08.000000 ssgpy-0.1.8/src/ssg/skel/templates/partials/my_table.html
--rw-r--r--   0 mardix     (501) staff       (20)    35553 2023-05-19 15:15:06.000000 ssgpy-0.1.8/src/ssg/ssg.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 15:20:50.820715 ssgpy-0.1.8/src/ssgpy.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1136 2023-05-19 15:20:50.000000 ssgpy-0.1.8/src/ssgpy.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)     1777 2023-05-19 15:20:50.000000 ssgpy-0.1.8/src/ssgpy.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-05-19 15:20:50.000000 ssgpy-0.1.8/src/ssgpy.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       36 2023-05-19 15:20:50.000000 ssgpy-0.1.8/src/ssgpy.egg-info/entry_points.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-03-12 12:03:37.000000 ssgpy-0.1.8/src/ssgpy.egg-info/not-zip-safe
--rw-r--r--   0 mardix     (501) staff       (20)      114 2023-05-19 15:20:50.000000 ssgpy-0.1.8/src/ssgpy.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        4 2023-05-19 15:20:50.000000 ssgpy-0.1.8/src/ssgpy.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.837331 ssgpy-0.1.9/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-12 18:45:07.000000 ssgpy-0.1.9/LICENSE
+-rwxr-xr-x   0 mardix     (501) staff       (20)       54 2023-03-13 07:26:52.000000 ssgpy-0.1.9/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1136 2023-05-19 16:34:07.837439 ssgpy-0.1.9/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)     7406 2023-05-19 15:19:49.000000 ssgpy-0.1.9/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)      116 2023-03-15 15:53:12.000000 ssgpy-0.1.9/requirements.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-05-19 16:34:07.837716 ssgpy-0.1.9/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)     1727 2023-03-13 07:19:40.000000 ssgpy-0.1.9/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.821159 ssgpy-0.1.9/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.823762 ssgpy-0.1.9/src/ssg/
+-rw-r--r--   0 mardix     (501) staff       (20)      636 2023-05-19 16:30:21.000000 ssgpy-0.1.9/src/ssg/__about__.py
+-rw-r--r--   0 mardix     (501) staff       (20)       28 2023-03-12 11:59:25.000000 ssgpy-0.1.9/src/ssg/__init__.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.827839 ssgpy-0.1.9/src/ssg/__pycache__/
+-rw-r--r--   0 mardix     (501) staff       (20)      775 2023-03-15 18:30:15.000000 ssgpy-0.1.9/src/ssg/__pycache__/__about__.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)      223 2023-03-12 12:03:44.000000 ssgpy-0.1.9/src/ssg/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)    17473 2023-03-16 05:39:25.000000 ssgpy-0.1.9/src/ssg/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)    15441 2023-03-12 03:53:56.000000 ssgpy-0.1.9/src/ssg/__pycache__/ext.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)    29419 2023-03-11 23:46:27.000000 ssgpy-0.1.9/src/ssg/__pycache__/kolibri.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)    19404 2023-03-16 05:39:25.000000 ssgpy-0.1.9/src/ssg/__pycache__/lib.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)    30239 2023-03-12 11:14:09.000000 ssgpy-0.1.9/src/ssg/__pycache__/migos.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)    35122 2023-03-16 07:00:01.000000 ssgpy-0.1.9/src/ssg/__pycache__/ssg.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)     8065 2023-03-12 18:52:02.000000 ssgpy-0.1.9/src/ssg/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 mardix     (501) staff       (20)     8478 2023-05-19 16:30:12.000000 ssgpy-0.1.9/src/ssg/cli.py
+-rw-r--r--   0 mardix     (501) staff       (20)     9533 2023-03-12 03:51:00.000000 ssgpy-0.1.9/src/ssg/ext.py
+-rw-r--r--   0 mardix     (501) staff       (20)    10616 2023-05-19 15:15:06.000000 ssgpy-0.1.9/src/ssg/lib.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.828396 ssgpy-0.1.9/src/ssg/skel/
+-rw-r--r--   0 mardix     (501) staff       (20)     1626 2023-03-13 03:17:40.000000 ssgpy-0.1.9/src/ssg/skel/README.md
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.828966 ssgpy-0.1.9/src/ssg/skel/content/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2023-03-13 03:17:39.000000 ssgpy-0.1.9/src/ssg/skel/content/hello-world.md
+-rw-r--r--   0 mardix     (501) staff       (20)       67 2023-03-13 03:17:39.000000 ssgpy-0.1.9/src/ssg/skel/content/more-details.md
+-rw-r--r--   0 mardix     (501) staff       (20)      115 2023-03-13 03:17:39.000000 ssgpy-0.1.9/src/ssg/skel/content/readme.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.829666 ssgpy-0.1.9/src/ssg/skel/data/
+-rw-r--r--   0 mardix     (501) staff       (20)      326 2023-03-17 06:36:17.000000 ssgpy-0.1.9/src/ssg/skel/data/articles.json
+-rw-r--r--   0 mardix     (501) staff       (20)      118 2023-03-13 03:17:39.000000 ssgpy-0.1.9/src/ssg/skel/data/cars.json
+-rw-r--r--   0 mardix     (501) staff       (20)      149 2023-03-13 03:17:39.000000 ssgpy-0.1.9/src/ssg/skel/data/readme.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.832125 ssgpy-0.1.9/src/ssg/skel/pages/
+-rw-r--r--   0 mardix     (501) staff       (20)       99 2023-03-17 06:35:48.000000 ssgpy-0.1.9/src/ssg/skel/pages/_generated.html
+-rw-r--r--   0 mardix     (501) staff       (20)      373 2023-03-17 06:35:48.000000 ssgpy-0.1.9/src/ssg/skel/pages/about.html
+-rw-r--r--   0 mardix     (501) staff       (20)     1023 2023-03-17 06:35:48.000000 ssgpy-0.1.9/src/ssg/skel/pages/advanced.html
+-rw-r--r--   0 mardix     (501) staff       (20)      119 2023-03-17 06:35:48.000000 ssgpy-0.1.9/src/ssg/skel/pages/article_generator.html
+-rw-r--r--   0 mardix     (501) staff       (20)     1009 2023-03-17 06:35:48.000000 ssgpy-0.1.9/src/ssg/skel/pages/contact.html
+-rw-r--r--   0 mardix     (501) staff       (20)      441 2023-03-17 06:35:48.000000 ssgpy-0.1.9/src/ssg/skel/pages/error.html
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.832474 ssgpy-0.1.9/src/ssg/skel/pages/folder2/
+-rw-r--r--   0 mardix     (501) staff       (20)       46 2023-03-17 06:35:48.000000 ssgpy-0.1.9/src/ssg/skel/pages/folder2/index.html
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.832695 ssgpy-0.1.9/src/ssg/skel/pages/folder2/join/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2023-03-17 06:35:48.000000 ssgpy-0.1.9/src/ssg/skel/pages/folder2/join/new-stuff.html
+-rw-r--r--   0 mardix     (501) staff       (20)     1815 2023-03-17 06:35:48.000000 ssgpy-0.1.9/src/ssg/skel/pages/index.html
+-rw-r--r--   0 mardix     (501) staff       (20)      136 2023-03-17 06:35:48.000000 ssgpy-0.1.9/src/ssg/skel/pages/info.md
+-rw-r--r--   0 mardix     (501) staff       (20)       60 2023-03-17 06:35:48.000000 ssgpy-0.1.9/src/ssg/skel/pages/redirectme.html
+-rw-r--r--   0 mardix     (501) staff       (20)      159 2023-03-17 06:35:48.000000 ssgpy-0.1.9/src/ssg/skel/pages/starwars_planet_generator.html
+-rw-r--r--   0 mardix     (501) staff       (20)      585 2023-03-17 06:35:48.000000 ssgpy-0.1.9/src/ssg/skel/pages/sub.html
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.832940 ssgpy-0.1.9/src/ssg/skel/plugins/
+-rw-r--r--   0 mardix     (501) staff       (20)     1370 2023-03-13 03:17:40.000000 ssgpy-0.1.9/src/ssg/skel/plugins/default.py
+-rw-r--r--   0 mardix     (501) staff       (20)     3026 2023-03-17 06:38:13.000000 ssgpy-0.1.9/src/ssg/skel/ssg.yml
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.820917 ssgpy-0.1.9/src/ssg/skel/static/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.833687 ssgpy-0.1.9/src/ssg/skel/static/css/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2023-03-13 03:17:40.000000 ssgpy-0.1.9/src/ssg/skel/static/css/main.css
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.833839 ssgpy-0.1.9/src/ssg/skel/static/images/
+-rw-r--r--   0 mardix     (501) staff       (20)    28358 2023-03-13 03:17:40.000000 ssgpy-0.1.9/src/ssg/skel/static/images/kolibri.png
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.834315 ssgpy-0.1.9/src/ssg/skel/static/js/
+-rw-r--r--   0 mardix     (501) staff       (20)       85 2023-03-13 03:17:40.000000 ssgpy-0.1.9/src/ssg/skel/static/js/main.js
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.835046 ssgpy-0.1.9/src/ssg/skel/static/vendor/
+-rw-r--r--   0 mardix     (501) staff       (20)    30383 2023-03-13 03:17:40.000000 ssgpy-0.1.9/src/ssg/skel/static/vendor/kolibri.css
+-rw-r--r--   0 mardix     (501) staff       (20)     6138 2023-03-13 03:17:40.000000 ssgpy-0.1.9/src/ssg/skel/static/vendor/normalize.css
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.821097 ssgpy-0.1.9/src/ssg/skel/templates/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.835302 ssgpy-0.1.9/src/ssg/skel/templates/layouts/
+-rw-r--r--   0 mardix     (501) staff       (20)     6172 2023-03-17 06:37:08.000000 ssgpy-0.1.9/src/ssg/skel/templates/layouts/default.html
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.835604 ssgpy-0.1.9/src/ssg/skel/templates/partials/
+-rw-r--r--   0 mardix     (501) staff       (20)      483 2023-03-17 06:37:08.000000 ssgpy-0.1.9/src/ssg/skel/templates/partials/my_table.html
+-rw-r--r--   0 mardix     (501) staff       (20)    35553 2023-05-19 15:15:06.000000 ssgpy-0.1.9/src/ssg/ssg.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-19 16:34:07.837162 ssgpy-0.1.9/src/ssgpy.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1136 2023-05-19 16:34:07.000000 ssgpy-0.1.9/src/ssgpy.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)     1777 2023-05-19 16:34:07.000000 ssgpy-0.1.9/src/ssgpy.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-05-19 16:34:07.000000 ssgpy-0.1.9/src/ssgpy.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       36 2023-05-19 16:34:07.000000 ssgpy-0.1.9/src/ssgpy.egg-info/entry_points.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-03-12 12:03:37.000000 ssgpy-0.1.9/src/ssgpy.egg-info/not-zip-safe
+-rw-r--r--   0 mardix     (501) staff       (20)      114 2023-05-19 16:34:07.000000 ssgpy-0.1.9/src/ssgpy.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        4 2023-05-19 16:34:07.000000 ssgpy-0.1.9/src/ssgpy.egg-info/top_level.txt
```

### Comparing `ssgpy-0.1.8/LICENSE` & `ssgpy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/PKG-INFO` & `ssgpy-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssgpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: SSG is an elegant and modern static site generator for the common folks!
 Home-page: https://github.com/mardix/ssg
 Author: Mardix
 Author-email: mardix@illybee.com
 License: MIT
 Keywords: static site generator
 Platform: any
```

### Comparing `ssgpy-0.1.8/README.md` & `ssgpy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/setup.py` & `ssgpy-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/__about__.py` & `ssgpy-0.1.9/src/ssg/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "__email__",
     "__license__",
     "__copyright__",
     "__long_description__"
 ]
 
 __title__ = "SSG"
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 __summary__ = "SSG is an elegant and modern static site generator for the common folks!"
 __uri__ = "https://github.com/mardix/ssg"
 __author__ = "Mardix"
 __email__ = "mardix@illybee.com"
 __license__ = "MIT"
 __copyright__ = "(c) 2023 %s" % __author__
 __long_description__ = """
```

### Comparing `ssgpy-0.1.8/src/ssg/__pycache__/__about__.cpython-311.pyc` & `ssgpy-0.1.9/src/ssg/__pycache__/__about__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/__pycache__/cli.cpython-311.pyc` & `ssgpy-0.1.9/src/ssg/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/__pycache__/ext.cpython-311.pyc` & `ssgpy-0.1.9/src/ssg/__pycache__/ext.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/__pycache__/kolibri.cpython-311.pyc` & `ssgpy-0.1.9/src/ssg/__pycache__/kolibri.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/__pycache__/lib.cpython-311.pyc` & `ssgpy-0.1.9/src/ssg/__pycache__/lib.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/__pycache__/migos.cpython-311.pyc` & `ssgpy-0.1.9/src/ssg/__pycache__/migos.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/__pycache__/ssg.cpython-311.pyc` & `ssgpy-0.1.9/src/ssg/__pycache__/ssg.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/__pycache__/utils.cpython-311.pyc` & `ssgpy-0.1.9/src/ssg/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/cli.py` & `ssgpy-0.1.9/src/ssg/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import os
 import sys
 import time
 import click
 import pkg_resources
 from livereload import Server, shell
-from . import Generator
+from . import Generator, lib
 from .ssg import PAGE_FORMAT
 from .__about__ import *
 
 CWD = os.getcwd()
 
 
 class color:
@@ -133,37 +133,46 @@
 @cli.command("version")
 def version():
     """Return the vesion of SSG"""
     print(__version__)
     footer()
 
 
-@cli.command("create")
-@click.argument("sitename")
-def create_site(sitename):
-    """Create a new site directory and init SSG"""
-    title('Create new site')
+@cli.command("generate")
+@click.option("--sitename", default=None)
+def generate(sitename=None):
+    """Generate a new site directory from --sitename or base_dir in the ssg.yml"""
+    title('Generate new site')
     ssg_conf = os.path.join(CWD, "ssg.yml")
+
     if os.path.isfile(ssg_conf):
-        error_exit("Can't create new site in a directory that contain 'ssg.yml'")
-    
+        if conf := lib.load_conf(ssg_conf):
+            if base_dir := conf.get("base_dir"):
+                sitename = base_dir
+            else:
+                error_exit("SSG already initialized in '%s'. Or delete 'ssg.yml' if a mistake " % CWD)
+    if not sitename:
+        error_exit("sitename or base_dir not set. Use 'ssg init' to initialize in the current directory")
+
     sitepath = os.path.join(CWD, sitename)
-    if os.path.isdir(sitepath):
-        error_exit("Site directory '%s' exists already!" % sitename)
-    else:
-        info("Creating site: %s..." % sitename)
+    if not os.path.isdir(sitepath):
+        info("Generating site: %s..." % sitename)
         os.makedirs(sitepath)
         copy_resource("skel/", sitepath)
         stamp_ssg_current_version(sitepath)
         info("Site created successfully!")
-        info("CD into '%s' and run 'ssg serve' to view the site" % sitename)
+        info("Update the [base_dir:'%s'] in ssg.yml and run 'ssg serve' to view the site" % sitename)
+    else:
+        error_exit("Site directory '%s' exists already!" % sitename)
 
     done()
 
 
+
+
 @cli.command("init")
 def init():
     """Initialize SSG in the current directory """
     title("Init SSG...")
     ssg_conf = os.path.join(CWD, "ssg.yml")
     if os.path.isfile(ssg_conf):
         error_exit("SSG already initialized in '%s'. Or delete 'ssg.yml' if a mistake " % CWD)
@@ -214,14 +223,15 @@
         content += TPL_BODY[markup]
         with open(dest_file, "w") as f:
             f.write(content)
         log("- %s" % page)
     done()
 
 
+
 @cli.command("build")
 @click.option("-i", "--info", is_flag=True)
 @click.option("--env", default=None)
 def build(info, env):
     """Build the site"""
     title("Building site...")
     K = Generator(CWD, {"env": env, "build": "build"})
@@ -229,15 +239,15 @@
     log('Base Url: %s' % K.base_url)
     log('Static Url: %s' % K.static_url)    
     total_pages = K.build(print_info=info)
     log("Total pages: %s" % total_pages)
 
     done()
 
-@cli.command()
+@cli.command("serve")
 @click.option("-p", "--port", default=None)
 @click.option("--no-livereload", default=None)
 @click.option("--open-url", default=None)
 @click.option("--env", default=None)
 def serve(port, no_livereload, open_url, env):
     """Serve the site """
     
@@ -277,17 +287,17 @@
 @cli.command("clean")
 def clean():
     """Clean the build dir """
     title("Cleaning build dir...")
     Generator(CWD).clean_build_dir()
     done()
 
-@cli.command("macros")
+#@cli.command("macros")
 def macros():
-    """Clean the build dir """
+    """ List all macros """
     title("SSG macros")
     K = Generator(CWD)
     macros = K.ssg_macros
     for m in sorted(macros):
         log("- %s: %s" % (m, macros[m]))
     done()
```

### Comparing `ssgpy-0.1.8/src/ssg/ext.py` & `ssgpy-0.1.9/src/ssg/ext.py`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/lib.py` & `ssgpy-0.1.9/src/ssg/lib.py`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/skel/README.md` & `ssgpy-0.1.9/src/ssg/skel/README.md`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/skel/pages/advanced.html` & `ssgpy-0.1.9/src/ssg/skel/pages/advanced.html`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/skel/pages/contact.html` & `ssgpy-0.1.9/src/ssg/skel/pages/contact.html`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/skel/pages/index.html` & `ssgpy-0.1.9/src/ssg/skel/pages/index.html`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/skel/pages/sub.html` & `ssgpy-0.1.9/src/ssg/skel/pages/sub.html`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/skel/plugins/default.py` & `ssgpy-0.1.9/src/ssg/skel/plugins/default.py`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/skel/ssg.yml` & `ssgpy-0.1.9/src/ssg/skel/ssg.yml`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/skel/static/images/kolibri.png` & `ssgpy-0.1.9/src/ssg/skel/static/images/kolibri.png`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/skel/static/vendor/kolibri.css` & `ssgpy-0.1.9/src/ssg/skel/static/vendor/kolibri.css`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/skel/static/vendor/normalize.css` & `ssgpy-0.1.9/src/ssg/skel/static/vendor/normalize.css`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/skel/templates/layouts/default.html` & `ssgpy-0.1.9/src/ssg/skel/templates/layouts/default.html`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssg/ssg.py` & `ssgpy-0.1.9/src/ssg/ssg.py`

 * *Files identical despite different names*

### Comparing `ssgpy-0.1.8/src/ssgpy.egg-info/PKG-INFO` & `ssgpy-0.1.9/src/ssgpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssgpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: SSG is an elegant and modern static site generator for the common folks!
 Home-page: https://github.com/mardix/ssg
 Author: Mardix
 Author-email: mardix@illybee.com
 License: MIT
 Keywords: static site generator
 Platform: any
```

### Comparing `ssgpy-0.1.8/src/ssgpy.egg-info/SOURCES.txt` & `ssgpy-0.1.9/src/ssgpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

