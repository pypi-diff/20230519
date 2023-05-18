# Comparing `tmp/yambs-1.3.0.tar.gz` & `tmp/yambs-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.3.0.tar", last modified: Thu May 18 09:13:47 2023, max compression
+gzip compressed data, was "yambs-1.3.1.tar", last modified: Thu May 18 23:49:31 2023, max compression
```

## Comparing `yambs-1.3.0.tar` & `yambs-1.3.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:13:47.682656 yambs-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-18 09:12:24.000000 yambs-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-18 09:13:47.678656 yambs-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-18 09:12:24.000000 yambs-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-18 09:12:24.000000 yambs-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 09:13:47.682656 yambs-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-18 09:12:24.000000 yambs-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:13:47.670656 yambs-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-18 09:12:24.000000 yambs-1.3.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-18 09:12:24.000000 yambs-1.3.0/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:13:47.674656 yambs-1.3.0/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:13:47.674656 yambs-1.3.0/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:13:47.674656 yambs-1.3.0/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:13:47.674656 yambs-1.3.0/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:13:47.674656 yambs-1.3.0/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/includes/chips.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:13:47.678656 yambs-1.3.0/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/schemas/Toolchain.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:13:47.678656 yambs-1.3.0/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:13:47.678656 yambs-1.3.0/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/generate/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/generate/ninja.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:13:47.678656 yambs-1.3.0/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-05-18 09:12:24.000000 yambs-1.3.0/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:13:47.674656 yambs-1.3.0/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-18 09:13:47.000000 yambs-1.3.0/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-18 09:13:47.000000 yambs-1.3.0/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:13:47.000000 yambs-1.3.0/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 09:13:47.000000 yambs-1.3.0/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-18 09:13:47.000000 yambs-1.3.0/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 09:13:47.000000 yambs-1.3.0/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.103654 yambs-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-18 23:48:19.000000 yambs-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-18 23:49:31.103654 yambs-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-18 23:48:19.000000 yambs-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-18 23:48:19.000000 yambs-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 23:49:31.103654 yambs-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-18 23:48:19.000000 yambs-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-18 23:48:19.000000 yambs-1.3.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-18 23:48:19.000000 yambs-1.3.1/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/includes/chips.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/schemas/Toolchain.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.103654 yambs-1.3.1/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/data/yambs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.103654 yambs-1.3.1/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/ninja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.103654 yambs-1.3.1/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-18 23:48:19.000000 yambs-1.3.1/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:49:31.099654 yambs-1.3.1/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-18 23:49:31.000000 yambs-1.3.1/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-18 23:49:31.000000 yambs-1.3.1/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:49:31.000000 yambs-1.3.1/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 23:49:31.000000 yambs-1.3.1/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-18 23:49:31.000000 yambs-1.3.1/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 23:49:31.000000 yambs-1.3.1/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.3.0/LICENSE` & `yambs-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/PKG-INFO` & `yambs-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.3.0
+Version: 1.3.1
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=221f06b2074c5386e8c457bcdc2ad511
+    hash=ef7f414918ad82f1abad57ff15edbd1b
     =====================================
 -->
 
-# yambs ([1.3.0](https://pypi.org/project/yambs/))
+# yambs ([1.3.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.3.0/README.md` & `yambs-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=221f06b2074c5386e8c457bcdc2ad511
+    hash=ef7f414918ad82f1abad57ff15edbd1b
     =====================================
 -->
 
-# yambs ([1.3.0](https://pypi.org/project/yambs/))
+# yambs ([1.3.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.3.0/pyproject.toml` & `yambs-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.3.0"
+version = "1.3.1"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.3.0/setup.py` & `yambs-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/tests/test_entry.py` & `yambs-1.3.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/app.py` & `yambs-1.3.1/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/commands/all.py` & `yambs-1.3.1/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/commands/gen.py` & `yambs-1.3.1/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/commands/uf2conv.py` & `yambs-1.3.1/yambs/commands/uf2conv.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,29 +61,31 @@
         elif uf2.is_hex(inpbuf):
             outbuf = uf2.convert_from_hex_to_uf2(inpbuf.decode("utf-8"))
         elif args.carray:
             outbuf = uf2.convert_to_carray(inpbuf)
             ext = "h"
         else:
             outbuf = uf2.convert_to_uf2(inpbuf)
+
         if not args.deploy and not args.info:
             print(
                 (
                     f"Converted to {ext}, output size: {len(outbuf)}, "
                     f"start address: 0x{uf2.APPSTARTADDR:x}"
                 )
             )
         if args.convert or ext != "uf2":
             if args.output is None:  # pragma: nocover
                 args.output = "flash." + ext
+
         if args.output:
             uf2.write_file(args.output, outbuf)
-        if (
-            ext == "uf2" and not args.convert and not args.info
-        ):  # pragma: nocover
+
+        # Deploy the file (if specified).
+        if ext == "uf2" and args.deploy:  # pragma: nocover
             drives = uf2.get_drives()
             if len(drives) == 0:
                 if args.wait:
                     print("Waiting for drive to deploy...")
                     while len(drives) == 0:
                         sleep(0.1)
                         drives = uf2.get_drives()
```

### Comparing `yambs-1.3.0/yambs/config/__init__.py` & `yambs-1.3.1/yambs/config/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,9 +47,12 @@
 
     return Config.create(
         merge(
             _ARBITER.decode(
                 src_config, includes_key="includes", require_success=True
             ).data,
             _ARBITER.decode(path, includes_key="includes").data,
+            # Always allow the project-specific configuration to override
+            # package data.
+            expect_overwrite=True,
         )
     )
```

### Comparing `yambs-1.3.0/yambs/data/includes/chips.yaml` & `yambs-1.3.1/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/data/schemas/Chip.yaml` & `yambs-1.3.1/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/data/schemas/Config.yaml` & `yambs-1.3.1/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/data/templates/rules.ninja.j2` & `yambs-1.3.1/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/data/uf2families.json` & `yambs-1.3.1/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/entry.py` & `yambs-1.3.1/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/generate/__init__.py` & `yambs-1.3.1/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/generate/architectures.py` & `yambs-1.3.1/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/generate/boards.py` & `yambs-1.3.1/yambs/generate/boards.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/generate/chips.py` & `yambs-1.3.1/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/generate/common.py` & `yambs-1.3.1/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/generate/ninja.py` & `yambs-1.3.1/yambs/generate/ninja.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/generate/toolchains.py` & `yambs-1.3.1/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/schemas.py` & `yambs-1.3.1/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-1.3.0/yambs/uf2/__init__.py` & `yambs-1.3.1/yambs/uf2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,16 +306,18 @@
             # NO-flash flag set; skip block
             continue
 
         datalen = header[4]
         if datalen > 476:  # pragma: nocover
             assert False, f"Invalid UF2 data size at {ptr}"
         newaddr = header[3]
+
         if (header[2] & 0x2000) and (currfamilyid is None):
             currfamilyid = header[7]
+
         if curraddr is None or (
             (header[2] & 0x2000) and header[7] != currfamilyid
         ):
             currfamilyid = header[7]
             curraddr = newaddr
             if FAMILYID in [0x0, header[7]]:
                 APPSTARTADDR = newaddr
@@ -343,20 +345,23 @@
         curraddr = newaddr + datalen
         if header[2] & 0x2000:
             if header[7] in families_found:
                 if families_found[header[7]] > newaddr:  # pragma: nocover
                     families_found[header[7]] = newaddr
             else:
                 families_found[header[7]] = newaddr
+
         if prev_flag is None:
             prev_flag = header[2]
         if prev_flag != header[2]:  # pragma: nocover
             all_flags_same = False
+
         if blockno == (numblocks - 1):
             print("--- UF2 File Header Info ---")
+
             families = load_families()
             for family_hex, data in families_found.items():
                 family_short_name = ""
                 for name, value in families.items():
                     if value == family_hex:
                         family_short_name = name
                 print(
```

### Comparing `yambs-1.3.0/yambs.egg-info/PKG-INFO` & `yambs-1.3.1/yambs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.3.0
+Version: 1.3.1
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=221f06b2074c5386e8c457bcdc2ad511
+    hash=ef7f414918ad82f1abad57ff15edbd1b
     =====================================
 -->
 
-# yambs ([1.3.0](https://pypi.org/project/yambs/))
+# yambs ([1.3.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.3.0/yambs.egg-info/SOURCES.txt` & `yambs-1.3.1/yambs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

