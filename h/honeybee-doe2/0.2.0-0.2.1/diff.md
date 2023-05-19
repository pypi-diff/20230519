# Comparing `tmp/honeybee-doe2-0.2.0.tar.gz` & `tmp/honeybee-doe2-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-doe2-0.2.0.tar", last modified: Wed May 17 17:30:32 2023, max compression
+gzip compressed data, was "dist/honeybee-doe2-0.2.1.tar", last modified: Fri May 19 15:14:09 2023, max compression
```

## Comparing `honeybee-doe2-0.2.0.tar` & `honeybee-doe2-0.2.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-17 17:29:25.000000 honeybee-doe2-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-17 17:29:25.000000 honeybee-doe2-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-17 17:29:25.000000 honeybee-doe2-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-17 17:29:25.000000 honeybee-doe2-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-17 17:29:25.000000 honeybee-doe2-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-17 17:29:25.000000 honeybee-doe2-0.2.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/honeybee_doe2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/_extend_honeybee_doe2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/honeybee_doe2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/cli/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/honeybee_doe2/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/geometry/polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/aperture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/constructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/exposedfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/groundcontact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/hvac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/inputils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/inputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/inputils/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/inputils/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/inputils/glass_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/inputils/run_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/inputils/sitebldg.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/inputils/title.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/roof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/shades.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/story.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/properties/wall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/honeybee_doe2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/utils/doe_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/honeybee_doe2/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/honeybee_doe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/honeybee_doe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/honeybee_doe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/honeybee_doe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/honeybee_doe2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/honeybee_doe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/honeybee_doe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 17:30:32.000000 honeybee-doe2-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-17 17:29:26.000000 honeybee-doe2-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/_extend_honeybee_doe2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/cli/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/geometry/polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/constructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/exposedfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/groundcontact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/hvac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/glass_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/run_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/sitebldg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/roof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/shades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/properties/wall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/utils/doe_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/honeybee_doe2/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/honeybee_doe2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 15:14:09.000000 honeybee-doe2-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-19 15:13:12.000000 honeybee-doe2-0.2.1/setup.py
```

### Comparing `honeybee-doe2-0.2.0/LICENSE` & `honeybee-doe2-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/PKG-INFO` & `honeybee-doe2-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.2.0
+Version: 0.2.1
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.2.0/README.md` & `honeybee-doe2-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/_extend_honeybee_doe2.py` & `honeybee-doe2-0.2.1/honeybee_doe2/_extend_honeybee_doe2.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/cli/translate.py` & `honeybee-doe2-0.2.1/honeybee_doe2/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/geometry/polygon.py` & `honeybee-doe2-0.2.1/honeybee_doe2/geometry/polygon.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,44 @@
-from ..utils.doe_formatters import short_name
+import math
+from typing import List
+
 from honeybee.face import Face
-from honeybee.shade import Shade
 from ladybug_geometry.geometry3d import Vector3D, Plane, Face3D
 from ladybug_geometry.geometry2d import Point2D
-import math
+
+from ..utils.doe_formatters import short_name
 
 
 class DoePolygon(object):
     "A Doe2 Polygon."
 
     def __init__(self, name, vertices, flip=False):
         self.name = name
-        self.vertices = vertices
+        self.vertices = self._remove_duplicate_vertices(vertices, 0.001)
         self.flip = flip
 
+    @staticmethod
+    def _remove_duplicate_vertices(vertices: List[Point2D], tol=0.001):
+        """Remove identical vertices.
+
+        Since the list is already sorted we only need to check the vertices with the one
+        that comes before it.
+        """
+        unique_vertices = [vertices[0]]
+        for v in vertices[1:]:
+            if v.distance_to_point(unique_vertices[-1]) < tol:
+                continue
+            unique_vertices.append(v)
+
+        # catch the case when the first and the last vertices are the same
+        if unique_vertices[0].distance_to_point(unique_vertices[-1]) < tol:
+            return unique_vertices[:-1]
+
+        return unique_vertices
+
     @classmethod
     def from_face(cls, face: Face, flip=False):
         """
         Create a DoePolygon from a Honeybee Face.
 
         Args:
             face: A Face object.
```

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/aperture.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/aperture.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                     start_row = last_row + 1
 
         for count, group in enumerate(merged_groups):
             min_2d = group['min']
             max_2d = group['max']
             height = max_2d.y - min_2d.y
             width = max_2d.x - min_2d.x
-            name = f'{short_name(self.aperture.display_name)}_{1000 + count}'
+            name = f'{short_name(self.aperture.display_name, 28)}_{100 + count}'
             window = \
                 '"{}" = WINDOW\n'.format(name) + \
                 "\n  X             = {}".format(min_2d.x) + \
                 "\n  Y             = {}".format(min_2d.y) + \
                 "\n  WIDTH         = {}".format(width, 3) + \
                 "\n  HEIGHT        = {}".format(height, 3) + \
                 '\n  GLASS-TYPE    = "{}"'.format(glass_type) + "\n  ..\n"
```

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/constructions.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/constructions.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/exposedfloor.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/exposedfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/face.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/groundcontact.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/groundcontact.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/hvac.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/hvac.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/inputils/blocks.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/blocks.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/inputils/compliance.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/compliance.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/inputils/glass_types.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/glass_types.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/inputils/run_period.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/run_period.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/inputils/sitebldg.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/inputils/sitebldg.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/materials.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/materials.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/model.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/model.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/roof.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/roof.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/room.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/room.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/shades.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/shades.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/story.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/story.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/properties/wall.py` & `honeybee-doe2-0.2.1/honeybee_doe2/properties/wall.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/utils/doe_formatters.py` & `honeybee-doe2-0.2.1/honeybee_doe2/utils/doe_formatters.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,18 +14,19 @@
     if len(shortened_name) <= max_length:
         return shortened_name
 
     shortened_name = ''.join(shortened_name.split())
     if len(shortened_name) > max_length:
         shortened_name = ''.join(shortened_name.split())
         if len(shortened_name) > max_length:
-            shortened_name = f'{shortened_name[:16]}_{shortened_name[-15:]}'
+            end_length = -1 * (max_length - 17)
+            shortened_name = f'{shortened_name[:16]}_{shortened_name[end_length:]}'
     return shortened_name
 
-#! DF specific
+# ! DF specific
 
 
 def lower_left_properties(room_2d):
     """Get the vertices, boundary conditions and windows starting from lower left.
     v2 WIP
     """
     room_2d.remove_duplicate_vertices()
```

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/utils/geometry.py` & `honeybee-doe2-0.2.1/honeybee_doe2/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2/writer.py` & `honeybee-doe2-0.2.1/honeybee_doe2/writer.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2.egg-info/PKG-INFO` & `honeybee-doe2-0.2.1/honeybee_doe2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.2.0
+Version: 0.2.1
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.2.0/honeybee_doe2.egg-info/SOURCES.txt` & `honeybee-doe2-0.2.1/honeybee_doe2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.2.0/setup.py` & `honeybee-doe2-0.2.1/setup.py`

 * *Files identical despite different names*

