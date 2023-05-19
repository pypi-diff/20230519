# Comparing `tmp/laff-0.5.0.tar.gz` & `tmp/laff-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laff-0.5.0.tar", last modified: Wed Nov  9 16:10:16 2022, max compression
+gzip compressed data, was "laff-0.6.0.tar", max compression
```

## Comparing `laff-0.5.0.tar` & `laff-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,5 @@
-drwxr-xr-x   0 ah724    (38450) _lpoperator   (100)        0 2022-11-09 16:10:16.158693 laff-0.5.0/
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)    35129 2022-07-21 15:30:45.000000 laff-0.5.0/LICENSE
--rw-rw-r--   0 ah724    (38450) _lpoperator   (100)       15 2022-06-01 14:54:00.000000 laff-0.5.0/MANIFEST.in
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)      408 2022-11-09 16:10:16.158498 laff-0.5.0/PKG-INFO
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)        1 2022-10-06 13:42:25.000000 laff-0.5.0/README.rst
-drwxr-xr-x   0 ah724    (38450) _lpoperator   (100)        0 2022-11-09 16:10:16.156438 laff-0.5.0/laff/
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)        0 2022-07-21 15:41:38.000000 laff-0.5.0/laff/__init__.py
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)      134 2022-07-21 15:41:28.000000 laff-0.5.0/laff/__main__.py
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)     2949 2022-10-06 13:43:09.000000 laff-0.5.0/laff/bulklc.py
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)    21420 2022-11-09 16:04:27.000000 laff-0.5.0/laff/laff.py
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)     3240 2022-11-09 15:18:40.000000 laff-0.5.0/laff/lcimport.py
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)     3195 2022-11-09 15:28:44.000000 laff-0.5.0/laff/models.py
-drwxr-xr-x   0 ah724    (38450) _lpoperator   (100)        0 2022-11-09 16:10:16.158271 laff-0.5.0/laff.egg-info/
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)      408 2022-11-09 16:10:15.000000 laff-0.5.0/laff.egg-info/PKG-INFO
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)      303 2022-11-09 16:10:16.000000 laff-0.5.0/laff.egg-info/SOURCES.txt
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)        1 2022-11-09 16:10:15.000000 laff-0.5.0/laff.egg-info/dependency_links.txt
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)       40 2022-11-09 16:10:15.000000 laff-0.5.0/laff.egg-info/entry_points.txt
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)       84 2022-11-09 16:10:16.000000 laff-0.5.0/laff.egg-info/requires.txt
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)        5 2022-11-09 16:10:16.000000 laff-0.5.0/laff.egg-info/top_level.txt
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)       38 2022-11-09 16:10:16.158750 laff-0.5.0/setup.cfg
--rw-r--r--   0 ah724    (38450) _lpoperator   (100)      973 2022-09-06 16:49:52.000000 laff-0.5.0/setup.py
+-rw-r--r--   0        0        0     2642 2023-04-10 13:43:40.172834 laff-0.6.0/README.md
+-rw-r--r--   0        0        0       31 2023-05-19 17:34:57.346443 laff-0.6.0/laff/__init__.py
+-rw-r--r--   0        0        0     1482 2023-05-19 18:24:22.268766 laff-0.6.0/laff/lcimport.py
+-rw-r--r--   0        0        0      410 2023-05-19 18:24:16.448792 laff-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 laff-0.6.0/PKG-INFO
```

