# Comparing `tmp/honeybee-doe2-0.2.1.tar.gz` & `tmp/honeybee-doe2-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-doe2-0.2.1.tar", last modified: Fri May 19 15:14:09 2023, max compression
+gzip compressed data, was "dist/honeybee-doe2-0.3.0.tar", last modified: Fri May 19 16:28:11 2023, max compression
```

## Comparing `honeybee-doe2-0.2.1.tar` & `honeybee-doe2-0.3.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/_extend_honeybee_doe2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/cli/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/geometry/polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/aperture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/constructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/exposedfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/groundcontact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/hvac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/glass_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/run_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/sitebldg.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/title.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/roof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/shades.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/story.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/wall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/utils/doe_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/honeybee_doe2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/_extend_honeybee_doe2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/honeybee_doe2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/cli/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/honeybee_doe2/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/geometry/polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/constructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/exposedfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/groundcontact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/hvac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/inputils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/inputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/inputils/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/inputils/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/inputils/glass_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/inputils/run_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/inputils/sitebldg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/inputils/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/roof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/shades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/properties/wall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/honeybee_doe2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/utils/doe_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/honeybee_doe2/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/honeybee_doe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/honeybee_doe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/honeybee_doe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/honeybee_doe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/honeybee_doe2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/honeybee_doe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/honeybee_doe2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 16:28:11.000000 honeybee-doe2-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-19 16:27:17.000000 honeybee-doe2-0.3.0/setup.py
```

### Comparing `honeybee-doe2-0.2.1/LICENSE` & `honeybee-doe2-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/PKG-INFO` & `honeybee-doe2-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.2.1
+Version: 0.3.0
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.2.1/README.md` & `honeybee-doe2-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/_extend_honeybee_doe2.py` & `honeybee-doe2-0.3.0/honeybee_doe2/_extend_honeybee_doe2.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/cli/translate.py` & `honeybee-doe2-0.3.0/honeybee_doe2/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/geometry/polygon.py` & `honeybee-doe2-0.3.0/honeybee_doe2/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/aperture.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/constructions.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/constructions.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/exposedfloor.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/exposedfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/face.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/groundcontact.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/groundcontact.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/hvac.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/hvac.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/blocks.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/inputils/blocks.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/compliance.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/inputils/compliance.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/glass_types.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/inputils/glass_types.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/run_period.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/inputils/run_period.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/sitebldg.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/inputils/sitebldg.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/materials.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/materials.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/model.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """ HB-Model Doe2 (eQuest) Properties."""
 from collections import defaultdict
 
 from honeybee.model import Model
 from honeybee.room import Room
 from honeybee.face import Face
 from honeybee_energy.construction.opaque import OpaqueConstruction
+from honeybee_energy.lib.constructionsets import generic_construction_set
 
 from .inputils import blocks as fb
 from .inputils.compliance import ComplianceData
 from .inputils.sitebldg import SiteBldgData as sbd
 from .inputils.run_period import RunPeriod
 from .inputils.title import Title
 
@@ -77,19 +78,27 @@
     @property
     def mats_cons_layers(self):
         return self._make_mats_cons_layers(self.host)
 
     @staticmethod
     def _make_mats_cons_layers(obj):
         cons = []
+        for construction in generic_construction_set.wall_set.constructions:
+            if isinstance(construction, OpaqueConstruction):
+                cons.append(construction)
+        for construction in generic_construction_set.floor_set.constructions:
+            if isinstance(construction, OpaqueConstruction):
+                cons.append(construction)
+        for construction in generic_construction_set.roof_ceiling_set.constructions:
+            if isinstance(construction, OpaqueConstruction):
+                cons.append(construction)
         for construction in obj.properties.energy.constructions:
             if isinstance(construction, OpaqueConstruction):
                 cons.append(construction)
         return ConstructionCollection.from_hb_constructions(constructions=cons).to_inp()
-        # return '\n'.join([l for l in cons])
 
     @property
     def hvac_sys_zones(self):
         return self._get_hvac_sys_zones(self.stories)
 
     @staticmethod
     def _get_hvac_sys_zones(stories):
```

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/roof.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/roof.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/room.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/room.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/shades.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/shades.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/story.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/story.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/properties/wall.py` & `honeybee-doe2-0.3.0/honeybee_doe2/properties/wall.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/utils/doe_formatters.py` & `honeybee-doe2-0.3.0/honeybee_doe2/utils/doe_formatters.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/utils/geometry.py` & `honeybee-doe2-0.3.0/honeybee_doe2/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2/writer.py` & `honeybee-doe2-0.3.0/honeybee_doe2/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .properties.inputils.run_period import RunPeriod
 from .properties.inputils.title import Title
 from .properties.inputils.glass_types import GlassType
 from .utils.doe_formatters import short_name
 
 from honeybee.model import Model
 from honeybee_energy.construction.window import WindowConstruction
+from honeybee_energy.lib.constructionsets import generic_construction_set
 from honeybee.boundarycondition import Surface
 
 
 def model_to_inp(hb_model):
     # type: (Model) -> str
     rp = RunPeriod()
     comp_data = ComplianceData()
@@ -52,16 +53,17 @@
                 else:
                     face_dir = 'W'
                 thestr = f'{room_name}_{i}_{str(face.type)}{ii}_{face_dir}'.replace(
                     ' ', '_')
                 thestr.replace('&', '')
                 face.display_name = short_name(thestr)
 
-    # TODO: Add routine to 'reverbose' constr/matters prior to writing to inp
-    window_constructions = []
+    window_constructions = [GlassType.from_hb_window_constr(
+        generic_construction_set.aperture_set.window_construction)]
+
     for construction in hb_model.properties.energy.constructions:
         if isinstance(construction, WindowConstruction):
             window_constructions.append(GlassType.from_hb_window_constr(construction))
 
     data = [
         hb_model.properties.doe2._header,
         fb.global_params,
```

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2.egg-info/PKG-INFO` & `honeybee-doe2-0.3.0/honeybee_doe2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.2.1
+Version: 0.3.0
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.2.1/honeybee_doe2.egg-info/SOURCES.txt` & `honeybee-doe2-0.3.0/honeybee_doe2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.1/setup.py` & `honeybee-doe2-0.3.0/setup.py`

 * *Files identical despite different names*

