# Comparing `tmp/agsi-1.0.6.tar.gz` & `tmp/agsi-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-1.0.6.tar", last modified: Fri May 19 03:59:55 2023, max compression
+gzip compressed data, was "agsi-1.0.7.tar", last modified: Fri May 19 06:23:02 2023, max compression
```

## Comparing `agsi-1.0.6.tar` & `agsi-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-19 03:59:55.590041 agsi-1.0.6/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-17 09:39:46.000000 agsi-1.0.6/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-19 03:59:55.590041 agsi-1.0.6/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.0.6/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-19 03:59:55.590041 agsi-1.0.6/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.0.6/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-19 03:59:55.590041 agsi-1.0.6/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    14072 2023-05-19 03:58:21.000000 agsi-1.0.6/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.0.6/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.0.6/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)   970300 2023-05-18 10:02:54.000000 agsi-1.0.6/agsi/demo_V2.ipynb
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.0.6/agsi/main.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-17 09:13:44.000000 agsi-1.0.6/agsi/requirements.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-19 03:59:55.590041 agsi-1.0.6/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-19 03:59:55.000000 agsi-1.0.6/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-05-19 03:59:55.000000 agsi-1.0.6/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-19 03:59:55.000000 agsi-1.0.6/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-19 03:59:55.000000 agsi-1.0.6/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-19 03:59:55.000000 agsi-1.0.6/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-19 03:59:55.590041 agsi-1.0.6/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      369 2023-05-19 03:59:52.000000 agsi-1.0.6/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-19 06:23:02.423539 agsi-1.0.7/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-17 09:39:46.000000 agsi-1.0.7/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-19 06:23:02.423539 agsi-1.0.7/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.0.7/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-19 06:23:02.419538 agsi-1.0.7/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.0.7/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-19 06:23:02.423539 agsi-1.0.7/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    14080 2023-05-19 06:21:26.000000 agsi-1.0.7/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.0.7/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.0.7/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)   970300 2023-05-18 10:02:54.000000 agsi-1.0.7/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.0.7/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-17 09:13:44.000000 agsi-1.0.7/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-19 06:23:02.419538 agsi-1.0.7/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-19 06:23:02.000000 agsi-1.0.7/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-05-19 06:23:02.000000 agsi-1.0.7/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-19 06:23:02.000000 agsi-1.0.7/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-19 06:23:02.000000 agsi-1.0.7/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-19 06:23:02.000000 agsi-1.0.7/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-19 06:23:02.423539 agsi-1.0.7/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      369 2023-05-19 06:22:02.000000 agsi-1.0.7/setup.py
```

### Comparing `agsi-1.0.6/README.md` & `agsi-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `agsi-1.0.6/agsi/data/FarmData.py` & `agsi-1.0.7/agsi/data/FarmData.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,17 +143,17 @@
                         if row[key]:
                             data_path[key] = row[key]
                         else:
                             data_path[key] = ""
 
                 # Extract satellite image paths or shp files
                 if row['sat_planet']:
-                    data_path['planet'] = row['sat_planet']
+                    data_path['sat_planet'] = row['sat_planet']
                 else:
-                    data_path['planet'] = ""
+                    data_path['sat_planet'] = ""
 
                 if row['sat_sentinel2']:
                     data_path['sentinel_2'] =row['sat_sentinel2']
                 else:
                     data_path['sentinel_2'] =""
 
                 # Create output dictionary for block
```

### Comparing `agsi-1.0.6/agsi/data/utils.py` & `agsi-1.0.7/agsi/data/utils.py`

 * *Files identical despite different names*

### Comparing `agsi-1.0.6/agsi/demo_V2.ipynb` & `agsi-1.0.7/agsi/demo_V2.ipynb`

 * *Files identical despite different names*

