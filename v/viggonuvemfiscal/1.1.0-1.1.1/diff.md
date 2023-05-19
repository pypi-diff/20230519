# Comparing `tmp/viggonuvemfiscal-1.1.0.tar.gz` & `tmp/viggonuvemfiscal-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggonuvemfiscal-1.1.0.tar", last modified: Mon May 15 19:46:30 2023, max compression
+gzip compressed data, was "viggonuvemfiscal-1.1.1.tar", last modified: Fri May 19 12:05:28 2023, max compression
```

## Comparing `viggonuvemfiscal-1.1.0.tar` & `viggonuvemfiscal-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.043693 viggonuvemfiscal-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-15 19:46:30.043693 viggonuvemfiscal-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:46:30.043693 viggonuvemfiscal-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.039693 viggonuvemfiscal-1.1.0/viggonuvemfiscal/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.039693 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.039693 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.039693 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.043693 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.039693 viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-15 19:46:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-15 19:46:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:46:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-15 19:46:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 19:46:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/viggonuvemfiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18422 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 12:05:28.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-19 12:05:28.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:05:28.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 12:05:28.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 12:05:28.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/top_level.txt
```

### Comparing `viggonuvemfiscal-1.1.0/viggonuvemfiscal/__init__.py` & `viggonuvemfiscal-1.1.1/viggonuvemfiscal/__init__.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.0/viggonuvemfiscal/resources.py` & `viggonuvemfiscal-1.1.1/viggonuvemfiscal/resources.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py` & `viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py` & `viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py` & `viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/SOURCES.txt` & `viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

