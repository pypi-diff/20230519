# Comparing `tmp/geopyv-0.0.5.tar.gz` & `tmp/geopyv-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopyv-0.0.5.tar", last modified: Tue May 16 10:33:20 2023, max compression
+gzip compressed data, was "geopyv-0.0.6.tar", last modified: Fri May 19 15:00:56 2023, max compression
```

## Comparing `geopyv-0.0.5.tar` & `geopyv-0.0.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:33:20.795104 geopyv-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-16 10:33:07.000000 geopyv-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-16 10:33:07.000000 geopyv-0.0.5/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-16 10:33:07.000000 geopyv-0.0.5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 10:33:07.000000 geopyv-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-16 10:33:20.795104 geopyv-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-16 10:33:07.000000 geopyv-0.0.5/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   167778 2023-05-16 10:33:07.000000 geopyv-0.0.5/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-16 10:33:07.000000 geopyv-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-16 10:33:07.000000 geopyv-0.0.5/basictest.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-16 10:33:07.000000 geopyv-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 10:33:20.795104 geopyv-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-16 10:33:07.000000 geopyv-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:33:20.787104 geopyv-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:33:20.791103 geopyv-0.0.5/src/geopyv/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    28277 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:33:20.795104 geopyv-0.0.5/src/geopyv/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/geometry/exclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/geometry/meshing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/geometry/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:33:20.795104 geopyv-0.0.5/src/geopyv/gui/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:33:20.795104 geopyv-0.0.5/src/geopyv/gui/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/gui/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/gui/selectors/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/gui/selectors/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/gui/selectors/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/gui/selectors/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    71443 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    26841 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39385 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    46343 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/speckle.py
--rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-05-16 10:33:07.000000 geopyv-0.0.5/src/geopyv/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:33:20.791103 geopyv-0.0.5/src/geopyv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-16 10:33:20.000000 geopyv-0.0.5/src/geopyv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-16 10:33:20.000000 geopyv-0.0.5/src/geopyv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:33:20.000000 geopyv-0.0.5/src/geopyv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 10:33:20.000000 geopyv-0.0.5/src/geopyv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 10:33:20.000000 geopyv-0.0.5/src/geopyv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.348039 geopyv-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-19 15:00:42.000000 geopyv-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-19 15:00:42.000000 geopyv-0.0.6/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-19 15:00:42.000000 geopyv-0.0.6/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 15:00:42.000000 geopyv-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-19 15:00:56.348039 geopyv-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-19 15:00:42.000000 geopyv-0.0.6/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   167778 2023-05-19 15:00:42.000000 geopyv-0.0.6/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-19 15:00:42.000000 geopyv-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-05-19 15:00:42.000000 geopyv-0.0.6/basictest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-19 15:00:42.000000 geopyv-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 15:00:56.348039 geopyv-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-19 15:00:42.000000 geopyv-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.340039 geopyv-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.344039 geopyv-0.0.6/src/geopyv/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28277 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.344039 geopyv-0.0.6/src/geopyv/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/geometry/exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/geometry/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/geometry/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.344039 geopyv-0.0.6/src/geopyv/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.348039 geopyv-0.0.6/src/geopyv/gui/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/gui/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/gui/selectors/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/gui/selectors/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/gui/selectors/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/gui/selectors/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71629 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25568 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39385 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47603 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/speckle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-05-19 15:00:42.000000 geopyv-0.0.6/src/geopyv/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:00:56.344039 geopyv-0.0.6/src/geopyv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-19 15:00:56.000000 geopyv-0.0.6/src/geopyv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-19 15:00:56.000000 geopyv-0.0.6/src/geopyv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:00:56.000000 geopyv-0.0.6/src/geopyv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-19 15:00:56.000000 geopyv-0.0.6/src/geopyv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 15:00:56.000000 geopyv-0.0.6/src/geopyv.egg-info/top_level.txt
```

### Comparing `geopyv-0.0.5/.gitignore` & `geopyv-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/CMakeLists.txt` & `geopyv-0.0.6/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/LICENSE` & `geopyv-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/PKG-INFO` & `geopyv-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geopyv
-Version: 0.0.5
+Version: 0.0.6
 Summary: A PIV/DIC analysis package for Python.
 Author-email: Sam Stanier <sas229@cam.ac.uk>, Jonathan Smith <jdks2@cam.ac.uk>
 Project-URL: Homepage, https://github.com/sas229/geopyv
 Project-URL: Bug Tracker, https://github.com/sas229/geopyv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `geopyv-0.0.5/Pipfile` & `geopyv-0.0.6/Pipfile`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/Pipfile.lock` & `geopyv-0.0.6/Pipfile.lock`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954990492373669%*

 * *Differences: {"'default'": "{'astroid': {'hashes': "*

 * *              "['sha256:283cec0fe8ac79d891e0457a15a642caa61ef0efdba0537688762e77479c8d35', "*

 * *              "'sha256:63251dcd00630f80822e52e42377a3163218d0943535caff86b266946b1d48a5'], "*

 * *              "'version': '==3.0.0a3'}, 'docutils': {'hashes': "*

 * *              "['sha256:a428f10de4de4774389734c986a01b4af2d802d26717108b0f1b9356862937c5', "*

 * *              "'sha256:f75a5a52fbcacd81b47e42888ad2b380748aaccfb3f13af0fe69deb759f01eb6'], "*

 * *              "'version': '==0.20'} […]*

```diff
@@ -46,19 +46,19 @@
                 "sha256:96a5ddd5f09534a35f03a8916aeeaac00fe4d6bec2f9ad78f87f57be3007f795"
             ],
             "index": "pypi",
             "version": "==1.3.1"
         },
         "astroid": {
             "hashes": [
-                "sha256:15948c44ce75754a3da761b2aae717401e93997982bac41dae19147e17a60ad7",
-                "sha256:9e650d4ebc67e0054991f4152092cc173519abc97a406558374244968cbefb71"
+                "sha256:283cec0fe8ac79d891e0457a15a642caa61ef0efdba0537688762e77479c8d35",
+                "sha256:63251dcd00630f80822e52e42377a3163218d0943535caff86b266946b1d48a5"
             ],
             "markers": "python_full_version >= '3.8.0'",
-            "version": "==3.0.0a2"
+            "version": "==3.0.0a3"
         },
         "babel": {
             "hashes": [
                 "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
                 "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "markers": "python_version >= '3.7'",
@@ -281,19 +281,19 @@
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
-                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
-                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
+                "sha256:a428f10de4de4774389734c986a01b4af2d802d26717108b0f1b9356862937c5",
+                "sha256:f75a5a52fbcacd81b47e42888ad2b380748aaccfb3f13af0fe69deb759f01eb6"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.19"
+            "version": "==0.20"
         },
         "filelock": {
             "hashes": [
                 "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
                 "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
             ],
             "markers": "python_version >= '3.7'",
@@ -305,19 +305,19 @@
                 "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "index": "pypi",
             "version": "==6.0.0"
         },
         "fonttools": {
             "hashes": [
-                "sha256:64c0c05c337f826183637570ac5ab49ee220eec66cf50248e8df527edfa95aeb",
-                "sha256:9234b9f57b74e31b192c3fc32ef1a40750a8fbc1cd9837a7b7bfc4ca4a5c51d7"
+                "sha256:106caf6167c4597556b31a8d9175a3fdc0356fdcd70ab19973c3b0d4c893c461",
+                "sha256:dba8d7cdb8e2bac1b3da28c5ed5960de09e59a2fe7e63bb73f5a59e57b0430d2"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==4.39.3"
+            "version": "==4.39.4"
         },
         "gmsh": {
             "hashes": [
                 "sha256:69d56865d80e6e7bdb665426333487bc3679bc778b9fee500eb8cf0d2714ad99",
                 "sha256:bde90654db3b8820759d47ad3b309ec0a9ab7c062522c36b84de12bc73719d37",
                 "sha256:df6e401ea3cc6822b2cbff12a3e7fe68e0a11496807bb73f5e31af4496657c0b",
                 "sha256:f07d62ec3ee0edcf1c28ed070ce9eaca86f393e15480edaf37d323f09cc341c1"
@@ -562,19 +562,19 @@
                 "sha256:de346335408f84de0eada6ff9fafafff9bcda11f0a0dfaa931133debb146ab61"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==3.1"
         },
         "nodeenv": {
             "hashes": [
-                "sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e",
-                "sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b"
+                "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2",
+                "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
-            "version": "==1.7.0"
+            "version": "==1.8.0"
         },
         "numpy": {
             "hashes": [
                 "sha256:0ec87a7084caa559c36e0a2309e4ecb1baa03b687201d0a847c8b0ed476a7187",
                 "sha256:1a7d6acc2e7524c9955e5c903160aa4ea083736fde7e91276b0e5d98e6332812",
                 "sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7",
                 "sha256:210461d87fb02a84ef243cac5e814aad2b7f4be953b32cb53327bb49fd77fbb4",
@@ -765,19 +765,19 @@
                 "sha256:3ef6ac33239e4027d9a5598a381b9d30880a1477e50039db2eac6e8a8f6d1b18"
             ],
             "index": "pypi",
             "version": "==23.1.2"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
-                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.0"
+            "version": "==3.5.1"
         },
         "pre-commit": {
             "hashes": [
                 "sha256:218e9e3f7f7f3271ebc355a15598a4d3893ad9fc7b57fe446db75644543323b9",
                 "sha256:733f78c9a056cdd169baa6cd4272d51ecfda95346ef8a89bf93712706021b907"
             ],
             "index": "pypi",
@@ -1083,19 +1083,19 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:283c44aa28922bb4223777b44ac0d59af50a279ac7690dfe945bb2b9575dc41b",
-                "sha256:3cfc1c6756ef1b132687b813ec6ea2214cb7a7e5d1dcb2772006cb895a0fa469"
+                "sha256:60c5e04756c1709a98845ed27a2eed7a556af3993afb66e77fec48189f742616",
+                "sha256:61e025f788c5977d9412587e733733a289e2b9fdc2fef8868ddfbfc4ccfe881d"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==7.0.0"
+            "version": "==7.0.1"
         },
         "sphinx-autoapi": {
             "hashes": [
                 "sha256:5b5c58064214d5a846c9c81d23f00990a64654b9bca10213231db54a241bc50f",
                 "sha256:b25c7b2cda379447b8c36b6a0e3bdf76e02fd64f7ca99d41c6cbdf130a01768f"
             ],
             "index": "pypi",
@@ -1228,19 +1228,19 @@
                 "sha256:d2b89b60fee2f112668117a9f361ceea44a685a37cafd009f396b87b9816efa3"
             ],
             "index": "pypi",
             "version": "==3.1.2"
         },
         "astroid": {
             "hashes": [
-                "sha256:15948c44ce75754a3da761b2aae717401e93997982bac41dae19147e17a60ad7",
-                "sha256:9e650d4ebc67e0054991f4152092cc173519abc97a406558374244968cbefb71"
+                "sha256:283cec0fe8ac79d891e0457a15a642caa61ef0efdba0537688762e77479c8d35",
+                "sha256:63251dcd00630f80822e52e42377a3163218d0943535caff86b266946b1d48a5"
             ],
             "markers": "python_full_version >= '3.8.0'",
-            "version": "==3.0.0a2"
+            "version": "==3.0.0a3"
         },
         "asttokens": {
             "hashes": [
                 "sha256:4622110b2a6f30b77e1473affaa97e711bc2f07d3f10848420ff1898edbe94f3",
                 "sha256:6b0ac9e93fb0335014d382b8fa9b3afa7df546984258005da0b9e7095b3deb1c"
             ],
             "version": "==2.2.1"
@@ -1518,19 +1518,19 @@
                 "sha256:99522ca3e365cac527b44bde033f64c6945d90eb9f769703caaec52b09bbd3ff"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.8.0"
         },
         "docutils": {
             "hashes": [
-                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
-                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
+                "sha256:a428f10de4de4774389734c986a01b4af2d802d26717108b0f1b9356862937c5",
+                "sha256:f75a5a52fbcacd81b47e42888ad2b380748aaccfb3f13af0fe69deb759f01eb6"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.19"
+            "version": "==0.20"
         },
         "exceptiongroup": {
             "hashes": [
                 "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
                 "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
@@ -1565,19 +1565,19 @@
                 "sha256:fe8ea2eca98d8a504f22040d9117347f6b367458366952862ac3586e7d4eeaca"
             ],
             "index": "pypi",
             "version": "==0.3.6"
         },
         "fonttools": {
             "hashes": [
-                "sha256:64c0c05c337f826183637570ac5ab49ee220eec66cf50248e8df527edfa95aeb",
-                "sha256:9234b9f57b74e31b192c3fc32ef1a40750a8fbc1cd9837a7b7bfc4ca4a5c51d7"
+                "sha256:106caf6167c4597556b31a8d9175a3fdc0356fdcd70ab19973c3b0d4c893c461",
+                "sha256:dba8d7cdb8e2bac1b3da28c5ed5960de09e59a2fe7e63bb73f5a59e57b0430d2"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==4.39.3"
+            "version": "==4.39.4"
         },
         "geopyv": {
             "editable": true,
             "path": "."
         },
         "gmsh": {
             "hashes": [
@@ -1625,19 +1625,19 @@
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "ipykernel": {
             "hashes": [
-                "sha256:bd6f487d9e2744c84f6e667d46462d7647a4c862e70e08282f05a52b9d4b705f",
-                "sha256:fc886f1dcdc0ec17f277e4d21fd071c857d381adcb04f3f3735d25325ca323c6"
+                "sha256:1aba0ae8453e15e9bc6b24e497ef6840114afcdb832ae597f32137fa19d42a6f",
+                "sha256:77aeffab056c21d16f1edccdc9e5ccbf7d96eb401bd6703610a21be8b068aadc"
             ],
             "index": "pypi",
-            "version": "==6.23.0"
+            "version": "==6.23.1"
         },
         "ipython": {
             "hashes": [
                 "sha256:7dff3fad32b97f6488e02f87b970f309d082f758d7b7fc252e3b19ee0e432dbb",
                 "sha256:ffca270240fbd21b06b2974e14a86494d6d29290184e788275f55e0b55914926"
             ],
             "markers": "python_version >= '3.9'",
@@ -1890,19 +1890,19 @@
                 "sha256:d267cc1ff794403f7df692964d1d2a3fa9418ffea2a3f6859a439ff482fef290"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.5.6"
         },
         "nodeenv": {
             "hashes": [
-                "sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e",
-                "sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b"
+                "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2",
+                "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
-            "version": "==1.7.0"
+            "version": "==1.8.0"
         },
         "numpy": {
             "hashes": [
                 "sha256:0ec87a7084caa559c36e0a2309e4ecb1baa03b687201d0a847c8b0ed476a7187",
                 "sha256:1a7d6acc2e7524c9955e5c903160aa4ea083736fde7e91276b0e5d98e6332812",
                 "sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7",
                 "sha256:210461d87fb02a84ef243cac5e814aad2b7f4be953b32cb53327bb49fd77fbb4",
@@ -2077,19 +2077,19 @@
                 "sha256:fed1e1cf6a42577953abbe8e6cf2fe2f566daebde7c34724ec8803c4c0cda579"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==9.5.0"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
-                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.0"
+            "version": "==3.5.1"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -2381,19 +2381,19 @@
                 "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.30.0"
         },
         "scikit-build": {
             "hashes": [
-                "sha256:2256f16491da2b5e2ee552a12b71d8bcc2ec6f96f15df9a1d12ce9f4f53df700",
-                "sha256:4bf75dcf628513badb7cc8a926414155ab3db3273f5f8c243092e7a2bdbdd5c9"
+                "sha256:18861286b34fd2d685327d3bec6ebf4d33303adfaef28a08dd856710d16cf20f",
+                "sha256:76856e7631d9e8887a7aa71913d5f184a6177246225391af96ce4801d89fa254"
             ],
             "index": "pypi",
-            "version": "==0.17.3"
+            "version": "==0.17.5"
         },
         "scipy": {
             "hashes": [
                 "sha256:049a8bbf0ad95277ffba9b3b7d23e5369cc39e66406d60422c8cfef40ccc8415",
                 "sha256:07c3457ce0b3ad5124f98a86533106b643dd811dd61b548e78cf4c8786652f6f",
                 "sha256:0f1564ea217e82c1bbe75ddf7285ba0709ecd503f048cb1236ae9995f64217bd",
                 "sha256:1553b5dcddd64ba9a0d95355e63fe6c3fc303a8fd77c7bc91e77d61363f7433f",
@@ -2451,19 +2451,19 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:283c44aa28922bb4223777b44ac0d59af50a279ac7690dfe945bb2b9575dc41b",
-                "sha256:3cfc1c6756ef1b132687b813ec6ea2214cb7a7e5d1dcb2772006cb895a0fa469"
+                "sha256:60c5e04756c1709a98845ed27a2eed7a556af3993afb66e77fec48189f742616",
+                "sha256:61e025f788c5977d9412587e733733a289e2b9fdc2fef8868ddfbfc4ccfe881d"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==7.0.0"
+            "version": "==7.0.1"
         },
         "sphinx-autoapi": {
             "hashes": [
                 "sha256:5b5c58064214d5a846c9c81d23f00990a64654b9bca10213231db54a241bc50f",
                 "sha256:b25c7b2cda379447b8c36b6a0e3bdf76e02fd64f7ca99d41c6cbdf130a01768f"
             ],
             "index": "pypi",
@@ -2562,28 +2562,28 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tornado": {
             "hashes": [
-                "sha256:1285f0691143f7ab97150831455d4db17a267b59649f7bd9700282cba3d5e771",
-                "sha256:3455133b9ff262fd0a75630af0a8ee13564f25fb4fd3d9ce239b8a7d3d027bf8",
-                "sha256:5e2f49ad371595957c50e42dd7e5c14d64a6843a3cf27352b69c706d1b5918af",
-                "sha256:81c17e0cc396908a5e25dc8e9c5e4936e6dfd544c9290be48bd054c79bcad51e",
-                "sha256:90f569a35a8ec19bde53aa596952071f445da678ec8596af763b9b9ce07605e6",
-                "sha256:9661aa8bc0e9d83d757cd95b6f6d1ece8ca9fd1ccdd34db2de381e25bf818233",
-                "sha256:a27a1cfa9997923f80bdd962b3aab048ac486ad8cfb2f237964f8ab7f7eb824b",
-                "sha256:b4e7b956f9b5e6f9feb643ea04f07e7c6b49301e03e0023eedb01fa8cf52f579",
-                "sha256:d7117f3c7ba5d05813b17a1f04efc8e108a1b811ccfddd9134cc68553c414864",
-                "sha256:db181eb3df8738613ff0a26f49e1b394aade05034b01200a63e9662f347d4415",
-                "sha256:ffdce65a281fd708da5a9def3bfb8f364766847fa7ed806821a69094c9629e8a"
+                "sha256:05615096845cf50a895026f749195bf0b10b8909f9be672f50b0fe69cba368e4",
+                "sha256:0c325e66c8123c606eea33084976c832aa4e766b7dff8aedd7587ea44a604cdf",
+                "sha256:29e71c847a35f6e10ca3b5c2990a52ce38b233019d8e858b755ea6ce4dcdd19d",
+                "sha256:4b927c4f19b71e627b13f3db2324e4ae660527143f9e1f2e2fb404f3a187e2ba",
+                "sha256:5b17b1cf5f8354efa3d37c6e28fdfd9c1c1e5122f2cb56dac121ac61baa47cbe",
+                "sha256:6a0848f1aea0d196a7c4f6772197cbe2abc4266f836b0aac76947872cd29b411",
+                "sha256:7efcbcc30b7c654eb6a8c9c9da787a851c18f8ccd4a5a3a95b05c7accfa068d2",
+                "sha256:834ae7540ad3a83199a8da8f9f2d383e3c3d5130a328889e4cc991acc81e87a0",
+                "sha256:b46a6ab20f5c7c1cb949c72c1994a4585d2eaa0be4853f50a03b5031e964fc7c",
+                "sha256:c2de14066c4a38b4ecbbcd55c5cc4b5340eb04f1c5e81da7451ef555859c833f",
+                "sha256:c367ab6c0393d71171123ca5515c61ff62fe09024fa6bf299cd1339dc9456829"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==6.3.1"
+            "version": "==6.3.2"
         },
         "traitlets": {
             "hashes": [
                 "sha256:9e6ec080259b9a5940c797d58b613b5e31441c2257b87c2e795c5228ae80d2d8",
                 "sha256:f6cde21a9c68cf756af02035f72d5a723bf607e862e7be33ece505abf4a3bad9"
             ],
             "markers": "python_version >= '3.7'",
```

### Comparing `geopyv-0.0.5/README.md` & `geopyv-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/basictest.py` & `geopyv-0.0.6/basictest.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 # You can inspect subsets and their convergence
 # via the mesh object by passing a subset number.
 mesh.inspect(subset_index=0)
 mesh.convergence(subset_index=0)
 
 # If you supply a subset index that is out of range you get a ValueError.
-mesh.convergence(subset_index=4000)
+# mesh.convergence(subset_index=4000)
 
 # Sequence test.
 # Sequence setup.
 template = gp.templates.Circle(50)
 boundary = np.asarray(
     [[200.0, 200.0], [200.0, 2700.0], [3900.0, 2700.0], [3900.0, 200.0]]
 )
```

### Comparing `geopyv-0.0.5/pyproject.toml` & `geopyv-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "cmake",
     "ninja"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geopyv"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Sam Stanier", email="sas229@cam.ac.uk" },
   { name="Jonathan Smith", email="jdks2@cam.ac.uk" },
 ]
 description = "A PIV/DIC analysis package for Python."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `geopyv-0.0.5/src/geopyv/__init__.py` & `geopyv-0.0.6/src/geopyv/__init__.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/calibration.py` & `geopyv-0.0.6/src/geopyv/calibration.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/check.py` & `geopyv-0.0.6/src/geopyv/check.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/field.py` & `geopyv-0.0.6/src/geopyv/field.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/geometry/exclusions.py` & `geopyv-0.0.6/src/geopyv/geometry/exclusions.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/geometry/meshing.py` & `geopyv-0.0.6/src/geopyv/geometry/meshing.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/geometry/utilities.py` & `geopyv-0.0.6/src/geopyv/geometry/utilities.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/gui/selectors/coordinate.py` & `geopyv-0.0.6/src/geopyv/gui/selectors/coordinate.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/gui/selectors/file.py` & `geopyv-0.0.6/src/geopyv/gui/selectors/file.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/gui/selectors/folder.py` & `geopyv-0.0.6/src/geopyv/gui/selectors/folder.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/gui/selectors/image.py` & `geopyv-0.0.6/src/geopyv/gui/selectors/image.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/image.py` & `geopyv-0.0.6/src/geopyv/image.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/io.py` & `geopyv-0.0.6/src/geopyv/io.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/log.py` & `geopyv-0.0.6/src/geopyv/log.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/mesh.py` & `geopyv-0.0.6/src/geopyv/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import gmsh
 from copy import deepcopy
 from scipy.optimize import minimize_scalar
 import PIL.Image as ImagePIL
 import PIL.ImageDraw as ImageDrawPIL
 from alive_progress import alive_bar
 import traceback
-import re
 
 log = logging.getLogger(__name__)
 
 
 class MeshBase(Object):
     """
 
@@ -1114,14 +1113,17 @@
             # Pack data.
             self.solved = True
             self.data["nodes"] = self._nodes
             self.data["elements"] = self._elements
             self.data["areas"] = self._areas
             self.data["solved"] = self.solved
             self.data["unsolvable"] = self._unsolvable
+            self.data.update(
+                {"centroids": np.mean(self._nodes[self._elements], axis=-2)}
+            )
 
             # Pack settings.
             self._settings = {
                 "max_iterations": self._max_iterations,
                 "max_norm": self._max_norm,
                 "adaptive_iterations": self._adaptive_iterations,
                 "method": self._method,
@@ -1679,19 +1681,14 @@
                     max_iterations=self._max_iterations,
                     warp_0=np.zeros(np.shape(self._seed_warp)),
                     order=self._subset_order,
                     method=self._method,
                     tolerance=self._seed_tolerance,
                 )
                 if not self._subsets[self._seed_node].data["solved"]:
-                    self._subsets[self._seed_node].convergence(
-                        show=False,
-                        save="convergence_"
-                        + re.findall(r"\d+", self.data["images"]["g_img"])[-1],
-                    )
                     self._update = True
                     log.error(
                         "Specified seed correlation coefficient tolerance not met."
                         "Minimum seed correlation coefficient:"
                         "{seed_C:.2f}; tolerance: {seed_tolerance:.2f}.".format(
                             seed_C=self._subsets[self._seed_node].data["results"][
                                 "C_ZNCC"
@@ -1725,31 +1722,32 @@
                     try:
                         p_0 = self._subsets[cur_idx].data["results"][
                             "p"
                         ]  # Precondition based on selected subset.
                     except Exception:
                         p_0 = self._subsets[self._seed_node].data["results"]["p"]
                     self._subset_solved[cur_idx] = -1  # Set as solved.
-                    solved = self._neighbours(
+                    solvable = self._neighbours(
                         cur_idx, p_0
                     )  # Calculate for neighbouring subsets.
                     count += 1
                     self._bar()
                     if count == number_nodes:
                         break
-                    elif solved is False:
+                    elif solvable is False:
                         break
-
+        if self._subsets[self._seed_node].data["solved"]:
+            self._corrections()
         # Update check.
-        if any(self._subset_solved != -1):
+        if any(self._subset_solved != -1) or any(self._C_ZNCC < self._tolerance):
             self._update = True
             self.solved = False
             self._unsolvable = True
         else:
-            self._corrections()
+            # self._corrections()
             # Compute element areas and strains.
             self._update = False
             self.solved = True
             self._unsolvable = False
             self._element_area()
             self._element_strains()
 
@@ -1775,21 +1773,27 @@
                         max_norm=self._max_norm,
                         max_iterations=self._max_iterations,
                         warp_0=warp,
                         order=self._subset_order,
                         method=self._method,
                         tolerance=self._seed_tolerance,
                     )
-                    if subset._C_ZNCC > self._subsets[idx]._C_ZNCC and subset.solved:
-                        j += 1
-                        self._subsets[idx] = subset
-                        self._store_variables(idx)
+                    try:
+                        if (
+                            subset._C_ZNCC > self._subsets[idx]._C_ZNCC
+                            and subset.solved
+                        ):
+                            j += 1
+                            self._subsets[idx] = subset
+                            self._store_variables(idx, seed=True)
+                    except Exception:
+                        pass
                     bar()
                     bar.text = "{} corrections accepted".format(round(j / (idx + 1), 3))
-            log.info("{} corrections accepted".format(round(j / (idx + 1), 3)))
+            log.info("{ca} corrections accepted".format(ca=round(j / (idx + 1), 3)))
 
     def _connectivity(self, idx):
         """
 
         A private method that returns the indices of nodes connected
         to the index node according to the input array.
 
@@ -1914,15 +1918,15 @@
                         )
                         if self._subsets[idx].data["solved"]:
                             self._store_variables(idx)
                         else:
                             self._C_ZNCC[idx] = np.max(
                                 (self._subsets[idx].data["results"]["C_ZNCC"], 0)
                             )
-                            return False
+        return True
 
     def _store_variables(self, idx, seed=False):
         """
 
         Private method to store variables.
 
         Parameters
```

### Comparing `geopyv-0.0.5/src/geopyv/particle.py` & `geopyv-0.0.6/src/geopyv/particle.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import logging
 import numpy as np
 import geopyv as gp
 from geopyv.object import Object
 import re
 import shapely
 from alive_progress import alive_bar
-import matplotlib.pyplot as plt
 
 log = logging.getLogger(__name__)
 
 
 class ParticleBase(Object):
     """
     Particle base class to be used as a mixin. Contains plot functionality.
@@ -408,17 +407,14 @@
 
         self._coordinates[0] = coordinate_0
         self._warps[0] = warp_0[: np.shape(self._warps)[1]]
         self._volumes[0] = volume_0
         self._stresses[0] = stress_0
 
         self._reference_index = 0
-        self._centroids = np.mean(
-            self._series[0]["nodes"][self._series[0]["elements"]], axis=-2
-        )
         self.solved = False
 
         self._initialised = True
         self.data = {
             "type": "Particle",
             "solved": self.solved,
             "series_type": self._series_type,
@@ -461,46 +457,26 @@
         ----------
         m : int
             Series index.
 
         """
         elements = self._series[m]["elements"]
         nodes = self._series[m]["nodes"]
+        centroids = self._series[m]["centroids"]
         flag = False
-        diff = self._centroids - self._coordinates[self._reference_index]
+        diff = centroids - self._coordinates[self._reference_index]
         dist = np.einsum("ij,ij->i", diff, diff)
         dist_sorted = np.argpartition(dist, 10)
         for index in dist_sorted:
             poly = shapely.Polygon(nodes[elements[index]][:3])
             point = shapely.Point(self._coordinates[self._reference_index])
             if poly.intersects(point):
                 flag = True
                 break
         if flag is False:
-            # for index in dist_sorted:
-            #    print(self._coordinates[self._reference_index])
-            #    print(nodes[elements[index]][:3])
-            #    poly = shapely.Polygon(nodes[elements[index]][:3])
-            #    point = shapely.Point(self._coordinates[self._reference_index])
-            #    print(poly.intersects(point))
-            #    print()
-            #    input()
-            for j in range(len(self._coordinates)):
-                print(j, self._coordinates[j])
-            print(self._reference_index)
-            print(self._coordinates[self._reference_index])
-            print(self._reference_update_register)
-            fig, ax = plt.subplots()
-            ax.scatter(self._coordinates[:m, 0], self._coordinates[:m, 1])
-            for j in range(np.shape(self._series)[0]):
-                ax.plot(
-                    self._series[j]["boundary"][[0, 1, 2, 3, 0], 0],
-                    self._series[j]["boundary"][[0, 1, 2, 3, 0], 1],
-                )
-            plt.show()
             log.error(
                 "Particle {particle} is outside of boundary {boundary}.\n"
                 " Check for convex boundary update.".format(
                     particle=self._coordinates[self._reference_index],
                     boundary=self._series[m]["boundary"],
                 )
             )
@@ -682,30 +658,28 @@
                 re.findall(
                     r"\d+",
                     self._series[self._reference_index]["images"]["f_img"],
                 )[-1]
             ) != int(re.findall(r"\d+", self._series[m]["images"]["f_img"])[-1]):
                 self._reference_index = m
                 self._reference_update_register.append(m)
-                self._centroids = np.mean(
-                    self._series[m]["nodes"][self._series[m]["elements"]], axis=-2
-                )
             # Mesh bearings.
             tri_idx = self._element_locator(m)
             # Interpolation.
             self._warp_increment(m, tri_idx)
+            # print(self._warp_inc)
             # Updates.
             self._coordinates[m + 1] = self._coordinates[
                 self._reference_index
             ] + self._warp_inc[:2] * int(self._track)
             self._warps[m + 1] = self._warps[self._reference_index] + self._warp_inc
             self._volumes[m + 1] = (
-                self._volumes[m]
-                * (1 + (self._warps[m + 1, 2] - self._warps[m, 2]))
-                * (1 + (self._warps[m + 1, 5] - self._warps[m, 5]))
+                self._volumes[self._reference_index]
+                * (1 + self._warp_inc[2])
+                * (1 + self._warp_inc[5])
             )
 
         return True
 
     def _stress_path(self, model, statev, props):
         if model == "Hooke":
             self._E = props["E"]
```

### Comparing `geopyv-0.0.5/src/geopyv/plots.py` & `geopyv-0.0.6/src/geopyv/plots.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/sequence.py` & `geopyv-0.0.6/src/geopyv/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -856,14 +856,15 @@
         mesh_order=2,
         subset_order=1,
         tolerance=0.75,
         seed_tolerance=0.9,
         alpha=0.5,
         track=False,
         hard_boundary=True,
+        rigid=False,
         subset_size_compensation=False,
         guide=False,
     ):
         """
         Method to solve for the sequence.
 
         Parameters
@@ -1043,14 +1044,15 @@
             try:
                 alpha = float(alpha)
                 self._report(gp.check._conversion(alpha, "alpha", float), "Warning")
             except Exception:
                 self._report(check, "TypeError")
         self._report(gp.check._check_range(alpha, "alpha", 0.0, 1.0), "ValueError")
         self._report(gp.check._check_type(track, "track", [bool]), "TypeError")
+        self._report(gp.check._check_type(rigid, "rigid", [bool]), "TypeError")
         self._report(
             gp.check._check_type(hard_boundary, "hard_boundary", [bool]), "TypeError"
         )
         self._report(
             gp.check._check_type(
                 subset_size_compensation, "subset_size_compensation", [bool]
             ),
@@ -1086,14 +1088,15 @@
         self._subset_order = subset_order
         self._mesh_order = mesh_order
         self._tolerance = tolerance
         self._seed_tolerance = seed_tolerance
         self._alpha = alpha
         self._track = track
         self._hard_boundary = hard_boundary
+        self._rigid = rigid
         self._subset_size_compensation = subset_size_compensation
         self._seed_warp = np.zeros(6 * self._subset_order)
 
         # Solve.
         _f_index = 0
         _g_index = 1
         _f_img = gp.image.Image(self._image_dir + self._images[_f_index])
@@ -1209,19 +1212,46 @@
         else:
             previous_mesh = self.data["meshes"][_f_index - 1]
         self._boundary = (
             previous_mesh["nodes"][self._boundary_tags]
             + previous_mesh["results"]["displacements"][self._boundary_tags]
         )
         _exclusions = []
-        for i in range(np.shape(self._exclusions)[0]):
-            _exclusions.append(
-                previous_mesh["nodes"][self._exclusions_tags[i]]
-                + previous_mesh["results"]["displacements"][self._exclusions_tags[i]]
-            )
+        if self._rigid:
+            for i in range(np.shape(self._exclusions)[0]):
+                centre = np.mean(self._exclusions[i], axis=0)
+                local_coordinates = self._exclusions[i] - centre
+                f_img = gp.image.Image(
+                    filepath=previous_mesh["images"]["f_img"],
+                )
+                g_img = gp.image.Image(
+                    filepath=previous_mesh["images"]["g_img"],
+                )
+                subset = gp.subset.Subset(
+                    f_img=f_img,
+                    g_img=g_img,
+                    f_coord=centre,
+                    template=gp.templates.Circle(50),
+                )
+                subset.solve()
+                warp = subset.data["results"]["p"].flatten()
+                theta = (warp[3] - warp[4]) / 2
+                rot = np.asarray(
+                    [[np.cos(theta), np.sin(theta)], [-np.sin(theta), np.cos(theta)]]
+                )
+                centre += warp[:2]
+                _exclusions.append(centre + local_coordinates @ rot)
+        else:
+            for i in range(np.shape(self._exclusions)[0]):
+                _exclusions.append(
+                    previous_mesh["nodes"][self._exclusions_tags[i]]
+                    + previous_mesh["results"]["displacements"][
+                        self._exclusions_tags[i]
+                    ]
+                )
         self._exclusions = _exclusions
 
     def load(self):
         try:
             _meshes = glob.glob("*.pyv", root_dir=self._mesh_dir)
             _mesh_tars = [int(re.findall(r"\d+", x)[-1]) for x in _meshes]
             _mesh_indices_arguments = np.argsort(_mesh_tars)
```

### Comparing `geopyv-0.0.5/src/geopyv/speckle.py` & `geopyv-0.0.6/src/geopyv/speckle.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/subset.py` & `geopyv-0.0.6/src/geopyv/subset.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/templates.py` & `geopyv-0.0.6/src/geopyv/templates.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv/validation.py` & `geopyv-0.0.6/src/geopyv/validation.py`

 * *Files identical despite different names*

### Comparing `geopyv-0.0.5/src/geopyv.egg-info/PKG-INFO` & `geopyv-0.0.6/src/geopyv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geopyv
-Version: 0.0.5
+Version: 0.0.6
 Summary: A PIV/DIC analysis package for Python.
 Author-email: Sam Stanier <sas229@cam.ac.uk>, Jonathan Smith <jdks2@cam.ac.uk>
 Project-URL: Homepage, https://github.com/sas229/geopyv
 Project-URL: Bug Tracker, https://github.com/sas229/geopyv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `geopyv-0.0.5/src/geopyv.egg-info/SOURCES.txt` & `geopyv-0.0.6/src/geopyv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

