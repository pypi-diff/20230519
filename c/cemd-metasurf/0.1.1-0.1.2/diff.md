# Comparing `tmp/cemd_metasurf-0.1.1.tar.gz` & `tmp/cemd_metasurf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cemd_metasurf-0.1.1.tar", last modified: Fri May 19 13:05:13 2023, max compression
+gzip compressed data, was "cemd_metasurf-0.1.2.tar", last modified: Fri May 19 14:36:43 2023, max compression
```

## Comparing `cemd_metasurf-0.1.1.tar` & `cemd_metasurf-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,26 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-19 13:05:13.886746 cemd_metasurf-0.1.1/
--rw-rw-r--   0 diego     (1000) diego     (1000)     1078 2023-05-19 11:50:25.000000 cemd_metasurf-0.1.1/LICENSE
--rw-rw-r--   0 diego     (1000) diego     (1000)      859 2023-05-19 13:05:13.886746 cemd_metasurf-0.1.1/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      606 2023-05-19 09:37:13.000000 cemd_metasurf-0.1.1/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-19 13:05:13.886746 cemd_metasurf-0.1.1/cemd_metasurf/
--rw-rw-r--   0 diego     (1000) diego     (1000)       91 2023-05-19 12:10:17.000000 cemd_metasurf-0.1.1/cemd_metasurf/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)    10444 2023-05-19 09:12:07.000000 cemd_metasurf-0.1.1/cemd_metasurf/my_metasurface.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-19 13:05:13.886746 cemd_metasurf-0.1.1/cemd_metasurf.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)      859 2023-05-19 13:05:13.000000 cemd_metasurf-0.1.1/cemd_metasurf.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      268 2023-05-19 13:05:13.000000 cemd_metasurf-0.1.1/cemd_metasurf.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-05-19 13:05:13.000000 cemd_metasurf-0.1.1/cemd_metasurf.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        6 2023-05-19 13:05:13.000000 cemd_metasurf-0.1.1/cemd_metasurf.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       14 2023-05-19 13:05:13.000000 cemd_metasurf-0.1.1/cemd_metasurf.egg-info/top_level.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-05-19 13:05:13.886746 cemd_metasurf-0.1.1/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      698 2023-05-19 12:38:05.000000 cemd_metasurf-0.1.1/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-19 14:36:43.750178 cemd_metasurf-0.1.2/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1078 2023-05-19 11:50:25.000000 cemd_metasurf-0.1.2/LICENSE
+-rw-rw-r--   0 diego     (1000) diego     (1000)      859 2023-05-19 14:36:43.750178 cemd_metasurf-0.1.2/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      606 2023-05-19 09:37:13.000000 cemd_metasurf-0.1.2/README.md
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-19 14:36:43.750178 cemd_metasurf-0.1.2/cemd_metasurf/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       91 2023-05-19 12:10:17.000000 cemd_metasurf-0.1.2/cemd_metasurf/__init__.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-19 14:36:43.750178 cemd_metasurf-0.1.2/cemd_metasurf/depolarization_gf/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2023-05-09 14:21:26.000000 cemd_metasurf-0.1.2/cemd_metasurf/depolarization_gf/__init__.py
+-rwxr-xr-x   0 diego     (1000) diego     (1000)    10091 2023-05-18 18:33:08.000000 cemd_metasurf-0.1.2/cemd_metasurf/depolarization_gf/depolarization_functions.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2087 2023-05-18 18:33:20.000000 cemd_metasurf-0.1.2/cemd_metasurf/depolarization_gf/depolarization_gf.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)    10444 2023-05-19 09:12:07.000000 cemd_metasurf-0.1.2/cemd_metasurf/my_metasurface.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-19 14:36:43.750178 cemd_metasurf-0.1.2/cemd_metasurf/polarizability/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2023-05-09 14:21:26.000000 cemd_metasurf-0.1.2/cemd_metasurf/polarizability/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3978 2023-05-18 18:47:39.000000 cemd_metasurf-0.1.2/cemd_metasurf/polarizability/mie_functions.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-19 14:36:43.750178 cemd_metasurf-0.1.2/cemd_metasurf/reflec_transm/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2023-05-09 14:21:26.000000 cemd_metasurf-0.1.2/cemd_metasurf/reflec_transm/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3132 2023-05-19 07:42:42.000000 cemd_metasurf-0.1.2/cemd_metasurf/reflec_transm/reflec_transm.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)    11149 2023-05-18 18:44:26.000000 cemd_metasurf-0.1.2/cemd_metasurf/reflec_transm/rt_functions.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-19 14:36:43.750178 cemd_metasurf-0.1.2/cemd_metasurf.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)      859 2023-05-19 14:36:43.000000 cemd_metasurf-0.1.2/cemd_metasurf.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      641 2023-05-19 14:36:43.000000 cemd_metasurf-0.1.2/cemd_metasurf.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-05-19 14:36:43.000000 cemd_metasurf-0.1.2/cemd_metasurf.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        6 2023-05-19 14:36:43.000000 cemd_metasurf-0.1.2/cemd_metasurf.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       14 2023-05-19 14:36:43.000000 cemd_metasurf-0.1.2/cemd_metasurf.egg-info/top_level.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-05-19 14:36:43.750178 cemd_metasurf-0.1.2/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      793 2023-05-19 14:36:00.000000 cemd_metasurf-0.1.2/setup.py
```

### Comparing `cemd_metasurf-0.1.1/LICENSE` & `cemd_metasurf-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cemd_metasurf-0.1.1/PKG-INFO` & `cemd_metasurf-0.1.2/cemd_metasurf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cemd_metasurf
-Version: 0.1.1
+Name: cemd-metasurf
+Version: 0.1.2
 Summary: Optical properties of metasurfaces made of dipolar particles
 Author: Diego Romero Abujetas
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cemd_metasurf-0.1.1/README.md` & `cemd_metasurf-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cemd_metasurf-0.1.1/cemd_metasurf/my_metasurface.py` & `cemd_metasurf-0.1.2/cemd_metasurf/my_metasurface.py`

 * *Files identical despite different names*

### Comparing `cemd_metasurf-0.1.1/cemd_metasurf.egg-info/PKG-INFO` & `cemd_metasurf-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cemd-metasurf
-Version: 0.1.1
+Name: cemd_metasurf
+Version: 0.1.2
 Summary: Optical properties of metasurfaces made of dipolar particles
 Author: Diego Romero Abujetas
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cemd_metasurf-0.1.1/setup.py` & `cemd_metasurf-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cemd_metasurf',
-    packages=find_packages(include=['cemd_metasurf']),
-    version='0.1.1',
+    packages=find_packages(include=['cemd_metasurf','cemd_metasurf.depolarization_gf','cemd_metasurf.reflec_transm','cemd_metasurf.polarizability']),
+    version='0.1.2',
     description='Optical properties of metasurfaces made of dipolar particles',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Diego Romero Abujetas',
     license='MIT',
     install_requires=['numpy'],
     setup_requires=['pytest-runner'],
```

