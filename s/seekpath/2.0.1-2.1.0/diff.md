# Comparing `tmp/seekpath-2.0.1.tar.gz` & `tmp/seekpath-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seekpath-2.0.1.tar", last modified: Sun May 17 11:08:59 2020, max compression
+gzip compressed data, was "seekpath-2.1.0.tar", last modified: Fri May 19 17:43:56 2023, max compression
```

## Comparing `seekpath-2.0.1.tar` & `seekpath-2.1.0.tar`

### file list

```diff
@@ -1,202 +1,230 @@
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/
--rw-r--r--   0 pizzi      (501) staff       (20)     4876 2020-05-17 11:08:59.000000 seekpath-2.0.1/PKG-INFO
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath.egg-info/
--rw-r--r--   0 pizzi      (501) staff       (20)     4876 2020-05-17 11:08:58.000000 seekpath-2.0.1/seekpath.egg-info/PKG-INFO
--rw-r--r--   0 pizzi      (501) staff       (20)     7900 2020-05-17 11:08:58.000000 seekpath-2.0.1/seekpath.egg-info/SOURCES.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      125 2020-05-17 11:08:58.000000 seekpath-2.0.1/seekpath.egg-info/requires.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        9 2020-05-17 11:08:58.000000 seekpath-2.0.1/seekpath.egg-info/top_level.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        1 2020-05-17 11:08:58.000000 seekpath-2.0.1/seekpath.egg-info/dependency_links.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      135 2017-10-13 16:00:45.000000 seekpath-2.0.1/MANIFEST.in
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/
--rw-r--r--   0 pizzi      (501) staff       (20)    11464 2020-05-17 10:33:51.000000 seekpath-2.0.1/seekpath/hpkot/spg_mapping.py
--rw-r--r--   0 pizzi      (501) staff       (20)    13748 2020-05-17 10:33:51.000000 seekpath-2.0.1/seekpath/hpkot/tools.py
--rw-r--r--   0 pizzi      (501) staff       (20)    21351 2020-05-17 10:33:51.000000 seekpath-2.0.1/seekpath/hpkot/__init__.py
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hR1/
--rw-r--r--   0 pizzi      (501) staff       (20)      625 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hR1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       52 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hR1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       30 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hR1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      626 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hR1/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      264 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hR1/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oA2/
--rw-r--r--   0 pizzi      (501) staff       (20)      749 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oA2/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       72 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oA2/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       16 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oA2/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      198 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oA2/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tI1/
--rw-r--r--   0 pizzi      (501) staff       (20)     1003 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tI1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       50 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tI1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       16 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tI1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      874 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tI1/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)       83 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tI1/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/aP2/
--rw-r--r--   0 pizzi      (501) staff       (20)      507 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/aP2/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       56 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/aP2/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        0 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/aP2/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      508 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/aP2/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)       92 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/aP2/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cP1/
--rw-r--r--   0 pizzi      (501) staff       (20)      750 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cP1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       42 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cP1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        0 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cP1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      948 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cP1/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)       60 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cP1/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mP1/
--rw-r--r--   0 pizzi      (501) staff       (20)      934 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       64 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mP1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       56 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mP1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      563 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion_alternate
--rw-r--r--   0 pizzi      (501) staff       (20)      502 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mP1/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      228 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mP1/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/aP3/
--rw-r--r--   0 pizzi      (501) staff       (20)      507 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/aP3/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       64 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/aP3/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        0 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/aP3/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      625 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/aP3/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      118 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/aP3/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cF1/
--rw-r--r--   0 pizzi      (501) staff       (20)     5728 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cF1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       42 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cF1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        0 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cF1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)     5728 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cF1/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)       96 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cF1/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC3/
--rw-r--r--   0 pizzi      (501) staff       (20)      754 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC3/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       58 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC3/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      197 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC3/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      625 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC3/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      236 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC3/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hP2/
--rw-r--r--   0 pizzi      (501) staff       (20)      377 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hP2/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       48 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hP2/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        0 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hP2/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      440 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hP2/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)       87 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hP2/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF3/
--rw-r--r--   0 pizzi      (501) staff       (20)     1246 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF3/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       68 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF3/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       72 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF3/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)     2245 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF3/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      164 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF3/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oC1/
--rw-r--r--   0 pizzi      (501) staff       (20)      750 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oC1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       72 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oC1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       16 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oC1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      502 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oC1/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      126 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oC1/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC2/
--rw-r--r--   0 pizzi      (501) staff       (20)      625 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC2/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       44 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC2/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      123 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC2/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      701 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      197 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC2/points.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      997 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion_alternate
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF2/
--rw-r--r--   0 pizzi      (501) staff       (20)     1742 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF2/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       65 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF2/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       48 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF2/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      125 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF2/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI1/
--rw-r--r--   0 pizzi      (501) staff       (20)     1162 2019-07-29 19:20:57.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI1/POSCAR_inversion~
--rw-r--r--   0 pizzi      (501) staff       (20)      756 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       80 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       68 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      502 2019-07-29 19:43:13.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI1/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      172 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI1/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hR2/
--rw-r--r--   0 pizzi      (501) staff       (20)      817 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hR2/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       36 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hR2/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       34 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hR2/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)     1990 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      116 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hR2/points.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      997 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion_alternate
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tI2/
--rw-r--r--   0 pizzi      (501) staff       (20)      501 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tI2/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       54 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tI2/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       28 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tI2/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      501 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tI2/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      107 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tI2/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oA1/
--rw-r--r--   0 pizzi      (501) staff       (20)      625 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oA1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       72 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oA1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       16 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oA1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      126 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oA1/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cP2/
--rw-r--r--   0 pizzi      (501) staff       (20)      563 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cP2/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       36 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cP2/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        0 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cP2/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      378 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cP2/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)       60 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cP2/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oP1/
--rw-r--r--   0 pizzi      (501) staff       (20)      378 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oP1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       60 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oP1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        0 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oP1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      439 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oP1/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)       92 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oP1/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tP1/
--rw-r--r--   0 pizzi      (501) staff       (20)      439 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tP1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       48 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tP1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        0 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tP1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      378 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tP1/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)       70 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/tP1/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI3/
--rw-r--r--   0 pizzi      (501) staff       (20)      469 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI3/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       85 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI3/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       68 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI3/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      502 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI3/POSCAR_noinversion_alternate
--rw-r--r--   0 pizzi      (501) staff       (20)      998 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI3/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      177 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI3/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cI1/
--rw-r--r--   0 pizzi      (501) staff       (20)      873 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cI1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       36 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cI1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        0 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cI1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      749 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cI1/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)       51 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cI1/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cF2/
--rw-r--r--   0 pizzi      (501) staff       (20)      749 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cF2/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       36 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cF2/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        0 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cF2/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      749 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cF2/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)       96 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/cF2/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hP1/
--rw-r--r--   0 pizzi      (501) staff       (20)      571 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hP1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       54 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hP1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        0 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hP1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      687 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hP1/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)       87 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/hP1/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI2/
--rw-r--r--   0 pizzi      (501) staff       (20)     1500 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI2/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       81 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI2/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       68 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI2/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      171 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oI2/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF1/
--rw-r--r--   0 pizzi      (501) staff       (20)      748 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       64 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       48 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      997 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF1/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      124 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oF1/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oC2/
--rw-r--r--   0 pizzi      (501) staff       (20)     1250 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oC2/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       72 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oC2/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       16 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oC2/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      749 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oC2/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      198 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/oC2/points.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC1/
--rw-r--r--   0 pizzi      (501) staff       (20)      701 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion
--rw-r--r--   0 pizzi      (501) staff       (20)       76 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC1/path.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      114 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC1/k_vector_parameters.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      626 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion_alternate
--rw-r--r--   0 pizzi      (501) staff       (20)      701 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion
--rw-r--r--   0 pizzi      (501) staff       (20)      211 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC1/points.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      626 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion_alternate
--rw-r--r--   0 pizzi      (501) staff       (20)     9896 2020-05-17 10:33:51.000000 seekpath-2.0.1/seekpath/hpkot/spg_db.py
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-05-17 11:08:59.000000 seekpath-2.0.1/seekpath/brillouinzone/
--rw-r--r--   0 pizzi      (501) staff       (20)        0 2017-10-13 16:00:45.000000 seekpath-2.0.1/seekpath/brillouinzone/__init__.py
--rw-r--r--   0 pizzi      (501) staff       (20)    12008 2020-05-17 10:33:51.000000 seekpath-2.0.1/seekpath/brillouinzone/brillouinzone.py
--rw-r--r--   0 pizzi      (501) staff       (20)     1645 2020-05-17 10:33:51.000000 seekpath-2.0.1/seekpath/util.py
--rw-r--r--   0 pizzi      (501) staff       (20)    14253 2020-05-17 10:33:51.000000 seekpath-2.0.1/seekpath/getpaths.py
--rw-r--r--   0 pizzi      (501) staff       (20)      885 2020-05-17 11:07:47.000000 seekpath-2.0.1/seekpath/__init__.py
--rw-r--r--   0 pizzi      (501) staff       (20)     2749 2020-05-17 10:33:51.000000 seekpath-2.0.1/setup.py
--rw-r--r--   0 pizzi      (501) staff       (20)       38 2020-05-17 11:08:59.000000 seekpath-2.0.1/setup.cfg
--rw-r--r--   0 pizzi      (501) staff       (20)     3154 2020-05-17 10:33:51.000000 seekpath-2.0.1/README.rst
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.126080 seekpath-2.1.0/
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.065631 seekpath-2.1.0/.github/
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.075432 seekpath-2.1.0/.github/workflows/
+-rw-r--r--   0 pizzi      (501) staff       (20)      915 2023-05-19 17:20:13.000000 seekpath-2.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 pizzi      (501) staff       (20)       77 2023-05-19 12:55:39.000000 seekpath-2.1.0/.gitignore
+-rw-r--r--   0 pizzi      (501) staff       (20)      418 2023-05-19 17:20:13.000000 seekpath-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 pizzi      (501) staff       (20)       21 2023-05-19 12:55:39.000000 seekpath-2.1.0/.prospector.yaml
+-rw-r--r--   0 pizzi      (501) staff       (20)      529 2023-05-19 12:55:39.000000 seekpath-2.1.0/.pylintrc
+-rw-r--r--   0 pizzi      (501) staff       (20)      316 2023-05-19 17:20:13.000000 seekpath-2.1.0/.readthedocs.yml
+-rw-r--r--   0 pizzi      (501) staff       (20)       32 2020-08-18 20:07:54.000000 seekpath-2.1.0/.style.yapf
+-rw-r--r--   0 pizzi      (501) staff       (20)      548 2023-05-19 12:55:39.000000 seekpath-2.1.0/CHANGELOG.md
+-rw-r--r--   0 pizzi      (501) staff       (20)     1474 2023-05-19 17:33:03.000000 seekpath-2.1.0/LICENSE.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      135 2020-08-18 20:07:54.000000 seekpath-2.1.0/MANIFEST.in
+-rw-r--r--   0 pizzi      (501) staff       (20)     4977 2023-05-19 17:43:56.125832 seekpath-2.1.0/PKG-INFO
+-rw-r--r--   0 pizzi      (501) staff       (20)     3223 2023-05-19 17:41:54.000000 seekpath-2.1.0/README.rst
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.076267 seekpath-2.1.0/docs/
+-rw-r--r--   0 pizzi      (501) staff       (20)        6 2020-08-18 20:07:54.000000 seekpath-2.1.0/docs/.gitignore
+-rwxrwx---   0 pizzi      (501) staff       (20)     1433 2020-05-17 11:07:47.000000 seekpath-2.1.0/docs/Makefile
+-rw-r--r--   0 pizzi      (501) staff       (20)       14 2020-08-18 20:07:54.000000 seekpath-2.1.0/docs/requirements_for_rtd.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.077131 seekpath-2.1.0/docs/source/
+-rwxr-xr-x   0 pizzi      (501) staff       (20)    11575 2023-05-19 17:34:15.000000 seekpath-2.1.0/docs/source/conf.py
+-rwxrwx---   0 pizzi      (501) staff       (20)      338 2020-05-17 11:07:47.000000 seekpath-2.1.0/docs/source/index.rst
+-rw-r--r--   0 pizzi      (501) staff       (20)     6971 2023-05-19 17:32:21.000000 seekpath-2.1.0/docs/source/maindoc.rst
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.077412 seekpath-2.1.0/docs/source/module_guide/
+-rw-r--r--   0 pizzi      (501) staff       (20)      318 2023-05-19 17:32:21.000000 seekpath-2.1.0/docs/source/module_guide/index.rst
+-rw-r--r--   0 pizzi      (501) staff       (20)       65 2023-05-19 12:55:39.000000 seekpath-2.1.0/optional-requirements.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       29 2023-05-19 17:32:21.000000 seekpath-2.1.0/requirements.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.078323 seekpath-2.1.0/seekpath/
+-rw-r--r--   0 pizzi      (501) staff       (20)     1504 2023-05-19 17:34:53.000000 seekpath-2.1.0/seekpath/__init__.py
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.080235 seekpath-2.1.0/seekpath/brillouinzone/
+-rw-r--r--   0 pizzi      (501) staff       (20)        0 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/brillouinzone/__init__.py
+-rw-r--r--   0 pizzi      (501) staff       (20)    12006 2023-05-19 17:20:13.000000 seekpath-2.1.0/seekpath/brillouinzone/brillouinzone.py
+-rw-r--r--   0 pizzi      (501) staff       (20)    26349 2023-05-19 17:32:21.000000 seekpath-2.1.0/seekpath/getpaths.py
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.081432 seekpath-2.1.0/seekpath/hpkot/
+-rw-r--r--   0 pizzi      (501) staff       (20)    21490 2023-05-19 17:35:04.000000 seekpath-2.1.0/seekpath/hpkot/__init__.py
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.071319 seekpath-2.1.0/seekpath/hpkot/band_path_data/
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.082841 seekpath-2.1.0/seekpath/hpkot/band_path_data/aP2/
+-rw-r--r--   0 pizzi      (501) staff       (20)      508 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/aP2/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      507 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/aP2/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)        0 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/aP2/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       56 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/aP2/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       92 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/aP2/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.084230 seekpath-2.1.0/seekpath/hpkot/band_path_data/aP3/
+-rw-r--r--   0 pizzi      (501) staff       (20)      625 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/aP3/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      507 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/aP3/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)        0 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/aP3/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       64 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/aP3/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      118 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/aP3/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.087160 seekpath-2.1.0/seekpath/hpkot/band_path_data/cF1/
+-rw-r--r--   0 pizzi      (501) staff       (20)     5728 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cF1/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)     5728 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cF1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)        0 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cF1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       42 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cF1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       96 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cF1/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.088692 seekpath-2.1.0/seekpath/hpkot/band_path_data/cF2/
+-rw-r--r--   0 pizzi      (501) staff       (20)      749 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cF2/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      749 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cF2/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)        0 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cF2/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       36 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cF2/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       96 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cF2/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.090199 seekpath-2.1.0/seekpath/hpkot/band_path_data/cI1/
+-rw-r--r--   0 pizzi      (501) staff       (20)      749 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cI1/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      873 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cI1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)        0 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cI1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       36 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cI1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       51 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cI1/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.091596 seekpath-2.1.0/seekpath/hpkot/band_path_data/cP1/
+-rw-r--r--   0 pizzi      (501) staff       (20)      948 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cP1/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      750 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cP1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)        0 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cP1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       42 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cP1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       60 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cP1/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.092975 seekpath-2.1.0/seekpath/hpkot/band_path_data/cP2/
+-rw-r--r--   0 pizzi      (501) staff       (20)      378 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cP2/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      563 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cP2/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)        0 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cP2/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       36 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cP2/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       60 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/cP2/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.094362 seekpath-2.1.0/seekpath/hpkot/band_path_data/hP1/
+-rw-r--r--   0 pizzi      (501) staff       (20)      687 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hP1/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      571 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hP1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)        0 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hP1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       54 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hP1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       87 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hP1/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.095769 seekpath-2.1.0/seekpath/hpkot/band_path_data/hP2/
+-rw-r--r--   0 pizzi      (501) staff       (20)      440 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hP2/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      377 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hP2/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)        0 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hP2/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       48 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hP2/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       87 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hP2/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.097207 seekpath-2.1.0/seekpath/hpkot/band_path_data/hR1/
+-rw-r--r--   0 pizzi      (501) staff       (20)      626 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hR1/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      625 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hR1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)       30 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hR1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       52 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hR1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      264 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hR1/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.099223 seekpath-2.1.0/seekpath/hpkot/band_path_data/hR2/
+-rw-r--r--   0 pizzi      (501) staff       (20)     1990 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      997 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion_alternate
+-rw-r--r--   0 pizzi      (501) staff       (20)      817 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hR2/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)       34 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hR2/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       36 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hR2/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      116 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/hR2/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.101527 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC1/
+-rw-r--r--   0 pizzi      (501) staff       (20)      701 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      626 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion_alternate
+-rw-r--r--   0 pizzi      (501) staff       (20)      701 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      626 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion_alternate
+-rw-r--r--   0 pizzi      (501) staff       (20)      114 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       76 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      211 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC1/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.103648 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC2/
+-rw-r--r--   0 pizzi      (501) staff       (20)      701 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      997 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion_alternate
+-rw-r--r--   0 pizzi      (501) staff       (20)      625 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC2/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      123 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC2/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       44 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC2/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      197 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC2/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.105066 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC3/
+-rw-r--r--   0 pizzi      (501) staff       (20)      625 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC3/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      754 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC3/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      197 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC3/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       58 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC3/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      236 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mC3/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.106557 seekpath-2.1.0/seekpath/hpkot/band_path_data/mP1/
+-rw-r--r--   0 pizzi      (501) staff       (20)      502 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mP1/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      934 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      563 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion_alternate
+-rw-r--r--   0 pizzi      (501) staff       (20)       56 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mP1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       64 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mP1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      228 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/mP1/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.107549 seekpath-2.1.0/seekpath/hpkot/band_path_data/oA1/
+-rw-r--r--   0 pizzi      (501) staff       (20)      625 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oA1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)       16 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oA1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       72 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oA1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      126 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oA1/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.108526 seekpath-2.1.0/seekpath/hpkot/band_path_data/oA2/
+-rw-r--r--   0 pizzi      (501) staff       (20)      749 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oA2/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)       16 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oA2/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       72 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oA2/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      198 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oA2/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.109780 seekpath-2.1.0/seekpath/hpkot/band_path_data/oC1/
+-rw-r--r--   0 pizzi      (501) staff       (20)      502 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oC1/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      750 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oC1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)       16 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oC1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       72 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oC1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      126 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oC1/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.111003 seekpath-2.1.0/seekpath/hpkot/band_path_data/oC2/
+-rw-r--r--   0 pizzi      (501) staff       (20)      749 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oC2/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)     1250 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oC2/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)       16 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oC2/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       72 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oC2/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      198 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oC2/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.112239 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF1/
+-rw-r--r--   0 pizzi      (501) staff       (20)      997 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF1/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      748 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)       48 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       64 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      124 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF1/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.113237 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF2/
+-rw-r--r--   0 pizzi      (501) staff       (20)     1742 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF2/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)       48 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF2/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       65 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF2/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      125 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF2/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.114465 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF3/
+-rw-r--r--   0 pizzi      (501) staff       (20)     2245 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF3/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)     1246 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF3/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)       72 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF3/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       68 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF3/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      164 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oF3/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.116707 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI1/
+-rw-r--r--   0 pizzi      (501) staff       (20)      502 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI1/POSCAR_inversion
+-rwxrwx---   0 pizzi      (501) staff       (20)     1162 2019-07-29 19:20:57.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI1/POSCAR_inversion~
+-rw-r--r--   0 pizzi      (501) staff       (20)      756 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)       68 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       80 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      172 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI1/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.117788 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI2/
+-rw-r--r--   0 pizzi      (501) staff       (20)     1500 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI2/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)       68 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI2/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       81 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI2/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      171 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI2/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.119380 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI3/
+-rw-r--r--   0 pizzi      (501) staff       (20)      998 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI3/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      469 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI3/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      502 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI3/POSCAR_noinversion_alternate
+-rw-r--r--   0 pizzi      (501) staff       (20)       68 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI3/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       85 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI3/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      177 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oI3/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.120619 seekpath-2.1.0/seekpath/hpkot/band_path_data/oP1/
+-rw-r--r--   0 pizzi      (501) staff       (20)      439 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oP1/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      378 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oP1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)        0 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oP1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       60 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oP1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       92 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/oP1/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.121877 seekpath-2.1.0/seekpath/hpkot/band_path_data/tI1/
+-rw-r--r--   0 pizzi      (501) staff       (20)      874 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tI1/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)     1003 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tI1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)       16 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tI1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       50 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tI1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       83 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tI1/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.123181 seekpath-2.1.0/seekpath/hpkot/band_path_data/tI2/
+-rw-r--r--   0 pizzi      (501) staff       (20)      501 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tI2/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      501 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tI2/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)       28 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tI2/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       54 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tI2/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      107 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tI2/points.txt
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.124408 seekpath-2.1.0/seekpath/hpkot/band_path_data/tP1/
+-rw-r--r--   0 pizzi      (501) staff       (20)      378 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tP1/POSCAR_inversion
+-rw-r--r--   0 pizzi      (501) staff       (20)      439 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tP1/POSCAR_noinversion
+-rw-r--r--   0 pizzi      (501) staff       (20)        0 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tP1/k_vector_parameters.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       48 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tP1/path.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       70 2020-08-18 20:07:54.000000 seekpath-2.1.0/seekpath/hpkot/band_path_data/tP1/points.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)     9666 2023-05-19 17:20:13.000000 seekpath-2.1.0/seekpath/hpkot/spg_db.py
+-rw-r--r--   0 pizzi      (501) staff       (20)    11432 2023-05-19 17:20:13.000000 seekpath-2.1.0/seekpath/hpkot/spg_mapping.py
+-rw-r--r--   0 pizzi      (501) staff       (20)    13740 2023-05-19 17:20:13.000000 seekpath-2.1.0/seekpath/hpkot/tools.py
+-rw-r--r--   0 pizzi      (501) staff       (20)     1645 2023-05-19 12:55:39.000000 seekpath-2.1.0/seekpath/util.py
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.079727 seekpath-2.1.0/seekpath.egg-info/
+-rw-r--r--   0 pizzi      (501) staff       (20)     4977 2023-05-19 17:43:55.000000 seekpath-2.1.0/seekpath.egg-info/PKG-INFO
+-rw-r--r--   0 pizzi      (501) staff       (20)     8351 2023-05-19 17:43:55.000000 seekpath-2.1.0/seekpath.egg-info/SOURCES.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)        1 2023-05-19 17:43:55.000000 seekpath-2.1.0/seekpath.egg-info/dependency_links.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)      126 2023-05-19 17:43:55.000000 seekpath-2.1.0/seekpath.egg-info/requires.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)        9 2023-05-19 17:43:55.000000 seekpath-2.1.0/seekpath.egg-info/top_level.txt
+-rw-r--r--   0 pizzi      (501) staff       (20)       38 2023-05-19 17:43:56.126164 seekpath-2.1.0/setup.cfg
+-rw-r--r--   0 pizzi      (501) staff       (20)     2750 2023-05-19 17:20:13.000000 seekpath-2.1.0/setup.py
+drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2023-05-19 17:43:56.125378 seekpath-2.1.0/tests/
+-rw-r--r--   0 pizzi      (501) staff       (20)        0 2023-05-19 12:55:39.000000 seekpath-2.1.0/tests/conftest.py
+-rw-r--r--   0 pizzi      (501) staff       (20)     8496 2023-05-19 17:20:13.000000 seekpath-2.1.0/tests/test_brillouinzone.py
+-rw-r--r--   0 pizzi      (501) staff       (20)     3280 2023-05-19 12:55:39.000000 seekpath-2.1.0/tests/test_hpkot_get_primitive.py
+-rw-r--r--   0 pizzi      (501) staff       (20)    41021 2023-05-19 17:32:21.000000 seekpath-2.1.0/tests/test_paths_hpkot.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `seekpath-2.0.1/PKG-INFO` & `seekpath-2.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: seekpath
-Version: 2.0.1
+Version: 2.1.0
 Summary: A module to obtain and visualize k-vector coefficients and obtain band paths in the Brillouin zone of crystal structures
 Home-page: http://github.com/giovannipizzi/seekpath
 Author: Giovanni Pizzi
 License: The MIT license
-Download-URL: https://github.com/giovannipizzi/seekpath/archive/v2.0.1.tar.gz
+Download-URL: https://github.com/giovannipizzi/seekpath/archive/v2.1.0.tar.gz
 Description: #########
         SeeK-path
         #########
         
-        Test status: branch `master`: |travismaster|; branch `develop`: |travisdevelop|
+        Test status for default branch: |continuousintegration|
         
-        .. |travismaster| image:: https://travis-ci.org/giovannipizzi/seekpath.svg?branch=master
-            :target: https://travis-ci.org/giovannipizzi/seekpath
-        
-        .. |travisdevelop| image:: https://travis-ci.org/giovannipizzi/seekpath.svg?branch=develop
-            :target: https://travis-ci.org/giovannipizzi/seekpath
+        .. |continuousintegration| image:: https://github.com/giovannipizzi/seekpath/actions/workflows/ci.yml/badge.svg
+            :target: https://github.com/giovannipizzi/seekpath/actions/workflows/ci.yml
         
         ``SeeK-path`` is a python module to obtain band paths in the
         Brillouin zone of crystal structures.
         
         The definition of k-point labels follows crystallographic convention, as defined
         and discussed in the `HPKOT paper`_. Moreover, the Bravais lattice is detected
         properly using the spacegroup symmetry. Also the suggested band path provided
@@ -46,14 +43,20 @@
         
         =============================
         How to install and how to use
         =============================
         
         Please check the SeeK-path `user guide on ReadTheDocs`_.
         
+        ================
+        Acknowledgements
+        ================
+        
+        * Jae-Mo Lihm: k-point paths for the original unit cell (i.e., the one provided in input by the user) without standardization or symmetrization
+        
         =======
         License
         =======
         
         The code is open-source (licensed with a MIT license, see LICENSE.txt).
         
         ===================
@@ -83,14 +86,15 @@
         .. _arXiv link: https://arxiv.org/abs/1602.06402
         .. _spglib: http://atztogo.github.io/spglib/
         .. _Materials Cloud: http://www.materialscloud.org/tools/seekpath/
         .. _docker hub: https://hub.docker.com/r/giovannipizzi/seekpath/
         .. _user guide on ReadTheDocs: http://seekpath.readthedocs.io
         .. _spglib arXiv link: https://arxiv.org/abs/1808.01590
         .. _tools-seekpath: http://www.github.com/materialscloud-org/tools-seekpath/
+        
 Keywords: path,band structure,Brillouin,crystallography,physics,primitive cell,conventional cell
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `seekpath-2.0.1/seekpath.egg-info/PKG-INFO` & `seekpath-2.1.0/seekpath.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: seekpath
-Version: 2.0.1
+Version: 2.1.0
 Summary: A module to obtain and visualize k-vector coefficients and obtain band paths in the Brillouin zone of crystal structures
 Home-page: http://github.com/giovannipizzi/seekpath
 Author: Giovanni Pizzi
 License: The MIT license
-Download-URL: https://github.com/giovannipizzi/seekpath/archive/v2.0.1.tar.gz
+Download-URL: https://github.com/giovannipizzi/seekpath/archive/v2.1.0.tar.gz
 Description: #########
         SeeK-path
         #########
         
-        Test status: branch `master`: |travismaster|; branch `develop`: |travisdevelop|
+        Test status for default branch: |continuousintegration|
         
-        .. |travismaster| image:: https://travis-ci.org/giovannipizzi/seekpath.svg?branch=master
-            :target: https://travis-ci.org/giovannipizzi/seekpath
-        
-        .. |travisdevelop| image:: https://travis-ci.org/giovannipizzi/seekpath.svg?branch=develop
-            :target: https://travis-ci.org/giovannipizzi/seekpath
+        .. |continuousintegration| image:: https://github.com/giovannipizzi/seekpath/actions/workflows/ci.yml/badge.svg
+            :target: https://github.com/giovannipizzi/seekpath/actions/workflows/ci.yml
         
         ``SeeK-path`` is a python module to obtain band paths in the
         Brillouin zone of crystal structures.
         
         The definition of k-point labels follows crystallographic convention, as defined
         and discussed in the `HPKOT paper`_. Moreover, the Bravais lattice is detected
         properly using the spacegroup symmetry. Also the suggested band path provided
@@ -46,14 +43,20 @@
         
         =============================
         How to install and how to use
         =============================
         
         Please check the SeeK-path `user guide on ReadTheDocs`_.
         
+        ================
+        Acknowledgements
+        ================
+        
+        * Jae-Mo Lihm: k-point paths for the original unit cell (i.e., the one provided in input by the user) without standardization or symmetrization
+        
         =======
         License
         =======
         
         The code is open-source (licensed with a MIT license, see LICENSE.txt).
         
         ===================
@@ -83,14 +86,15 @@
         .. _arXiv link: https://arxiv.org/abs/1602.06402
         .. _spglib: http://atztogo.github.io/spglib/
         .. _Materials Cloud: http://www.materialscloud.org/tools/seekpath/
         .. _docker hub: https://hub.docker.com/r/giovannipizzi/seekpath/
         .. _user guide on ReadTheDocs: http://seekpath.readthedocs.io
         .. _spglib arXiv link: https://arxiv.org/abs/1808.01590
         .. _tools-seekpath: http://www.github.com/materialscloud-org/tools-seekpath/
+        
 Keywords: path,band structure,Brillouin,crystallography,physics,primitive cell,conventional cell
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `seekpath-2.0.1/seekpath.egg-info/SOURCES.txt` & `seekpath-2.1.0/seekpath.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,28 @@
+.gitignore
+.pre-commit-config.yaml
+.prospector.yaml
+.pylintrc
+.readthedocs.yml
+.style.yapf
+CHANGELOG.md
+LICENSE.txt
 MANIFEST.in
 README.rst
+optional-requirements.txt
+requirements.txt
 setup.py
+.github/workflows/ci.yml
+docs/.gitignore
+docs/Makefile
+docs/requirements_for_rtd.txt
+docs/source/conf.py
+docs/source/index.rst
+docs/source/maindoc.rst
+docs/source/module_guide/index.rst
 seekpath/__init__.py
 seekpath/getpaths.py
 seekpath/util.py
 seekpath.egg-info/PKG-INFO
 seekpath.egg-info/SOURCES.txt
 seekpath.egg-info/dependency_links.txt
 seekpath.egg-info/requires.txt
@@ -158,8 +176,12 @@
 seekpath/hpkot/band_path_data/tI2/k_vector_parameters.txt
 seekpath/hpkot/band_path_data/tI2/path.txt
 seekpath/hpkot/band_path_data/tI2/points.txt
 seekpath/hpkot/band_path_data/tP1/POSCAR_inversion
 seekpath/hpkot/band_path_data/tP1/POSCAR_noinversion
 seekpath/hpkot/band_path_data/tP1/k_vector_parameters.txt
 seekpath/hpkot/band_path_data/tP1/path.txt
-seekpath/hpkot/band_path_data/tP1/points.txt
+seekpath/hpkot/band_path_data/tP1/points.txt
+tests/conftest.py
+tests/test_brillouinzone.py
+tests/test_hpkot_get_primitive.py
+tests/test_paths_hpkot.py
```

### Comparing `seekpath-2.0.1/seekpath/hpkot/spg_mapping.py` & `seekpath-2.1.0/seekpath/hpkot/spg_mapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,46 +65,46 @@
 
 def pgnum_from_pgint(pgint):
     """
     Return the number of the pointgroup (from 1 to 32) from the
     international pointgroup name.
     """
     table = {
-        u"C1": 1,
-        u"C2": 3,
-        u"C2h": 5,
-        u"C2v": 7,
-        u"C3": 16,
-        u"C3h": 22,
-        u"C3i": 17,
-        u"C3v": 19,
-        u"C4": 9,
-        u"C4h": 11,
-        u"C4v": 13,
-        u"C6": 21,
-        u"C6h": 23,
-        u"C6v": 25,
-        u"Ci": 2,
-        u"Cs": 4,
-        u"D2": 6,
-        u"D2d": 14,
-        u"D2h": 8,
-        u"D3": 18,
-        u"D3d": 20,
-        u"D3h": 26,
-        u"D4": 12,
-        u"D4h": 15,
-        u"D6": 24,
-        u"D6h": 27,
-        u"O": 30,
-        u"Oh": 32,
-        u"S4": 10,
-        u"T": 28,
-        u"Td": 31,
-        u"Th": 29,
+        "C1": 1,
+        "C2": 3,
+        "C2h": 5,
+        "C2v": 7,
+        "C3": 16,
+        "C3h": 22,
+        "C3i": 17,
+        "C3v": 19,
+        "C4": 9,
+        "C4h": 11,
+        "C4v": 13,
+        "C6": 21,
+        "C6h": 23,
+        "C6v": 25,
+        "Ci": 2,
+        "Cs": 4,
+        "D2": 6,
+        "D2d": 14,
+        "D2h": 8,
+        "D3": 18,
+        "D3d": 20,
+        "D3h": 26,
+        "D4": 12,
+        "D4h": 15,
+        "D6": 24,
+        "D6h": 27,
+        "O": 30,
+        "Oh": 32,
+        "S4": 10,
+        "T": 28,
+        "Td": 31,
+        "Th": 29,
     }
 
     return table[pgint]
 
 
 def get_spgroup_data():
     """
```

### Comparing `seekpath-2.0.1/seekpath/hpkot/tools.py` & `seekpath-2.1.0/seekpath/hpkot/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     .. note::  To evaluate expressions, I hardcode a table of existing expressions in the
         DB rather than parsing the string (to avoid additional dependencies and
         avoid the use of ``eval``).
     """
     from math import sqrt
 
     # sinalpha = sqrt(1.0 - cosalpha ** 2)
-    sinbeta = sqrt(1.0 - cosbeta ** 2)
+    sinbeta = sqrt(1.0 - cosbeta**2)
     # singamma = sqrt(1.0 - cosgamma ** 2)
 
     try:
         if expr == "(a*a/b/b+(1+a/c*cosbeta)/sinbeta/sinbeta)/4":
             return (a * a / b / b + (1.0 + a / c * cosbeta) / sinbeta / sinbeta) / 4.0
         if expr == "1-Z*b*b/a/a":
             Z = kparam["Z"]
@@ -255,17 +255,17 @@
 def get_cell_params(cell):
     r"""
     Return (a,b,c,cosalpha,cosbeta,cosgamma) given a :math:`3\times 3` cell
 
     .. note:: Rows are vectors: ``v1 = cell[0]``, ``v2 = cell[1]``, ``v3 = cell[3]``
     """
     v1, v2, v3 = numpy.array(cell)
-    a = sqrt(sum(v1 ** 2))
-    b = sqrt(sum(v2 ** 2))
-    c = sqrt(sum(v3 ** 2))
+    a = sqrt(sum(v1**2))
+    b = sqrt(sum(v2**2))
+    c = sqrt(sum(v3**2))
     cosalpha = numpy.dot(v2, v3) / b / c
     cosbeta = numpy.dot(v1, v3) / a / c
     cosgamma = numpy.dot(v1, v2) / a / b
 
     return (a, b, c, cosalpha, cosbeta, cosgamma)
```

### Comparing `seekpath-2.0.1/seekpath/hpkot/__init__.py` & `seekpath-2.1.0/seekpath/hpkot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 The seekpath.hpkot module contains routines to get automatically the
 path in a 3D Brillouin zone to plot band structures according to the
 HPKOT paper (see references below).
 
-Author: Giovanni Pizzi, EPFL
+Author: Giovanni Pizzi, PSI
 
 Licence: MIT License, see LICENSE.txt
 
 .. note:: the list of point coordinates and example POSCAR files in
   the band_path_data subfolder have been provided by Yoyo Hinuma,
   Kyoto University, Japan. The POSCARs have been retrieved from
   the Materials Project (http://materialsproject.org).
@@ -116,14 +116,16 @@
           primitive cell (vectors are rows: ``reciprocal_primitive_lattice[0,:]``
           is the first vector)
         - ``primitive_transformation_matrix``: the transformation matrix :math:`P` between
           the conventional and the primitive cell
         - ``inverse_primitive_transformation_matrix``: the inverse of the matrix :math:`P`
           (the determinant is integer and gives the ratio in volume between
           the conventional and primitive cells)
+        - ``rotation_matrix``: rotation matrix in Cartesian space from the input
+          cell to the standardized cell
         - ``volume_original_wrt_conv``: volume ratio of the user-provided cell
           with respect to the the crystallographic conventional cell
         - ``volume_original_wrt_prim``: volume ratio of the user-provided cell
           with respect to the the crystallographic primitive cell
 
     :note: An :py:exc:`~seekpath.hpkot.EdgeCaseWarning` is issued for
         edge cases (e.g. if ``a==b==c`` for
@@ -214,25 +216,25 @@
         if c <= a:
             ext_bravais = "tI1"
         else:
             ext_bravais = "tI2"
     elif bravais_lattice == "oP":
         ext_bravais = "oP1"
     elif bravais_lattice == "oF":
-        if abs(1.0 / (a ** 2) - (1.0 / (b ** 2) + 1.0 / (c ** 2))) < threshold:
+        if abs(1.0 / (a**2) - (1.0 / (b**2) + 1.0 / (c**2))) < threshold:
             warnings.warn(
                 "oF lattice, but 1/a^2 almost equal to 1/b^2 + 1/c^2", EdgeCaseWarning
             )
-        if abs(1.0 / (c ** 2) - (1.0 / (a ** 2) + 1.0 / (b ** 2))) < threshold:
+        if abs(1.0 / (c**2) - (1.0 / (a**2) + 1.0 / (b**2))) < threshold:
             warnings.warn(
                 "oF lattice, but 1/c^2 almost equal to 1/a^2 + 1/b^2", EdgeCaseWarning
             )
-        if 1.0 / (a ** 2) > 1.0 / (b ** 2) + 1.0 / (c ** 2):
+        if 1.0 / (a**2) > 1.0 / (b**2) + 1.0 / (c**2):
             ext_bravais = "oF1"
-        elif 1.0 / (c ** 2) > 1.0 / (a ** 2) + 1.0 / (b ** 2):
+        elif 1.0 / (c**2) > 1.0 / (a**2) + 1.0 / (b**2):
             ext_bravais = "oF2"
         else:  # 1/a^2, 1/b^2, 1/c^2 edges of a triangle
             ext_bravais = "oF3"
     elif bravais_lattice == "oI":
         # Sort a,b,c, first is the largest
         sorted_vectors = sorted([(c, 1, "c"), (b, 3, "b"), (a, 2, "a")])[::-1]
         if abs(sorted_vectors[0][0] - sorted_vectors[1][0]) < threshold:
@@ -287,31 +289,31 @@
         if sqrt(3.0) * a <= sqrt(2.0) * c:
             ext_bravais = "hR1"
         else:
             ext_bravais = "hR2"
     elif bravais_lattice == "mP":
         ext_bravais = "mP1"
     elif bravais_lattice == "mC":
-        if abs(b - a * sqrt(1.0 - cosbeta ** 2)) < threshold:
+        if abs(b - a * sqrt(1.0 - cosbeta**2)) < threshold:
             warnings.warn(
                 "mC lattice, but b almost equal to a*sin(beta)", EdgeCaseWarning
             )
-        if b < a * sqrt(1.0 - cosbeta ** 2):
+        if b < a * sqrt(1.0 - cosbeta**2):
             ext_bravais = "mC1"
         else:
             if (
-                abs(-a * cosbeta / c + a ** 2 * (1.0 - cosbeta ** 2) / b ** 2 - 1.0)
+                abs(-a * cosbeta / c + a**2 * (1.0 - cosbeta**2) / b**2 - 1.0)
                 < threshold
             ):
                 warnings.warn(
                     "mC lattice, but -a*cos(beta)/c + "
                     "a^2*sin(beta)^2/b^2 almost equal to 1",
                     EdgeCaseWarning,
                 )
-            if -a * cosbeta / c + a ** 2 * (1.0 - cosbeta ** 2) / b ** 2 <= 1.0:
+            if -a * cosbeta / c + a**2 * (1.0 - cosbeta**2) / b**2 <= 1.0:
                 # 12-face
                 ext_bravais = "mC2"
             else:
                 ext_bravais = "mC3"
     elif bravais_lattice == "aP":
         # First step: cell that is Niggli reduced in reciprocal space
         # I use the default eps here, this could be changed
@@ -511,8 +513,9 @@
         # For the time being disabled, not valid for aP lattices
         # (for which we would need the transformation matrix from niggli)
         #'transformation_matrix': transf_matrix,
         "volume_original_wrt_conv": volume_conv_wrt_original,
         "volume_original_wrt_prim": volume_conv_wrt_original * np.linalg.det(invP),
         "spacegroup_number": dataset["number"],
         "spacegroup_international": dataset["international"],
+        "rotation_matrix": dataset["std_rotation_matrix"],
     }
```

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/hR1/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/hR1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/hR1/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/hR1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oA2/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oA2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/tI1/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/tI1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/tI1/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/tI1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/cP1/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/cP1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/cP1/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/cP1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion_alternate` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/mP1/POSCAR_noinversion_alternate`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/aP3/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/aP3/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/cF1/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/cF1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/cF1/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/cF1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/mC3/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/mC3/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/mC3/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/mC3/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oF3/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oF3/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oF3/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oF3/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oC1/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oC1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/mC2/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/mC2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion_alternate` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/mC2/POSCAR_inversion_alternate`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oF2/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oF2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oI1/POSCAR_inversion~` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oI1/POSCAR_inversion~`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oI1/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oI1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/hR2/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/hR2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion_alternate` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/hR2/POSCAR_inversion_alternate`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oA1/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oA1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/cP2/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/cP2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oI3/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oI3/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/cI1/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/cI1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/cI1/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/cI1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/cF2/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/cF2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/cF2/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/cF2/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/hP1/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/hP1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/hP1/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/hP1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oI2/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oI2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oF1/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oF1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oF1/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oF1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oC2/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oC2/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/oC2/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/oC2/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion_alternate` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/mC1/POSCAR_noinversion_alternate`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion_alternate` & `seekpath-2.1.0/seekpath/hpkot/band_path_data/mC1/POSCAR_inversion_alternate`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/hpkot/spg_db.py` & `seekpath-2.1.0/seekpath/hpkot/spg_db.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,244 +2,244 @@
 # Given a spgroup number, return
 # the crystal family letter, the centering, and if the corresponding
 # pointgroup has inversion (True) or not.
 # Generated from the output of spg_mapping.get_spgroup_data_realtime
 # using spglib v.1.9.4.
 
 spgroup_data = {
-    1: ("a", u"P", False),
-    2: ("a", u"P", True),
-    3: ("m", u"P", False),
-    4: ("m", u"P", False),
-    5: ("m", u"C", False),
-    6: ("m", u"P", False),
-    7: ("m", u"P", False),
-    8: ("m", u"C", False),
-    9: ("m", u"C", False),
-    10: ("m", u"P", True),
-    11: ("m", u"P", True),
-    12: ("m", u"C", True),
-    13: ("m", u"P", True),
-    14: ("m", u"P", True),
-    15: ("m", u"C", True),
-    16: ("o", u"P", False),
-    17: ("o", u"P", False),
-    18: ("o", u"P", False),
-    19: ("o", u"P", False),
-    20: ("o", u"C", False),
-    21: ("o", u"C", False),
-    22: ("o", u"F", False),
-    23: ("o", u"I", False),
-    24: ("o", u"I", False),
-    25: ("o", u"P", False),
-    26: ("o", u"P", False),
-    27: ("o", u"P", False),
-    28: ("o", u"P", False),
-    29: ("o", u"P", False),
-    30: ("o", u"P", False),
-    31: ("o", u"P", False),
-    32: ("o", u"P", False),
-    33: ("o", u"P", False),
-    34: ("o", u"P", False),
-    35: ("o", u"C", False),
-    36: ("o", u"C", False),
-    37: ("o", u"C", False),
-    38: ("o", u"A", False),
-    39: ("o", u"A", False),
-    40: ("o", u"A", False),
-    41: ("o", u"A", False),
-    42: ("o", u"F", False),
-    43: ("o", u"F", False),
-    44: ("o", u"I", False),
-    45: ("o", u"I", False),
-    46: ("o", u"I", False),
-    47: ("o", u"P", True),
-    48: ("o", u"P", True),
-    49: ("o", u"P", True),
-    50: ("o", u"P", True),
-    51: ("o", u"P", True),
-    52: ("o", u"P", True),
-    53: ("o", u"P", True),
-    54: ("o", u"P", True),
-    55: ("o", u"P", True),
-    56: ("o", u"P", True),
-    57: ("o", u"P", True),
-    58: ("o", u"P", True),
-    59: ("o", u"P", True),
-    60: ("o", u"P", True),
-    61: ("o", u"P", True),
-    62: ("o", u"P", True),
-    63: ("o", u"C", True),
-    64: ("o", u"C", True),
-    65: ("o", u"C", True),
-    66: ("o", u"C", True),
-    67: ("o", u"C", True),
-    68: ("o", u"C", True),
-    69: ("o", u"F", True),
-    70: ("o", u"F", True),
-    71: ("o", u"I", True),
-    72: ("o", u"I", True),
-    73: ("o", u"I", True),
-    74: ("o", u"I", True),
-    75: ("t", u"P", False),
-    76: ("t", u"P", False),
-    77: ("t", u"P", False),
-    78: ("t", u"P", False),
-    79: ("t", u"I", False),
-    80: ("t", u"I", False),
-    81: ("t", u"P", False),
-    82: ("t", u"I", False),
-    83: ("t", u"P", True),
-    84: ("t", u"P", True),
-    85: ("t", u"P", True),
-    86: ("t", u"P", True),
-    87: ("t", u"I", True),
-    88: ("t", u"I", True),
-    89: ("t", u"P", False),
-    90: ("t", u"P", False),
-    91: ("t", u"P", False),
-    92: ("t", u"P", False),
-    93: ("t", u"P", False),
-    94: ("t", u"P", False),
-    95: ("t", u"P", False),
-    96: ("t", u"P", False),
-    97: ("t", u"I", False),
-    98: ("t", u"I", False),
-    99: ("t", u"P", False),
-    100: ("t", u"P", False),
-    101: ("t", u"P", False),
-    102: ("t", u"P", False),
-    103: ("t", u"P", False),
-    104: ("t", u"P", False),
-    105: ("t", u"P", False),
-    106: ("t", u"P", False),
-    107: ("t", u"I", False),
-    108: ("t", u"I", False),
-    109: ("t", u"I", False),
-    110: ("t", u"I", False),
-    111: ("t", u"P", False),
-    112: ("t", u"P", False),
-    113: ("t", u"P", False),
-    114: ("t", u"P", False),
-    115: ("t", u"P", False),
-    116: ("t", u"P", False),
-    117: ("t", u"P", False),
-    118: ("t", u"P", False),
-    119: ("t", u"I", False),
-    120: ("t", u"I", False),
-    121: ("t", u"I", False),
-    122: ("t", u"I", False),
-    123: ("t", u"P", True),
-    124: ("t", u"P", True),
-    125: ("t", u"P", True),
-    126: ("t", u"P", True),
-    127: ("t", u"P", True),
-    128: ("t", u"P", True),
-    129: ("t", u"P", True),
-    130: ("t", u"P", True),
-    131: ("t", u"P", True),
-    132: ("t", u"P", True),
-    133: ("t", u"P", True),
-    134: ("t", u"P", True),
-    135: ("t", u"P", True),
-    136: ("t", u"P", True),
-    137: ("t", u"P", True),
-    138: ("t", u"P", True),
-    139: ("t", u"I", True),
-    140: ("t", u"I", True),
-    141: ("t", u"I", True),
-    142: ("t", u"I", True),
-    143: ("h", u"P", False),
-    144: ("h", u"P", False),
-    145: ("h", u"P", False),
-    146: ("h", u"R", False),
-    147: ("h", u"P", True),
-    148: ("h", u"R", True),
-    149: ("h", u"P", False),
-    150: ("h", u"P", False),
-    151: ("h", u"P", False),
-    152: ("h", u"P", False),
-    153: ("h", u"P", False),
-    154: ("h", u"P", False),
-    155: ("h", u"R", False),
-    156: ("h", u"P", False),
-    157: ("h", u"P", False),
-    158: ("h", u"P", False),
-    159: ("h", u"P", False),
-    160: ("h", u"R", False),
-    161: ("h", u"R", False),
-    162: ("h", u"P", True),
-    163: ("h", u"P", True),
-    164: ("h", u"P", True),
-    165: ("h", u"P", True),
-    166: ("h", u"R", True),
-    167: ("h", u"R", True),
-    168: ("h", u"P", False),
-    169: ("h", u"P", False),
-    170: ("h", u"P", False),
-    171: ("h", u"P", False),
-    172: ("h", u"P", False),
-    173: ("h", u"P", False),
-    174: ("h", u"P", False),
-    175: ("h", u"P", True),
-    176: ("h", u"P", True),
-    177: ("h", u"P", False),
-    178: ("h", u"P", False),
-    179: ("h", u"P", False),
-    180: ("h", u"P", False),
-    181: ("h", u"P", False),
-    182: ("h", u"P", False),
-    183: ("h", u"P", False),
-    184: ("h", u"P", False),
-    185: ("h", u"P", False),
-    186: ("h", u"P", False),
-    187: ("h", u"P", False),
-    188: ("h", u"P", False),
-    189: ("h", u"P", False),
-    190: ("h", u"P", False),
-    191: ("h", u"P", True),
-    192: ("h", u"P", True),
-    193: ("h", u"P", True),
-    194: ("h", u"P", True),
-    195: ("c", u"P", False),
-    196: ("c", u"F", False),
-    197: ("c", u"I", False),
-    198: ("c", u"P", False),
-    199: ("c", u"I", False),
-    200: ("c", u"P", True),
-    201: ("c", u"P", True),
-    202: ("c", u"F", True),
-    203: ("c", u"F", True),
-    204: ("c", u"I", True),
-    205: ("c", u"P", True),
-    206: ("c", u"I", True),
-    207: ("c", u"P", False),
-    208: ("c", u"P", False),
-    209: ("c", u"F", False),
-    210: ("c", u"F", False),
-    211: ("c", u"I", False),
-    212: ("c", u"P", False),
-    213: ("c", u"P", False),
-    214: ("c", u"I", False),
-    215: ("c", u"P", False),
-    216: ("c", u"F", False),
-    217: ("c", u"I", False),
-    218: ("c", u"P", False),
-    219: ("c", u"F", False),
-    220: ("c", u"I", False),
-    221: ("c", u"P", True),
-    222: ("c", u"P", True),
-    223: ("c", u"P", True),
-    224: ("c", u"P", True),
-    225: ("c", u"F", True),
-    226: ("c", u"F", True),
-    227: ("c", u"F", True),
-    228: ("c", u"F", True),
-    229: ("c", u"I", True),
-    230: ("c", u"I", True),
+    1: ("a", "P", False),
+    2: ("a", "P", True),
+    3: ("m", "P", False),
+    4: ("m", "P", False),
+    5: ("m", "C", False),
+    6: ("m", "P", False),
+    7: ("m", "P", False),
+    8: ("m", "C", False),
+    9: ("m", "C", False),
+    10: ("m", "P", True),
+    11: ("m", "P", True),
+    12: ("m", "C", True),
+    13: ("m", "P", True),
+    14: ("m", "P", True),
+    15: ("m", "C", True),
+    16: ("o", "P", False),
+    17: ("o", "P", False),
+    18: ("o", "P", False),
+    19: ("o", "P", False),
+    20: ("o", "C", False),
+    21: ("o", "C", False),
+    22: ("o", "F", False),
+    23: ("o", "I", False),
+    24: ("o", "I", False),
+    25: ("o", "P", False),
+    26: ("o", "P", False),
+    27: ("o", "P", False),
+    28: ("o", "P", False),
+    29: ("o", "P", False),
+    30: ("o", "P", False),
+    31: ("o", "P", False),
+    32: ("o", "P", False),
+    33: ("o", "P", False),
+    34: ("o", "P", False),
+    35: ("o", "C", False),
+    36: ("o", "C", False),
+    37: ("o", "C", False),
+    38: ("o", "A", False),
+    39: ("o", "A", False),
+    40: ("o", "A", False),
+    41: ("o", "A", False),
+    42: ("o", "F", False),
+    43: ("o", "F", False),
+    44: ("o", "I", False),
+    45: ("o", "I", False),
+    46: ("o", "I", False),
+    47: ("o", "P", True),
+    48: ("o", "P", True),
+    49: ("o", "P", True),
+    50: ("o", "P", True),
+    51: ("o", "P", True),
+    52: ("o", "P", True),
+    53: ("o", "P", True),
+    54: ("o", "P", True),
+    55: ("o", "P", True),
+    56: ("o", "P", True),
+    57: ("o", "P", True),
+    58: ("o", "P", True),
+    59: ("o", "P", True),
+    60: ("o", "P", True),
+    61: ("o", "P", True),
+    62: ("o", "P", True),
+    63: ("o", "C", True),
+    64: ("o", "C", True),
+    65: ("o", "C", True),
+    66: ("o", "C", True),
+    67: ("o", "C", True),
+    68: ("o", "C", True),
+    69: ("o", "F", True),
+    70: ("o", "F", True),
+    71: ("o", "I", True),
+    72: ("o", "I", True),
+    73: ("o", "I", True),
+    74: ("o", "I", True),
+    75: ("t", "P", False),
+    76: ("t", "P", False),
+    77: ("t", "P", False),
+    78: ("t", "P", False),
+    79: ("t", "I", False),
+    80: ("t", "I", False),
+    81: ("t", "P", False),
+    82: ("t", "I", False),
+    83: ("t", "P", True),
+    84: ("t", "P", True),
+    85: ("t", "P", True),
+    86: ("t", "P", True),
+    87: ("t", "I", True),
+    88: ("t", "I", True),
+    89: ("t", "P", False),
+    90: ("t", "P", False),
+    91: ("t", "P", False),
+    92: ("t", "P", False),
+    93: ("t", "P", False),
+    94: ("t", "P", False),
+    95: ("t", "P", False),
+    96: ("t", "P", False),
+    97: ("t", "I", False),
+    98: ("t", "I", False),
+    99: ("t", "P", False),
+    100: ("t", "P", False),
+    101: ("t", "P", False),
+    102: ("t", "P", False),
+    103: ("t", "P", False),
+    104: ("t", "P", False),
+    105: ("t", "P", False),
+    106: ("t", "P", False),
+    107: ("t", "I", False),
+    108: ("t", "I", False),
+    109: ("t", "I", False),
+    110: ("t", "I", False),
+    111: ("t", "P", False),
+    112: ("t", "P", False),
+    113: ("t", "P", False),
+    114: ("t", "P", False),
+    115: ("t", "P", False),
+    116: ("t", "P", False),
+    117: ("t", "P", False),
+    118: ("t", "P", False),
+    119: ("t", "I", False),
+    120: ("t", "I", False),
+    121: ("t", "I", False),
+    122: ("t", "I", False),
+    123: ("t", "P", True),
+    124: ("t", "P", True),
+    125: ("t", "P", True),
+    126: ("t", "P", True),
+    127: ("t", "P", True),
+    128: ("t", "P", True),
+    129: ("t", "P", True),
+    130: ("t", "P", True),
+    131: ("t", "P", True),
+    132: ("t", "P", True),
+    133: ("t", "P", True),
+    134: ("t", "P", True),
+    135: ("t", "P", True),
+    136: ("t", "P", True),
+    137: ("t", "P", True),
+    138: ("t", "P", True),
+    139: ("t", "I", True),
+    140: ("t", "I", True),
+    141: ("t", "I", True),
+    142: ("t", "I", True),
+    143: ("h", "P", False),
+    144: ("h", "P", False),
+    145: ("h", "P", False),
+    146: ("h", "R", False),
+    147: ("h", "P", True),
+    148: ("h", "R", True),
+    149: ("h", "P", False),
+    150: ("h", "P", False),
+    151: ("h", "P", False),
+    152: ("h", "P", False),
+    153: ("h", "P", False),
+    154: ("h", "P", False),
+    155: ("h", "R", False),
+    156: ("h", "P", False),
+    157: ("h", "P", False),
+    158: ("h", "P", False),
+    159: ("h", "P", False),
+    160: ("h", "R", False),
+    161: ("h", "R", False),
+    162: ("h", "P", True),
+    163: ("h", "P", True),
+    164: ("h", "P", True),
+    165: ("h", "P", True),
+    166: ("h", "R", True),
+    167: ("h", "R", True),
+    168: ("h", "P", False),
+    169: ("h", "P", False),
+    170: ("h", "P", False),
+    171: ("h", "P", False),
+    172: ("h", "P", False),
+    173: ("h", "P", False),
+    174: ("h", "P", False),
+    175: ("h", "P", True),
+    176: ("h", "P", True),
+    177: ("h", "P", False),
+    178: ("h", "P", False),
+    179: ("h", "P", False),
+    180: ("h", "P", False),
+    181: ("h", "P", False),
+    182: ("h", "P", False),
+    183: ("h", "P", False),
+    184: ("h", "P", False),
+    185: ("h", "P", False),
+    186: ("h", "P", False),
+    187: ("h", "P", False),
+    188: ("h", "P", False),
+    189: ("h", "P", False),
+    190: ("h", "P", False),
+    191: ("h", "P", True),
+    192: ("h", "P", True),
+    193: ("h", "P", True),
+    194: ("h", "P", True),
+    195: ("c", "P", False),
+    196: ("c", "F", False),
+    197: ("c", "I", False),
+    198: ("c", "P", False),
+    199: ("c", "I", False),
+    200: ("c", "P", True),
+    201: ("c", "P", True),
+    202: ("c", "F", True),
+    203: ("c", "F", True),
+    204: ("c", "I", True),
+    205: ("c", "P", True),
+    206: ("c", "I", True),
+    207: ("c", "P", False),
+    208: ("c", "P", False),
+    209: ("c", "F", False),
+    210: ("c", "F", False),
+    211: ("c", "I", False),
+    212: ("c", "P", False),
+    213: ("c", "P", False),
+    214: ("c", "I", False),
+    215: ("c", "P", False),
+    216: ("c", "F", False),
+    217: ("c", "I", False),
+    218: ("c", "P", False),
+    219: ("c", "F", False),
+    220: ("c", "I", False),
+    221: ("c", "P", True),
+    222: ("c", "P", True),
+    223: ("c", "P", True),
+    224: ("c", "P", True),
+    225: ("c", "F", True),
+    226: ("c", "F", True),
+    227: ("c", "F", True),
+    228: ("c", "F", True),
+    229: ("c", "I", True),
+    230: ("c", "I", True),
 }
 
 centering = {
     1: "P",
     2: "P",
     3: "P",
     4: "P",
```

### Comparing `seekpath-2.0.1/seekpath/brillouinzone/brillouinzone.py` & `seekpath-2.1.0/seekpath/brillouinzone/brillouinzone.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         points = np.array([hull.points[i] for i in simplex])
         center = points.sum(axis=0) / float(len(points))
 
         # Get normal vector (with direction!)
         normal = np.cross(center - points[1], center - points[0])
         # Normalize, then rescale to a small value
         normal = normal / np.linalg.norm(normal)
-        max_length = np.sqrt((points ** 2).sum(axis=1).max())
+        max_length = np.sqrt((points**2).sum(axis=1).max())
         normal /= max_length
         normal *= 1.0e-4
         point_up = center + normal
         point_down = center - normal
         delaunay = Delaunay(hull.points)
         is_up_inside = delaunay.find_simplex(point_up) >= 0
         is_down_inside = delaunay.find_simplex(point_down) >= 0
```

### Comparing `seekpath-2.0.1/seekpath/util.py` & `seekpath-2.1.0/seekpath/util.py`

 * *Files identical despite different names*

### Comparing `seekpath-2.0.1/seekpath/getpaths.py` & `seekpath-2.1.0/seekpath/getpaths.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 This module contains the main functions to get a path and an explicit path.
 """
 import numpy as np
+import warnings
+from . import SupercellWarning
 
 
 def get_explicit_from_implicit(  # pylint: disable=too-many-locals
     seekpath_output, reference_distance
 ):
     """
     Given the output of ``get_path`` by seekpath, compute an "explicit" path,
@@ -321,7 +323,286 @@
 
     explicit_res = get_explicit_from_implicit(
         res, reference_distance=reference_distance
     )
     for k, v in explicit_res.items():
         res["explicit_{}".format(k)] = v
     return res
+
+
+def get_path_orig_cell(
+    structure,
+    with_time_reversal=True,
+    recipe="hpkot",
+    threshold=1.0e-7,
+    symprec=1e-05,
+    angle_tolerance=-1.0,
+):
+    r"""
+    Return the kpoint path information for band structure given a
+    crystal structure, using the paths from the chosen recipe/reference.
+    The original unit cell (i.e., the one provided in input by the user) is used.
+    Standardization or symmetrization of the input unit cell is not performed.
+
+    If the provided unit cell is a supercell of a smaller primitive cell,
+    return the standard k path of the smaller primitive cell in the basis
+    of the supercell reciprocal lattice vectors. In this case, the k-point
+    labels lose their meaning as the corresponding k-points are not at the
+    high-symmetry points of the first BZ of the given supercell. A
+    :py:exc:`~seekpath.SupercellWarning` is issued.
+
+    If you use this module, please cite the paper of the corresponding
+    recipe (see parameter below).
+
+    :param structure: The crystal structure for which we want to obtain
+        the suggested path. It should be a tuple in the format
+        accepted by spglib: ``(cell, positions, numbers)``, where
+        (if N is the number of atoms):
+
+        - ``cell`` is a :math:`3 \times 3` list of floats (``cell[0]`` is the first lattice
+          vector, ...)
+        - ``positions`` is a :math:`N \times 3` list of floats with the atomic coordinates
+          in scaled coordinates (i.e., w.r.t. the cell vectors)
+        - ``numbers`` is a length-:math:`N` list with integers identifying uniquely
+          the atoms in the cell (e.g., the Z number of the atom, but
+          any other positive non-zero integer will work - e.g. if you
+          want to distinguish two Carbon atoms, you can set one number
+          to 6 and the other to 1006)
+
+    :param with_time_reversal: if False, and the group has no inversion
+        symmetry, additional lines are returned as described in the HPKOT
+        paper.
+
+    :param recipe: choose the reference publication that defines the special
+       points and paths.
+       Currently, the following value is implemented:
+
+       - ``hpkot``: HPKOT paper:
+         Y. Hinuma, G. Pizzi, Y. Kumagai, F. Oba, I. Tanaka, Band structure
+         diagram paths based on crystallography, Comp. Mat. Sci. 128, 140 (2017).
+         DOI: 10.1016/j.commatsci.2016.10.015
+
+    :param threshold: the threshold to use to verify if we are in
+        and edge case (e.g., a tetragonal cell, but ``a==c``). For instance,
+        in the tI lattice, if ``abs(a-c) < threshold``, a
+        :py:exc:`~seekpath.hpkot.EdgeCaseWarning` is issued.
+        Note that depending on the bravais lattice, the meaning of the
+        threshold is different (angle, length, ...)
+
+    :param symprec: the symmetry precision used internally by SPGLIB
+
+    :param angle_tolerance: the angle_tolerance used internally by SPGLIB
+
+
+    :return: a dictionary with the following
+      keys:
+
+        - ``point_coords``: a dictionary with label -> float coordinates
+        - ``path``: a list of length-2 tuples, with the labels of the starting
+          and ending point of each label section
+          input crystal structure has inversion symmetry or not.
+        - ``augmented_path``: if True, it means that the path was
+          augmented with the :math:`-k` points (this happens if both
+          has_inversion_symmetry is False, and the user set
+          with_time_reversal=False in the input)
+        - ``is_supercell``: True if the input unit cell is a supercell of
+          a smaller primitive cell.
+
+    :note: An :py:exc:`~seekpath.hpkot.EdgeCaseWarning` is issued for
+        edge cases (e.g. if ``a==b==c`` for
+        orthorhombic systems). In this case, still one of the valid cases
+        is picked.
+    """
+
+    res = get_path(
+        structure=structure,
+        with_time_reversal=with_time_reversal,
+        threshold=threshold,
+        symprec=symprec,
+        angle_tolerance=angle_tolerance,
+        recipe=recipe,
+    )
+
+    is_supercell = abs(res["volume_original_wrt_prim"] - 1) > 0.1
+
+    if is_supercell:
+        warnings.warn(
+            "The provided cell is a supercell: the returned k-path is the "
+            "standard k-path of the associated primitive cell in the basis of "
+            "the supercell reciprocal lattice.",
+            SupercellWarning,
+        )
+
+    # points in the output of get_path are in scaled coordinates of the
+    # standardized primitive lattice
+    points_scaled_standard = res["point_coords"]
+
+    # Convert points from scaled coordinates of the standardiced primitive
+    # lattice to Cartesian coordinates
+    points_cartesian = {}
+    for pointname, coords in points_scaled_standard.items():
+        points_cartesian[pointname] = coords @ np.array(
+            res["reciprocal_primitive_lattice"]
+        )
+
+    # Rotate points in Cartesian space
+    for pointname, coords in points_cartesian.items():
+        points_cartesian[pointname] = coords @ res["rotation_matrix"]
+
+    # Convert points from Cartesian coordinates to the scaled coordinates
+    # of the original lattice
+    points_scaled_original = {}
+    cell_orig = np.array(structure[0])
+    for pointname, coords in points_cartesian.items():
+        points_scaled_original[pointname] = list(coords @ cell_orig.T / np.pi / 2)
+
+    res_orig = {
+        "point_coords": points_scaled_original,
+        "path": res["path"],
+        "augmented_path": res["augmented_path"],
+        "is_supercell": is_supercell,
+        "has_inversion_symmetry": res["has_inversion_symmetry"],
+        "bravais_lattice": res["bravais_lattice"],
+        "bravais_lattice_extended": res["bravais_lattice_extended"],
+        "spacegroup_number": res["spacegroup_number"],
+        "spacegroup_international": res["spacegroup_international"],
+    }
+
+    return res_orig
+
+
+def get_explicit_k_path_orig_cell(
+    structure,
+    with_time_reversal=True,
+    reference_distance=0.025,
+    recipe="hpkot",
+    threshold=1.0e-7,
+    symprec=1e-05,
+    angle_tolerance=-1.0,
+):
+    r"""
+    Return the kpoint path for band structure (in scaled and absolute
+    coordinates), given a crystal structure,
+    using the paths proposed in the various publications (see description
+    of the 'recipe' input parameter) for the given unit cell.
+    Standardization or symmetrization of the input unit cell is not performed.
+
+    If the provided unit cell is a supercell of a smaller primitive cell,
+    return the standard k path of the smaller primitive cell in the basis
+    of the supercell reciprocal lattice vectors. In this case, the k-point
+    labels lose their meaning as the corresponding k-points are not at the
+    high-symmetry points of the first BZ of the given supercell. A
+    :py:exc:`~seekpath.SupercellWarning` is issued.
+
+    If you use this module, please cite the paper of the corresponding
+    recipe (see parameter below).
+
+    :param structure: The crystal structure for which we want to obtain
+        the suggested path. It should be a tuple in the format
+        accepted by spglib: (cell, positions, numbers), where
+        (if N is the number of atoms):
+
+        - ``cell`` is a :math:`3 \times 3` list of floats (``cell[0]`` is the first lattice
+          vector, ...)
+        - ``positions`` is a :math:`N \times 3` list of floats with the atomic coordinates
+          in scaled coordinates (i.e., w.r.t. the cell vectors)
+        - ``numbers`` is a length-:math:`N` list with integers identifying uniquely
+          the atoms in the cell (e.g., the Z number of the atom, but
+          any other positive non-zero integer will work - e.g. if you
+          want to distinguish two Carbon atoms, you can set one number
+          to 6 and the other to 1006)
+
+    :param with_time_reversal: if False, and the group has no inversion
+        symmetry, additional lines are returned.
+
+    :param reference_distance: a reference target distance between neighboring
+        k-points in the path, in units of 1/ang. The actual value will be as
+        close as possible to this value, to have an integer number of points in
+        each path.
+
+    :param recipe: choose the reference publication that defines the special
+       points and paths.
+       Currently, the following value is implemented:
+
+       - ``hpkot``: HPKOT paper:
+         Y. Hinuma, G. Pizzi, Y. Kumagai, F. Oba, I. Tanaka, Band structure
+         diagram paths based on crystallography, Comp. Mat. Sci. 128, 140 (2017).
+         DOI: 10.1016/j.commatsci.2016.10.015
+
+    :param threshold: the threshold to use to verify if we are in
+        and edge case (e.g., a tetragonal cell, but ``a==c``). For instance,
+        in the tI lattice, if ``abs(a-c) < threshold``, a
+        :py:exc:`~seekpath.hpkot.EdgeCaseWarning` is issued.
+        Note that depending on the bravais lattice, the meaning of the
+        threshold is different (angle, length, ...)
+
+    :param symprec: the symmetry precision used internally by SPGLIB
+
+    :param angle_tolerance: the angle_tolerance used internally by SPGLIB
+
+    .. versionchanged:: 1.8
+        The key ``segments`` has been renamed ``explicit_segments``
+        for consistency.
+
+    :return: a dictionary with a number of keys. They are the same as
+        ``get_path_orig_cell``, plus a few ones:
+
+        - ``explicit_kpoints_abs``: List of the kpoints along the specific path in
+          absolute (Cartesian) coordinates. The two endpoints are always
+          included, independently of the length.
+        - ``explicit_kpoints_rel``: List of the kpoints along the specific path in
+          relative (fractional) coordinates (same length as
+          explicit_kpoints_abs).
+        - ``explicit_kpoints_labels``: list of strings with kpoints labels. It has
+          the same length as explicit_kpoints_abs and explicit_kpoints_rel.
+          Empty if the point is not a special point.
+        - ``explicit_kpoints_linearcoord``: array of floats, giving the coordinate
+          at which to plot the corresponding point.
+        - ``explicit_segments``: a list of length-2 tuples, with the start and end
+          index of each segment. **Note**! The indices are supposed to be
+          used as follows: the labels for the i-th segment are given by::
+
+            segment_indices = explicit_segments[i]
+            segment_labels = explicit_kpoints_labels[slice(*segment_indices)]
+
+          This means, in particular, that if you want the label of the start
+          and end points, you should do::
+
+            start_label = explicit_kpoints_labels[segment_indices[0]]
+            stop_label = explicit_kpoints_labels[segment_indices[1]-1]
+
+          (note the minus one!)
+
+          Also, note that if
+          ``explicit_segments[i-1][1] == explicit_segments[i][0] + 1`` it means
+          that the point was calculated only once, and it belongs to both
+          paths. Instead, if
+          ``explicit_segments[i-1][1] == explicit_segments[i][0]``, then
+          this is a 'break' point in the path (e.g., ``explicit_segments[i-1][1]``
+          is the X point, and ``explicit_segments[i][0]`` is the R point,
+          and typically in a graphical representation they are shown at the
+          same coordinate, with a label ``R|X``).
+    """
+    from .hpkot.tools import get_reciprocal_cell_rows
+
+    res = get_path_orig_cell(
+        structure=structure,
+        with_time_reversal=with_time_reversal,
+        threshold=threshold,
+        symprec=symprec,
+        angle_tolerance=angle_tolerance,
+        recipe=recipe,
+    )
+
+    # Set reciprocal_primitive_lattice as the reciprocal lattice of the original
+    # cell. To be used only in the get_explicit_from_implicit function.
+    res["reciprocal_primitive_lattice"] = get_reciprocal_cell_rows(structure[0])
+
+    explicit_res = get_explicit_from_implicit(
+        res, reference_distance=reference_distance
+    )
+
+    res.pop("reciprocal_primitive_lattice")
+
+    for k, v in explicit_res.items():
+        res["explicit_{}".format(k)] = v
+    return res
```

### Comparing `seekpath-2.0.1/setup.py` & `seekpath-2.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     # of the difference and
     # http://blog.miguelgrinberg.com/post/the-package-dependency-blues
     # for a useful dicussion
     install_requires=["numpy>=1.0", "spglib>=1.14.1"],
     extras_require={
         "bz": ["scipy>=1"],
         "dev": [
-            "pre-commit>=1.4",
-            "black==19.10b0",
+            "pre-commit==3.3.2",
+            "black==23.3.0",
             "prospector==1.2.0",
             "pylint==2.4.4",
-            "pytest==5.3.5",
+            "pytest==7.3.1",
         ],
     },
     python_requires=">=3.5",
     packages=find_packages(),
     # Needed to include some static files declared in MANIFEST.in
     include_package_data=True,
     download_url="https://github.com/giovannipizzi/seekpath/archive/v{}.tar.gz".format(
```

### Comparing `seekpath-2.0.1/README.rst` & `seekpath-2.1.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 #########
 SeeK-path
 #########
 
-Test status: branch `master`: |travismaster|; branch `develop`: |travisdevelop|
+Test status for default branch: |continuousintegration|
 
-.. |travismaster| image:: https://travis-ci.org/giovannipizzi/seekpath.svg?branch=master
-    :target: https://travis-ci.org/giovannipizzi/seekpath
-
-.. |travisdevelop| image:: https://travis-ci.org/giovannipizzi/seekpath.svg?branch=develop
-    :target: https://travis-ci.org/giovannipizzi/seekpath
+.. |continuousintegration| image:: https://github.com/giovannipizzi/seekpath/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/giovannipizzi/seekpath/actions/workflows/ci.yml
 
 ``SeeK-path`` is a python module to obtain band paths in the
 Brillouin zone of crystal structures.
 
 The definition of k-point labels follows crystallographic convention, as defined
 and discussed in the `HPKOT paper`_. Moreover, the Bravais lattice is detected
 properly using the spacegroup symmetry. Also the suggested band path provided
@@ -38,14 +35,20 @@
 
 =============================
 How to install and how to use
 =============================
 
 Please check the SeeK-path `user guide on ReadTheDocs`_.
 
+================
+Acknowledgements
+================
+
+* Jae-Mo Lihm: k-point paths for the original unit cell (i.e., the one provided in input by the user) without standardization or symmetrization
+
 =======
 License
 =======
 
 The code is open-source (licensed with a MIT license, see LICENSE.txt).
 
 ===================
@@ -74,8 +77,8 @@
 .. _JOURNAL LINK: http://dx.doi.org/10.1016/j.commatsci.2016.10.015
 .. _arXiv link: https://arxiv.org/abs/1602.06402
 .. _spglib: http://atztogo.github.io/spglib/
 .. _Materials Cloud: http://www.materialscloud.org/tools/seekpath/
 .. _docker hub: https://hub.docker.com/r/giovannipizzi/seekpath/
 .. _user guide on ReadTheDocs: http://seekpath.readthedocs.io
 .. _spglib arXiv link: https://arxiv.org/abs/1808.01590
-.. _tools-seekpath: http://www.github.com/materialscloud-org/tools-seekpath/
+.. _tools-seekpath: http://www.github.com/materialscloud-org/tools-seekpath/
```

